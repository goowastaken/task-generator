<template lang="">
        <button v-on:click="update()" id='butt' class='btn'>
            {{title}}
        </button>
</template>
<script>
export default {
    name:'Button',
    props:{
        title:String
    },
    methods:{
        update(){
            console.log("Button pressed");
        }
    }
}
</script>
