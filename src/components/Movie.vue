<template lang="">
    <div>{{ name }}</div>
    <div>{{ likes }}</div>
    <div>{{ isPublished }}</div>
</template>
<script>
export default {
    name: "Movie",
    props: {
        name: {
            type: String,
            required: true,
            default: "default string",
        },
        likes: Number,
        isPublished: Boolean,
    },
};
</script>
