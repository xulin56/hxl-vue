<template lang="html">
    <div class="demo">
        <h1>count:{{this.$store.state.count}}</h1>
        <h1>count:{{getCount}}</h1>
        <button @click="add">点击加加</button>
    </div>
</template>

<script>
export default {
    computed:{
        getCount(){
            return this.$store.state.count
        }
    },
    methods: {
        add(){
            let v = 100;
            this.$store.commit('countAdd',v)
        }
    }
}
</script>

<style lang="css" scoped>
</style>
