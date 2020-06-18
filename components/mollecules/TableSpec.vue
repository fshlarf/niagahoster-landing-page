<template>
    <div>
        <table v-for="(spec, id) in specification" :key="id">
            <tr :style="[ id == 1 && { 'background-color' : '#ddd' }]">
                <i class="fa fa-check-circle"></i>
                <td>{{ spec }}</td>
                <td></td>
            </tr>
        </table>
    </div>
</template>

<script>
export default {
    props: {
        specification: Array
    }
}
</script>

<style lang="scss" scoped>
table {
    font-family: arial, sans-serif;
    border-collapse: collapse;
    width: 100%;
    border: 1px solid #dddddd;
    max-width: 350px;
    margin: 0 auto;
}
td, th {
    text-align: left;
    padding: 8px;
    text-align: center;
}
tr:nth-child(even) {
    background-color: #dddddd!important;
}
i {
    font-size: 23px!important;
    color: #00b348;
    margin-top: 9px;
    padding: 0px 16px
}
</style>