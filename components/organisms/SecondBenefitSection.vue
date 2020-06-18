<template>
  <div class="benefit">
        <div class="container">
            <h4>Mendukung Penuh Framework laravel</h4>
            <div class="row">
                <div class="col">
                    <div class="benefit__header">
                        <p>
                            Tak perlu menggunakan dedicated server ataupun VPS<br>
                            yang mahal. Layanan PHP hosting murah kami<br>
                            mendukung penuh framework favorit Anda
                        </p>
                    </div>
                    <div class="benefit__content">
                        <LabelChecked>
                            <p>Install Laravel <b>1 klik</b> dengan Softaculous</p>
                        </LabelChecked>
                         <LabelChecked>
                            <p>Mendukung eksetensi <b>PHP MCrypt, phar, mbstrig, json,</b> dan <b>fileinfo</b></p>
                        </LabelChecked>
                        <LabelChecked>
                            <p>Tersedia <b>Composer</b> dan <b>SSH</b> untuk menginstall package pilihan Anda</p>
                        </LabelChecked>
                    </div>
                    <p class="benefit__notes">Nb. Composer dan SSH hanya tersedia pada paket Personal dan Bisnis</p>
                    <button type="button" class="benefit__btn btn btn-primary">Pilih Hoting Anda</button>
                </div>
                <div class="benefit__img">
                    <img src="/images/support_laravel.svg">
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
.benefit {
    h4 {
        text-align: center;
    }
    border-bottom: 1px #ddd solid;
    padding: 40px 0px !important;
    .conatiner {
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
        p {
            margin-left: -20px;
        }
    }
    &__img {
        img {
            width: 28rem;
        }
    }
    .row {
        padding: 0px 8px !important;
    }
    &__notes {
        margin-top: 12px;
        font-size: 12px;
    }
    &__btn {
        margin-top: 16px;
    }
}
</style>