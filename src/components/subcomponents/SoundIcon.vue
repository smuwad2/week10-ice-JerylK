<script>
    export default { 
        data() {
            return {
                soundEmojis: ['🔇', '🔈', '🔉', '🔊']
            }
        },
        // TODO: add code to define a necessary prop
        props: {
            volume: Int16Array
        }
    }
</script>

<template>
    <!-- TODO: add your template code here. Use span element. --> 
    <span>{{ soundEmojis[volume] }}</span>
</template>