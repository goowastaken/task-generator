<template lang="">
<div id='head'>
    <h1>
        {{title}} 
    </h1>
    <Button title='Add task' />
</div>
    
<div id='sub'>
    <h2>{{subtitle}}</h2>
    
</div> 

   
</template>

<script>
import Button from './Button.vue'

export default {
    name: 'Header',
    props:{

        title: {
            type: String,
            default: "Task Generator 20XX"
        },
        subtitle: {
            type: String,
            default: "hello nice"
        }
    },
    components:{
        Button
    }
    
}
</script>


<style scoped>
   #head{
        display: flex;
        justify-content: space-between;
        align-items:center;
        margin-bottom: 10px;
    }
    /* #sub{
        justify-content: center;
        align-items: center;
        display: flex;
    }
    #butter{
        justify-content: center;
        align-items: center;
        display: flex;
    } */
</style>