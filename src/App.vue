<script>
export default {
    name: "App",
    data() {
        return {
            name: "BATMAN",
            html: "<b>CROSS</b>",
            isDisabled: true,
            count: 0,
            status: danger,
        };
    },
};
</script>

<template>
    <div class="bg-red-600">I am {{ name }}</div>
    <div v-html="html"></div>
    <button :disabled="isDisabled">Hello</button>
    <button @click="count++">Count : {{ count }}</button>
    <ul class="status">
        underlined
    </ul>

    <h2 :class="status">Status</h2>
</template>

<style>
.underline {
    text-decoration: underline;
}

.status {
    text-decoration: double;
}
</style>
