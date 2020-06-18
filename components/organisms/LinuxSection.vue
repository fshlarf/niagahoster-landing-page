<template>
  <div class="linux">
        <div class="container">
            <h4>Linux Hosting yang Stabil<br>dengan Teknologi LVE</h4>
            <div class="row">
                <div class="col">
                    <div class="linux__content">
                        <p>
                            Super Micro <b>Intel Xeon 24-Cores</b> server dengan RAM <b>128 GB</b> dan<br>
                            teknologi <b>LVE CloudLinux</b> untuk stabilitas server Anda. Dilengkapi<br>
                            dengan <b>SSD</b> untuk kecepatan <b>MySQL</b> dan caching. Apache load balancer<br>
                            berbasis LiteSpeed Technologies, <b>CageFS</b> security, <b>Raid-10</b> protection<br>
                            dan auto backup untuk keamanan website PHP Anda.
                        </p>
                    </div>
                    <button type="button" class="linux__btn btn btn-primary">Pilih Hoting Anda</button>
                </div>
                <div class="linux__img">
                    <img src="/images/image_support.png">
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
.linux {
    h4 {
        text-align: left!important;
    }
    border-bottom: 1px #ddd solid;
    padding: 40px 0px !important;
    .conatiner {
        max-width: 1120px!important;
        font-weight: 500 !important;
        margin: 0 auto !important;
    }
    &__content {
        padding: 0px 16px!important;
    }
    &__content {
        p {
            margin-left: -20px;
        }
    }
    &__img {
        img {
            width: 26rem;
        }
    }
    .row {
        padding: 0px 8px !important;
    }
    &__btn {
        margin-top: 16px;
    }
}
</style>