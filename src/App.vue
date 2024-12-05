<!-- html -->
<template>
    <div>
        <Movie name="JJK" :likes="50" :isPublished="true" />
        <Movie name="Kuroko no basuke" :likes="20" :isPublished="true" />
        <Movie :likes="500" :isPublished="false" />
    </div>
</template>

<!-- code -->
<script>
import Greet from "./components/Greet.vue";
import Movie from "./components/Movie.vue";

export default {
    name: "App",
    components: {
        Greet,
        Movie,
    },
};
</script>
