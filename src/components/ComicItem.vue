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
    
    <div class="col g-4">
        <div class="comic card border-0 rounded-0 h-100">
            <img :src="image" alt="">
            <div class="card border-0 pt-2 pb-2">
                <h3>{{title}}</h3>
                <span class="fs-5">{{price}} {{type}}</span>
            </div>
        </div>
    </div>

</template>

<style scoped>

</style>