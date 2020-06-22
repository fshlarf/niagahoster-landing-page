<template>
    <div>
        <h5>{{ title }}</h5>
        <p v-html="desc"></p>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        desc: String,
    }
}
</script>

<style lang="scss" scoped>
p {
    font-size: 15px;
}
h5 {
    font-weight: 600!important;
    margin-bottom: 5px;
}
</style>