<template>
  <div class="lx">
        <div class="container">
            <h4>Linux Hosting yang Stabil<br>dengan Teknologi LVE</h4>
            <div class="row">
                <div class="col">
                    <div class="lx__content">
                        <p>
                            Super Micro <b>Intel Xeon 24-Cores</b> server dengan RAM <b>128 GB</b> dan<br>
                            teknologi <b>LVE CloudLinux</b> untuk stabilitas server Anda. Dilengkapi<br>
                            dengan <b>SSD</b> untuk kecepatan <b>MySQL</b> dan caching. Apache load balancer<br>
                            berbasis LiteSpeed Technologies, <b>CageFS</b> security, <b>Raid-10</b> protection<br>
                            dan auto backup untuk keamanan website PHP Anda.
                        </p>
                    </div>
                    <button type="button" class="lx__btn btn btn-primary">Pilih Hoting Anda</button>
                </div>
                <img src="/images/image_support.png">
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
.lx {
    h4 {
        text-align: left!important;
    }
    padding: 40px 0px 0px 0px!important;
    .container {
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
    img {
        margin-top: -40px;
        width: 24rem;
    }
    .row {
        padding: 0px 8px !important;
        display: flex;
    }
    &__btn {
        margin-top: 16px;
    }
}
@media (max-width: 800) {
    img {
        max-width: 180px!important;
        margin: 0 auto;
    }
}
</style>