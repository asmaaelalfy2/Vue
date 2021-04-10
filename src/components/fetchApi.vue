<template>
    <div class="container">
        <div class="row">
            <button  @click="loaddata" class="btn btn-primary"> get Data</button>
        </div>
        <div class="row">
            <p v-for="post in allposts" :key="post.id">{{post.title}}</p>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
allposts:[]
        }
    },
    methods:{
      async  loaddata(){
         
         let allpostsdefault =await fetch("https://jsonplaceholder.typicode.com/posts");
        let postjson=await allpostsdefault.json();
        this.allposts=postjson;
        
        }

    }
}
</script>

<style scoped>

</style>