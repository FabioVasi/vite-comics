<script>
export default {
    name: 'Comic'
}
</script>

<template>

    <div class="row row-cols-1 row-cols-sm-3">
        <div class="col" v-for="comic in comics">
            <div class="comic card h-100">
                <img :src="comic.src" alt="">
                <div class="card-body">
                    <h3>{{ comic.name }}</h3>
                </div>
            </div>
        </div>
    </div>
    
</template>

<style>

</style>