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
            <div class="comic card border-0 rounded-0 p-2 h-100">
                <h3 class="text-white text-center">{{title}}</h3>
                <span class="fs-5 text-white text-center">{{price}} {{type}}</span>
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>
    
</style>