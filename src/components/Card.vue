<!-- html -->
<template lang="">
    <h2 v-for="(name, index) in names" :key="index">
        <slot :firstName="name.firstName" :lastName="name.lastName"></slot>
    </h2>
</template>

<!-- code -->
<script>
export default {
    data() {
        return {
            names: [
                {
                    firstName: "Clark",
                    lastName: "Kent",
                },
                {
                    firstName: "Bruce",
                    lastName: "Wayne",
                },
                {
                    firstName: "Princess",
                    lastName: "Diana",
                },
            ],
        };
    },
};
</script>
