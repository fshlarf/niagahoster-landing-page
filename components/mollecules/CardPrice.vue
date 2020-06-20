<template>
    <div class="card" v-if="result">
        <img class="best-seller" v-if="result.best_seller" src="/images/best-seller.png" alt="">
        <table :style="[ result.best_seller && { 'border-color': '#008fee' }]">
            <tr :class="setClassPrice(result.best_seller)" :style="[ result.best_seller && { 'border-color': '#008fee' }]"><td><h3>{{ result.type }}</h3></td></tr>
            <tr :class="setClassPrice(result.best_seller)" :style="[ result.best_seller && { 'border-color': '#008fee' }]">
                <td>
                    <span style="text-decoration: line-through;">Rp {{ formatCurrency(result.price) }}</span>
                    <div class="price-cont"> 
                        <p>Rp&nbsp;</p>
                        <p class="big-price">{{ setBigSizePrice(result.price_disc) }}</p>
                        <p style="font-weight: 800">{{ setMiniSizePrice(result.price_disc) }}</p>
                        <p>/bln</p>
                    </div>
                </td>
            </tr>
            <tr :class="setClassUsers(result.best_seller)" :style="[ result.best_seller && { 'border-color': '#008fee' }]"><td><b>{{ formatCurrency(result.total_users) }}</b> Pengguna Terdaftar</td></tr>
            <tr style="border-bottom: none" :style="[ result.best_seller && { 'border-color': '#008fee' }]">
                <div class="list-benefit">
                    <td v-for="(item, id) in result.benefits" :key="id">
                        <div v-html="item" v-if="item !== '5 stars'"></div>
                        <img src="/images/five-star.png" alt="" v-if="item == '5 stars'">
                    </td>
                </div>
            </tr>
            <tr style="border: none;" :style="[ result.best_seller && { 'border-color': '#008fee' }]">
                <div class="btn-container">
                    <button type="button" :class="`benefit__btn btn ${setClassBtn(result.best_seller)}`">Pilih Hoting Anda</button>
                </div>
            </tr>
        </table>
    </div>
</template>

<script>
export default {
    props: {
        result: Object
    },
    methods: {
        setBigSizePrice(val) {
            let value = val.toString().replace(/(\d)(?=(\d{3})+(?!\d))/g, '$1.')
            let newVal = value.split('.')
            return ` ${newVal[0]}`
        },
        setMiniSizePrice(val) {
            let value = val.toString().replace(/(\d)(?=(\d{3})+(?!\d))/g, '$1.')
            let newVal = value.split('.')
            return `.${newVal[1]}`
        },
        setClassPrice(param) {
            if (param) return 'row-price'
        },
        setClassUsers(param) {
            if (param) return 'row-users'
        },
        setClassBtn(param) {
            return param ? 'btn-primary' : 'btn-secondary'
        },
        formatCurrency(val) {
            return val.toString().replace(/(\d)(?=(\d{3})+(?!\d))/g, '$1.')
        }
    }
}
</script>

<style lang="scss" scoped>
.card {
    width: 19rem;
    text-align: center;
    table {
        font-family: arial, sans-serif;
        border-collapse: collapse;
        width: 100%;
        border: 1px solid #dddddd;
        max-width: 350px;
        margin: 0 auto;
    }
    tr {
        border: 1px solid #dddddd;
        button {
            font-weight: 700!important;
        }
    }
    td, th {
        text-align: left;
        padding: 8px;
        text-align: center;
        display: block;
    }
    h3 {
        font-weight: 700!important;
    }
    .best-seller {
        position: absolute;
        margin-left: -12px;
        margin-top: -10px;
        width: 116px;
    }
    .list-benefit {
        padding: 25px 0px;
        p {
            margin: 0px!important;
        }
    }
    .btn-container {
        padding: 30px 0px;
        margin-top: -20px;
    }
    .big-price {
        font-size: 50px;
        margin-top: -14px;
    }
    .price-cont {
        display: flex; margin-left: 70px;
        margin-top: 16px;
        p {
            margin-bottom: 0px;
        }
        }
        .row {
            &-users {
                background-color: #007fde;
                border-color: #007fde;
                color: white;
            }
            &-price {
                background-color: #008fee;
                color: white;
            }
        }
    }
</style>