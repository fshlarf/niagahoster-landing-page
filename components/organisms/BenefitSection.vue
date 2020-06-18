<template>
    <div>
        <div class="benefit container" align="center">
            <h4 class="benefit__header"> Semua Paket Sudah Termasuk</h4>
            <div class="row">
                <ImageBenefit
                    fileImg="icon PHP Hosting_PHP Semua Versi.svg"
                    title="PHP Semua Versi"
                    desc="Pilih mulai dari versi PHP 5.3 s/d PHP 7<br>Ubah sesuka Anda"
                />
                <ImageBenefit
                    fileImg="icon PHP Hosting_My SQL.svg"
                    title="MySQL Versi 5.6"
                    desc="Nikmati MySQL versi terbaru, tercepat dan<br>kaya akan fitur"
                />
                 <ImageBenefit
                    fileImg="icon PHP Hosting_CPanel.svg"
                    title="Panel Hosting cPanel"
                    desc="Kelola website dengan panel canggih yang <br>familiar di hati Anda"
                />
            </div>
            <div class="row">
                <ImageBenefit
                    fileImg="icon PHP Hosting_garansi uptime.svg"
                    title="Garansi Uptime 99.9%"
                    desc="Data center yang mendukung kelangsungan<br>website Anda 24/7"
                />
                <ImageBenefit
                    fileImg="icon PHP Hosting_InnoDB.svg"
                    title="Database InnoDB Unlimited"
                    desc="Jumlah dan ukuran database yang tumbuh <br>sesuai kebutuhan Anda"
                />
                 <ImageBenefit
                    fileImg="icon PHP Hosting_My SQL remote.svg"
                    title="Wilcard Remote MySQL"
                    desc="Mendukung s/d 25 max_user_connections<br>dan 100 max_connections"
                />
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
    padding: 40px 40px;
    text-align: center;
    position: relative;
    min-height: 150px;
    &__content {
        img {
            margin-bottom: 20px;
        }
    }
}
</style>