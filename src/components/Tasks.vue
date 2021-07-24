<template lang="">
    <div v-for="task in tasks" :key="task.id">
        <Task @task-delete="$emit('task-delete', task.id)" :task="task"/>
    </div>
</template>
<script>
import Task from './Task.vue'

export default {
    name: 'Tasks',
    props:{
        tasks:Array
    },
    components:{
        Task
    },
    emits:['task-delete']
}
</script>
<style lang="">
    
</style>