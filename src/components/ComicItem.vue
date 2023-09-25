<script>
export default {
    name: 'ComicItem',
    props: {
        image: 'String',
        title: 'String',
        price: 'String',
        type: 'String'
    }
}
</script>

<template>
    
    <div class="col">
        <div class="comic card h-100">
            <img :src="image" alt="">
            <div class="card">
                <h3>{{title}}</h3>
            </div>
        </div>
    </div>

</template>

<style scoped>

</style>