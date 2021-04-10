<template>
    
    <div class="container"><ul>
        <li><a href="" @click.prevent="targetcomponent='homecomponent'">Home</a></li>
        <li><a href="" @click.prevent="targetcomponent='aboutcomponent'">About</a></li>
        <li><a href="" @click.prevent="targetcomponent='contactcomponent'">Contact</a></li>
    </ul>
        <div class="row">
            <keep-alive>
        <component :is="targetcomponent" />
            </keep-alive>
    </div>

    </div>

</template>

<script>
import aboutcomponent from './aboutcomponent';
import homecomponent from './homecomponent';
import contactcomponent from './contactcomponent'
export default {
    data(){
        return{
            targetcomponent:'homecomponent'
        }
    },
    components:{
        aboutcomponent,
        homecomponent,
        contactcomponent
    }
}
</script>

<style scoped>

</style>