<template>
    <div class="price">
        <div class="container">
            <div v-for="(item, id) in packagesPrice" :key="id">
                <CardPrice
                    :result="item"
                />
            </div>
        </div>
    </div>
</template>

<script>
import axios from 'axios'
import CardPrice from '../mollecules/CardPrice'
export default {
    components: {
        CardPrice
    },
    data() {
        return {
            packagesPrice: []
        }
    },
    mounted() {
        this.getDataPackages()
    },
    methods: {
        getDataPackages() {
            axios.get('https://demo8935229.mockable.io/')
            .then(res => {
                this.packagesPrice = res.data.packages
                console.log(this.packages);
            })
            .catch(err => {
                console.log(err)
            })
        }
    }
}
</script>

<style lang="scss" scoped>
.price {
    padding: 30px 16px;
    margin-bottom: 70px;
    .container {
        display: flex;
        margin: 0 auto;
    }
}
</style>