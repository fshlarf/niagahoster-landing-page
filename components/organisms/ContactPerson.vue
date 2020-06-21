<template>
    <div class="cp">
        <div class="container">
            <div class="cp__title">
                <p>Perlu <b>BANTUAN?</b> Hubungi Kami : <b>0274-5305505</b></p>
            </div>
            <div class="cp__channel">
               <i class="icon fa icon fa-comments"></i>
               <span>Live Chat</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.cp {
    padding: 43px 0px;
    background-color: #00a2f3;
    color: white!important;
    .container {
        max-width: 1120px!important;
        margin: 0 auto !important;
        display: flex;
    }
    &__title {
        width: 75%;
        p {
            padding-top: 5px;
            font-weight: 300 !important;
            font-size: 32px;
        }
    }
    &__channel {
        cursor: pointer;
        padding: 0px 30px;
        border: 1px white solid;
        border-radius: 25px;
        display: flex;
        margin-left: auto;
        height: 48px;
        span {
            font-size: 16px;
            margin-top: 10px;
        }
        i {
            padding: 0px;
            margin-right: 16px;
            font-size: 28px;
            margin-top: 8px;
        }
    }
}
@media (max-width: 800px) {
    .container {
        display: block!important;
    }
    .cp__title {
        width: 100%;
        p {
            font-size: 18px!important;
        }
    }
    .cp__channel {
        width: fit-content;
        margin: 0 auto;
    }
}
</style>