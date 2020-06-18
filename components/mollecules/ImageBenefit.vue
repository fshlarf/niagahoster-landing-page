<template>
    <div class="col" style="margin-top: 20px; margin-bottom: 20px">
        <img :src="`/images/${fileImg}`" alt="Image not found">
        <h5>{{ title }}</h5>
        <p v-html="desc"></p>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        desc: String,
        fileImg: String
    }
}
</script>

<style lang="scss" scoped>
img {
    margin-bottom: 20px;
    width: 5rem;
}
p {
    font-size: 15px;
}
h5 {
    font-weight: 600!important;
    margin-bottom: 5px;
}
</style>