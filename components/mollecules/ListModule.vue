<template>
    <div class="col">
        <table>
            <div v-for="(item, id) in arrayModule" :key="id">
                <td>{{ item }}</td>
            </div>
        </table>
    </div>
</template>

<script>
export default {
    props: {
        arrayModule: Array
    }
}
</script>

<style lang="scss" scoped>
td {
    font-weight: 300!important;
}
</style>