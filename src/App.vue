<!-- html -->
<template lang="">
    <Card>
        <template v-slot:default="props">
            {{ props.firstName }} {{ props.lastName }}
        </template>
    </Card>
</template>

<!-- code -->
<script>
import Card from "./components/Card.vue";

export default {
    components: {
        Card,
    },
};
</script>
