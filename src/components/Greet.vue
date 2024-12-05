<!-- html -->
<template>
    <div>Wagwan {{ name }} aka {{ hero }}</div>
</template>

<!-- code -->
<script>
export default {
    name: "Greet",
    props: ["name", "hero"],
};
</script>
