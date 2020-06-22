<template>
    <div class="spec">
        <h4>Powerful dengan Limit PHP yang Lebih Besar</h4>
        <div class="row spec__content">
            <div class="col"> 
                <TableSpec
                    :specification="specificationOne"
                />
            </div>
            <div class="col"> 
                <TableSpec
                    :specification="specificationTwo"
                />
            </div>
        </div>
        <MiniCenteredLine/>
    </div>
</template>

<script>
import TableSpec from '../mollecules/TableSpec'
import MiniCenteredLine from '~/components/atoms/MiniCenteredLine'
export default {
    components: {
        TableSpec,
        MiniCenteredLine
    },
    data() {
        return {
            specificationOne: [
                'max execution time 300s',
                'max execution time 300s',
                'PHP memory limit 1024 MB'
            ],
            specificationTwo: [
                'post max size 128 MB',
                'upload max filesize 128 MB',
                'max input vars 2500'
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.spec {
    max-width: 700px!important;
    margin: 0 auto !important;
    &__content {
        margin-bottom: 45px;
    }
}
@media (max-width: 800px) { 
    .spec__content {
        display: block;
    }
    .col {
        margin: 20px 0px;
    }
}
</style>