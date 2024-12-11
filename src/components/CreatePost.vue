<template>
    <div>
        <form @submit.prevent="postData">
            <div>
                <label for="userId">userId: </label>
                <input type="text" v-model="formData.userId" />
            </div>
            <div>
                <label for="title">Title: </label>
                <input type="text" v-model="formData.title" />
            </div>
            <div>
                <label for="body">Body: </label>
                <input type="text" v-model="formData.body" />
            </div>

            <button>Post Data</button>
        </form>
    </div>
</template>

<script>
// import axios
import axios from "axios";

export default {
    data() {
        return {
            formData: {
                userId: "",
                title: "",
                body: "",
            },
        };
    },
    methods: {
        postData() {
            axios
                .post(
                    "https://jsonplaceholder.typicode.com/posts",
                    this.formData
                )
                .then((res) => console.log(res))
                .catch((err) => console.log(err));
        },
    },
};
</script>
