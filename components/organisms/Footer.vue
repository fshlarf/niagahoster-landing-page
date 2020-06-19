<template>
    <div class="footer">
        <div class="container">
            <div class="footer__row">
                <div>
                    <h5>HUBUNGI KAMI</h5>
                    <ListInfo
                        :arrayModule="dataCompany1"
                    />
                    <br>
                    <ListInfo
                        :arrayModule="dataCompany2"
                    />
                </div>
                <div>
                    <h5>LAYANAN</h5>
                    <ListInfo
                        :arrayModule="services"
                    />
                </div>
                <div>
                    <h5>SERVIS HOSTING</h5>
                    <ListInfo
                        :arrayModule="serviceHosting"
                    />
                </div>
                <div>
                    <h5>TUTORIAL</h5>
                    <ListInfo
                        :arrayModule="tutorial"
                    />
                </div>
            </div>
            <div class="footer__row">
                <div>
                    <h5>TENTANG KAMI</h5>
                    <ListInfo
                        :arrayModule="aboutUs"
                    />
                </div>
                <div>
                    <h5>KENAPA PILIH NIAGAHOSTER?</h5>
                    <ListInfo
                        :arrayModule="aboutUs"
                    />
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
            aboutUs: ['Tim Niagahoster', 'Karir', 'Events', 'Penawaran & Promo Spesial', 'Kontak']
        }
    }
}
</script>

<style lang="scss" scoped>
.footer {
    padding: 60px 0px 30px 0px;
    background-color: #303030;
    color: white!important;
    h5 {
        padding: 16px!important;
        margin-bottom: 16px;
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
}
</style>