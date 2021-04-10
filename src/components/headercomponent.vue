<template>

<div>
<slot name="bottom"> </slot>
    <p> {{branch}} </p>
<slot name="top"> </slot></div>

</template>

<script>
export default {
    data(){

    },

    props:["branch"]
}
</script>

<style scoped>

</style>