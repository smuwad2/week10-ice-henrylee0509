<script>
//import component
import SoundIcon from './subcomponents/SoundIcon.vue'
export default {
    data() {
        return {
            soundLevel: 0
        }
    },
    components: {
        SoundIcon
    }
}
</script>

<template>

    Sound level
    <input type="number" min="0" max="3" v-model="soundLevel">
    <!-- TODO: Add Code Here to make use of the component -->
    <!-- bind level attribute from SoundIcon component to soundLevel (number)
    update / change icon according to soundLevel (increase / decrease based on input)
    NOTE: Need to use v-bind if we want to update according to dynamic value 
    for static values can stick to normal binding e.g level = 2 -->
    <SoundIcon v-bind:level="soundLevel" />

</template>