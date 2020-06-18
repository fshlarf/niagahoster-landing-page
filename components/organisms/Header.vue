<template>
    <div>
        <div class="header">
            <div class="header__bar">
                <ul class="nav header__bar-left">
                    <li class="nav-item">
                        <img class="label-img" src="/images/ng-label.png">
                        <a class="nav-link" href="#" style="padding-left: 8px;">Gratis Ebook 9 Cara Cerdas Menggunakan Domain [ x ]</a>
                    </li>
                </ul>
                <ul class="nav justify-content-end">
                    <li class="nav-item">
                        <i class="icon fa fa-phone"></i>
                        <a class="nav-link" href="#">0274-5305505</a>
                    </li>
                    <li class="nav-item">
                        <i class="icon fa icon fa-comments"></i>
                        <a class="nav-link" href="#">Live Chat</a>
                    </li>
                    <li class="nav-item">
                        <i class="icon fa fa-user-circle"></i>
                        <a class="nav-link" href="#">Member Area</a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="header main">
            <div class="header__bar">
                <ul class="nav header__bar-left">
                    <img class="header__bar-left--img" src="/images/niagahoster.jpg">
                </ul>
                <ul class="nav justify-content-end">
                    <li class="nav-item">
                        <a class="nav-link" href="#">Hosting</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Domain</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Server</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Website</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Afiliasi</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Promo</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Pembayaran</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Review</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Kontak</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Blog</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.header {
    border-bottom: 1px #ddd solid;
    &.main {
        height: 73px;
        .nav-item {
            margin-top: 16px;
        }
    }
    &__bar{
        max-width: 1120px!important;
        font-size: 12px;
        font-weight: 500;
        margin: 0 auto;
        &-left {
            position: absolute;    
            width: 36%;
            &--img {
                height: auto;
                width: 191px;
            }
            .label-img {
                margin-left: 11px;
                height: auto;
                width: 34px;
            }
        }
    }
    a {
        color: black!important;
    }
    .nav-item {
        display: flex; 
        cursor: pointer;   
    }
}
</style>