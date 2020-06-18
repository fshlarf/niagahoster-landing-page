<template>
    <div class="col">
        <img :src="`/images/${fileImg}`" alt="Image not found">
        <h4>{{ title }}</h4>
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
</style>