<script>
    // TODO: Complete the code
    export default { 
        data() {
            return {
                
            }
        },
        // Hint: insert properties task (Object) and idx (Number)
        props:{
            task: Object,
            idx: Number
        },
        emits:[
            'removeTask'
        ]
    }
</script>

<template>
    <!-- TODO: add your template code here --> 
    <div class="card" style="width: 18rem; display: inline-block;">
        <div class="card-body">
            <div class="card-title">Deadline: {{ task.deadline }}</div>
            <hr></hr>
            <div class="card-text">{{ task.desc }}</div>
            <button class="btn btn-primary" @click="$emit('removeTask', idx)">Done</button>
        </div>
    </div>
</template>


