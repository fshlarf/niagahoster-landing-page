<template>
    <div class="footer">
        <div class="container">
            <div class="footer__row">
                <div class="coloum">
                    <h5>HUBUNGI KAMI</h5>
                    <ListInfo
                        :arrayModule="dataCompany1"
                    />
                    <br>
                    <ListInfo
                        :arrayModule="dataCompany2"
                    />
                </div>
                <div class="coloum">
                    <h5>LAYANAN</h5>
                    <ListInfo
                        :arrayModule="services"
                    />
                </div>
                <div class="coloum">
                    <h5>SERVIS HOSTING</h5>
                    <ListInfo
                        :arrayModule="serviceHosting"
                    />
                </div>
                <div class="coloum">
                    <h5>TUTORIAL</h5>
                    <ListInfo
                        :arrayModule="tutorial"
                    />
                </div>
            </div>
            <div class="footer__row">
                <div class="coloum">
                    <h5>TENTANG KAMI</h5>
                    <ListInfo
                        :arrayModule="aboutUs"
                    />
                </div>
                <div class="coloum">
                    <h5>KENAPA PILIH NIAGAHOSTER?</h5>
                    <ListInfo
                        :arrayModule="reasons"
                    />
                </div>
                <div class="footer__newsletter coloum">
                    <h5>NEWSLETTER</h5>
                    <div class="footer__newsletter-content">
                        <input placeholder="Email"/>
                        <button type="button" class="btn btn-primary">Berlangganan</button>
                    </div>
                    <p class="footer__newsletter-text">Dapatkan promo dan konten menarik <br>dari penyedia hosting terbaik Anda.</p>
                </div>
                <div class="footer__credentials coloum">
                    <i class="fa fa-facebook fb"></i>  
                    <i class="fa fa-twitter tw"></i>  
                    <i class="fa fa-google-plus gp"></i>  
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import ListModule from '../mollecules/ListModule'
export default {
    components: {
        ListInfo: ListModule
    },
    data() {
        return {
            dataCompany1: ['0274-5305505', 'Senin - Minggu', '24 Jam Nonstop'],
            dataCompany2: ['Jl. Selokan Mataram Monjali', 'Karangjati MT I/304', 'Sinduadi, Mlati, Sleman', 'Yogyakarta 55284'],
            services: ['Domain', 'Shared Hosting', 'Cloud VPS Hosting', 'Managed VPS Hosting', 'Web Builder', 'Keamanan SSL/HTTPS', 'Jasa Pembuatan Website', 'Program Affiliasi'],
            serviceHosting: ['Hosting Murah', 'Hosting Indonesia', 'Hosting Singapura SG', 'Hosting PHP', 'Hosting Wordpress', 'Hosting Laravel'],
            tutorial: ['Knowledgebase', 'Blog', 'Cara Pembayaran'],
            aboutUs: ['Tim Niagahoster', 'Karir', 'Events', 'Penawaran & Promo Spesial', 'Kontak'],
            reasons: ['Support Terbaik', 'Garansi Harga Termurah', 'Domain Gratis Selamanya', 'Datacenter Hosting Terbaik', 'Review Pelanggan']
        }
    }
}
</script>

<style lang="scss" scoped>
.footer {
    padding: 60px 0px 30px 0px;
    background-color: #303030;
    color: white!important;
    font-size: 14px!important;
    h5 {
        padding: 16px!important;
        margin-bottom: 16px;
        font-size: 16px;
    }
    .container {
        max-width: 1120px!important;
        margin: 0 auto !important;
    }
    .col-1 {
        width: 200%;
    }
    &__row {
        display: flex;
        margin-bottom: 70px;
    }
    &__newsletter {
        h5 {
            margin-left: -10px;
        }
        &-content {
            background-color: white;
            padding: 5px 4px;
            width: fit-content;
            border-radius: 25px;
            margin-bottom: 10px;
            button {
                padding: 10px 10px;
            }
            input {
                background-color: transparent!important;
                border: none!important;
                width: 100px!important;
                padding: 0px 16px!important;
            }
        }
        p {
            font-size: 13px;
        }
    }
    &__credentials {
        display: flex;
        height: max-content;
        margin-left: 20px;
        i {
            border: 1px solid white;
            border-radius: 50px;
            font-size: 26px;
            margin: 72px 10px;
        }
        .fb {
            padding: 18px 23px;
        }
        .tw {
            padding: 18px;
        }
        .gp {
            padding: 18px 14px;
        }
    }
    .coloum {
        width: 30%;
        text-align: left;
    }
}
</style>