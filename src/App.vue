<template>
    <div>
        <CreatePost />
        <PostList />
    </div>
</template>

<script>
import CreatePost from "./components/CreatePost.vue";
import PostList from "./components/PostList.vue";

export default {
    components: {
        PostList,
        CreatePost,
    },
};
</script>

<!-- https://jsonplaceholder.typicode.com/posts -->
