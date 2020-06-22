<template>
    <div class="product">
        <div class="container">
            <div class="row">
                <div class="col">
                    <div class="product__header">
                        <h2 class="product__header-h2">PHP Hosting</h2>
                        <h2>Cepat, handal, penuh dengan</h2>
                        <h2>modul PHP yang anda butuhkan</h2>
                    </div>
                    <div class="product__content">
                        <LabelChecked
                            title="Solusi PHP untuk performa query yang lebih cepat"
                        />
                        <LabelChecked
                            title="Konsumsi memory yang lebih rendah"
                        />
                        <LabelChecked
                            title="Support PHP 5.3, PHP 5.4, PHP 5.5, PHP 5.6, PHP 7"
                        />
                        <LabelChecked
                            title="Fitur enkripsi IonCube dan Zend Guard Loaders"
                        />
                    </div>
                </div>
                <div class="product__img">
                    <img src="~/assets/images/php-hosting.svg">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import LabelChecked from '../atoms/LabelChecked'
export default {
    components: {
        LabelChecked
    }
}
</script>

<style lang="scss" scoped>
.product {
    border-bottom: 1px #ddd solid;
    padding: 40px 0px !important;
    .container {
        max-width: 1120px!important;
        font-weight: 500 !important;
        margin: 0 auto !important;
    }
    &__header {
        &-h2 {
            font-weight: 700 !important;
            margin-bottom: 8px !important;
        }
        h2 {
            margin-bottom: 0px;
            font-weight: 300;
        }
    }
    &__content {
        margin-top: 20px;
    }
    &__img {
        img {
            width: 29rem;
        }
    }
    .row {
        padding: 0px 8px !important;
    }
}
@media (max-width: 800px) {
    img {
        width: 180px!important;
        margin: 0 auto!important;
    }
    .row {
        display:block;
    }
    .product__img {
        text-align: center;
        margin-top: 20px;
    }
    h2 {
        font-size: 20px;
    }
}
@media  only screen and (min-width: 880px) and (max-width: 1020px) {
    .container {
        display: contents!important;
    }
}
</style>