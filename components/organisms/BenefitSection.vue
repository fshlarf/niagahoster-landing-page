<template>
    <div>
        <div class="benefit container" align="center">
            <h4 class="benefit__header"> Semua Paket Sudah Termasuk</h4>
            <div>

                <div class="row">
                    <div class="benefit__item col">
                        <img src="~assets/images/icon PHP Hosting_PHP Semua Versi.svg" alt="Image not found">
                        <ImageBenefit
                            title="PHP Semua Versi"
                            desc="Pilih mulai dari versi PHP 5.3 s/d PHP 7<br>Ubah sesuka Anda"
                        />
                    </div>
                    <div class="benefit__item col">
                        <img src="~assets/images/icon PHP Hosting_My SQL.svg" alt="Image not found">
                        <ImageBenefit
                            title="MySQL Versi 5.6"
                            desc="Nikmati MySQL versi terbaru, tercepat dan<br>kaya akan fitur"
                        />
                    </div>
                    <div class="benefit__item col">
                        <img src="~assets/images/icon PHP Hosting_CPanel.svg" alt="Image not found">
                        <ImageBenefit
                            title="Panel Hosting cPanel"
                            desc="Kelola website dengan panel canggih yang <br>familiar di hati Anda"
                        />
                    </div>
                </div>
                <div class="row">
                    <div class="benefit__item col">
                        <img src="~assets/images/icon PHP Hosting_garansi uptime.svg" alt="Image not found">
                        <ImageBenefit
                            title="Garansi Uptime 99.9%"
                            desc="Data center yang mendukung kelangsungan<br>website Anda 24/7"
                        />
                    </div>
                    <div class="benefit__item col">
                        <img src="~assets/images/icon PHP Hosting_InnoDB.svg" alt="Image not found">
                        <ImageBenefit
                            title="Database InnoDB Unlimited"
                            desc="Jumlah dan ukuran database yang tumbuh <br>sesuai kebutuhan Anda"
                        />
                    </div>
                    <div class="benefit__item col">
                        <img src="~assets/images/icon PHP Hosting_My SQL remote.svg" alt="Image not found">
                        <ImageBenefit
                            title="Wilcard Remote MySQL"
                            desc="Mendukung s/d 25 max_user_connections<br>dan 100 max_connections"
                        />
                    </div>
                </div>
            </div>
        </div>
        <MiniCenteredLine/>
    </div>
</template>

<script>
import ImageBenefit from '~/components/mollecules/ImageBenefit'
import MiniCenteredLine from '~/components/atoms/MiniCenteredLine'
export default {
    components: {
        ImageBenefit,
        MiniCenteredLine
    }
}
</script>

<style lang="scss" scoped>
.benefit {
    padding: 40px 20px;
    text-align: center;
    position: relative;
    min-height: 150px;
    &__item {
        margin-top: 20px; 
        margin-bottom: 20px;
        padding: 0px 16px
    }
    img {
        margin-bottom: 20px;
        width: 5rem;
    }
    .row {
        margin: 0 auto;
    }
}
@media (max-width: 800px) {
    img {
        margin: 0 auto;
    }
    .row {
        display: block!important;
    }
}
</style>