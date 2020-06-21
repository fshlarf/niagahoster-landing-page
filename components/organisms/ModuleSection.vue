<template>
    <div class="module">
        <h4>Modul Lengkap untuk Menjalankan Aplikasi PHP Anda</h4>
        <div class="module__content">
            <div class="row">
                <div class="row__element">
                    <ListModule
                        :arrayModule="dataColoum1"
                    />
                    <ListModule
                        :arrayModule="dataColoum2"
                    />
                </div>
                <div class="row__element">
                    <ListModule
                        :arrayModule="dataColoum3"
                    />
                    <ListModule
                        :arrayModule="dataColoum4"
                    />
                </div>
            </div>
        </div>
        <div class="module__btn">
            <button type="button" class="btn btn-secondary">Selengkapnya</button>
        </div>
    </div>
</template>

<script>
import ListModule from '../mollecules/ListModule'
export default {
    components: {
        ListModule
    },
    data() {
        return {
            dataColoum1: ['IcePHP', 'apc', 'apcu', 'apm', 'ares', 'bcmath', 'bcompiler', 'big_int', 'bitset', 'bloomy', 'bz2_filter', 'clamav', 'coin_acceptor', 'crack', 'dba'],
            dataColoum2: ['http', 'huffman', 'idn', 'igbinary', 'imagick', 'imap', 'inclued', 'inotify', 'interbase', 'intl', 'incube_loader', 'incube_loader_4', 'jsmin', 'json', 'Idap'],
            dataColoum3: ['nd_pdo_mysql', 'oauth', 'oci8', 'odbcopache', 'pdf', 'pdo', 'pdo_dlib', 'pdo_firebird', 'pdo_mysql', 'pdl_sqlite', 'pdo_odbc' ,'pdo_pqsql', 'pdo_sqlite', 'pqsql', 'phalcon'],
            dataColoum4: ['stat', 'stem', 'stomp', 'suhosin', 'sybase_ct', 'sysvmsg', 'sysvsem', 'sysvshm', 'tidy', 'timezonedb', 'trader' ,'transit', 'uploadProgress', 'uri_template', 'uuid']
        }
    }
}
</script>

<style lang="scss" scoped>
.module {
    max-width: 1000px!important;
    padding: 40px 16px!important;
    margin: 0 auto !important;
    &__content {
        display: flex;
    }
    .col {
        margin-left: 4rem;
    }
    td {
        font-weight: 300!important;
    }
    &__btn {
        margin-top: 40px;
        text-align: center;
    }
    .row {
        &__element {
            display: flex;
        }
    }
}
@media (max-width: 350px) {
    .row {
        display: block!important;
    }
    .row__element {
        margin-bottom: 20px!important;
    }
    .col {
        margin-left: 0px!important;
    }
}
@media (max-width: 800px) {
    .row {
        display: block!important;
    }
    .row__element {
        margin-bottom: 20px!important;
    }
    .col {
        margin-left: 0px!important;
    }
}
</style>