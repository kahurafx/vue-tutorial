<template>
    <div>
        <button @click="getPosts">Load Posts</button>

        <ul v-for="post in posts" :key="post.id">
            <li>
                {{ post.title }}
            </li>
        </ul>
    </div>
</template>

<script>
// import axios
import axios from "axios";

export default {
    data() {
        return {
            posts: [],
        };
    },
    methods: {
        getPosts() {
            axios
                .get("https://jsonplaceholder.typicode.com/posts")
                .then((res) => (this.posts = res.data))
                .catch((err) => console.log(err));
        },
    },
};
</script>
