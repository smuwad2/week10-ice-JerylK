<script>
    export default {
        // Add code if/as necessary
        // Hint: Add properties subject, entry and mood
        props: {
            post: Object
        },
        computed: {
            imageLoc() {
                return `/assets/${this.post.mood.toLowerCase()}.png`
            } 
        }

    }
</script>


<template>
    <!-- TODO: add your template code here. Use boostrap card --> 
    <div class="card" style="width: 18rem;">
        <img :src="imageLoc" class="card-img-top" alt="...">
        <div class="card-body">
            <h5 class="card-title">{{ post.subject }}</h5>
            <p class="card-text">{{ post.entry }}</p>
            <slot></slot>
        </div>
    </div>
</template>

