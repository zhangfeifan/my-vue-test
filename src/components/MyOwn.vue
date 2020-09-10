<template>
<v-container class="text-center" id="my-app">
    <v-btn dark elevation="24" color="deep-purple" @click="myfunc">戳我</v-btn>
    <v-card elevation="24" class="pt-0 mt-7" color="pink">
        <v-card-text>{{ message }}</v-card-text>
    </v-card>
</v-container>
</template>

<script>
export default {
    name: "MyOwn",
    data: () => ({
        loading: false,
        selection: 1,
        message: "啥几把玩意"
    }),
    methods: {
        myfunc() {
            this.message = "就是这个几把玩意！"
        },
    },
};
</script>
