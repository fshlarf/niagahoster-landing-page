<template>
  <div class="linux">
        <div class="linux__content">
            <div class="linux__content-info">
                <h4>Linux Hosting yang Stabil<br>dengan Teknologi LVE</h4>
                <p>
                    Super Micro <b>Intel Xeon 24-Cores</b> server dengan RAM <b>128 GB</b> dan<br>
                    teknologi <b>LVE CloudLinux</b> untuk stabilitas server Anda. Dilengkapi<br>
                    dengan <b>SSD</b> untuk kecepatan <b>MySQL</b> dan caching. Apache load balancer<br>
                    berbasis LiteSpeed Technologies, <b>CageFS</b> security, <b>Raid-10</b> protection<br>
                    dan auto backup untuk keamanan website PHP Anda.
                </p>
                <button type="button" class="linux__btn btn btn-primary">Pilih Hoting Anda</button>
            </div>
            <div class="linux__content-img">
                <img src="~/assets/images/image_support.png">
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
    padding: 20px 0px 0px 0px!important;
    h4 {
        text-align: left!important;
    }
    &__content {
        max-width: 1120px!important;
        font-weight: 500 !important;
        margin: 0 auto !important;
        padding: 0px 16px;
        display: flex;
        &-info {

        }
        &-img {

        }
    }
}
@media (max-width: 800px) {
    .linux {
        padding: 20px 0px 0px 0px!important;
        h4 {
            text-align: left!important;
        }
        &__content {
            display: block!important;
            &-info {
                button {
                    margin-bottom: 20px;
                    margin-top: 0px;
                }
            }
            &-img {
                text-align: center!important;
            }
            img {
                width: 250px!important;
                margin: 0 auto;
            }
        }
    }
}

</style>