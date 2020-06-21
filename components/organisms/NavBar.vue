<template>
    <div>
        <nav class="header navbar navbar-expand-lg navbar-light bg-light">
            <a class="navbar-brand header__bar-left">
                <img class="header__bar-left--img" src="/images/niagahoster.jpg">
            </a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav justify-content-end header__bar-right">
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
        </nav>
        <hr>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
hr {
    margin: 0px;
}
.header {
    background-color: white!important;
    max-width: 1120px!important;
    margin: 0 auto;
    padding: 8px 0px;
    &.main {
        height: 73px;
        .nav-item {
            margin-top: 16px;
        }
    }
    &__bar{
        display: flex;
        font-size: 12px;
        font-weight: 500;
        width: -webkit-fill-available;
        &-left {
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
        &-right {
            padding: 0px 10px 0px 20px;
            margin-left: auto;
            align-self: center;
        }
    }
    a {
        color: black!important;
    }
    .nav-item {
        display: flex; 
        cursor: pointer;   
    }
    .navbar-toggler {
        height: 55px;
        border-radius: 10px!important;
    }
}
</style>