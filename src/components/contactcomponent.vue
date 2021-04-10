<template>
    <div>
        <h3>Contact</h3>
        <p>{{counter}}</p>
        <button class="btn btn-primary" @click="increaseCounter">Add</button>
    </div>
</template>

<script>
export default {
    data(){
       return{
counter:0,
       } 
    },
    methods:{
        increaseCounter(){
            this.counter++;
        }
    }
}
</script>

<style scoped>

</style>