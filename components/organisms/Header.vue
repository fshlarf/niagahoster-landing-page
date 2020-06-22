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
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.header {
    border-bottom: 1px #ddd solid;
    &__bar{
        max-width: 1120px!important;
        font-size: 12px;
        font-weight: 500;
        margin: 0 auto;
        &-left {
            position: absolute;    
            width: 50%;
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
@media (max-width: 800px) {
    .header {
        display: none;
    }
}
</style>