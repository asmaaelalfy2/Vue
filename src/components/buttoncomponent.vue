<template>
    <button @click="buttonClicked" value="add" >Submit</button>
</template>

<script>


export default {

    data(){
     
     return {
         dummyStd:[
             {name:"asmaa",city:"cairo"},
               {name:"esraa",city:"cairo"},
                 {name:"alaa",city:"cairo"}
         ],
         index:0,
         target:null

     }
    },

    
    methods:{
        buttonClicked(){
            this.target=this.dummyStd[this.index]
            this.index++;
            this.$emit("btnClick",this.target)
        }
    }
}
</script>

