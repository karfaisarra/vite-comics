<script>
export default {
    nome: 'Comic',
    props: {
        image: String,
        title: String
    }
}
</script>
<template>
    <div class="col">
        <img :src="image" alt="title">
        <h5>{{ title }}</h5>
    </div>
</template>
<style lang="scss" scoped>
.col {
    h5 {
        color: white;
    }
}
</style>