<script>
    export default {
        // Add code if/as necessary
        // Hint: Add properties subject, entry and mood
        props:{
            subject: String,
            entry: String,
            mood: String
        },
        computed:{
            imgLoc(){
                return `/assets/${this.mood.toLowerCase()}.png`
            }
        }
    }
</script>


<template>
    <!-- TODO: add your template code here. Use boostrap card --> 
    <div>
        <div class="card mb-3" style="width: 18rem;">
            <img :src="imgLoc" class="card-img-top" ></img>
            <div>
                <div class="card-title">{{ subject }}</div>
                <div class="card-text">{{ entry }}</div>
            </div>
        </div>
    </div>
</template>