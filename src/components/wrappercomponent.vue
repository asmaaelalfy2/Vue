<template>
<div>
    <headercomponent  branch=" iti mansoura">
        <template v-slot:top>  <h1> Hello OWLD</h1></template>
      <template v-slot:bottom>  <h1> Hello OWLD</h1></template>
    </headercomponent>
    <buttoncomponent @btnClick="added('asmaa')" />

    <p v-for="std in student" v-bind:key="std.id">{{std.id}}</p>
</div>
</template>

<script>
import headercomponent from './headercomponent.vue'
import buttoncomponent from './buttoncomponent.vue'
export default {

    data(){
return{
    student:[
        {
            "id":1,
            "name":"ahmed",
            "age":12
        },
          {
            "id":2,
            "name":"lied",
            "age":13
        }
    ]
}},

 
     components:{
        headercomponent,
    buttoncomponent
    },
    methods:{
added(data){
    this.student.push({name:data.name,city:data.city})
}
    }
}
</script>
