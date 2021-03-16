<template>
    <div class="space-y-4 font-sans text-center">
        <h1 class="text-5xl font-bold">{{ msg }}</h1>

        <div class="flex divide-x-2 divide-green-100">
            <a
                class="px-2 text-green-600 hover:underline"
                href="https://vitejs.dev/guide/features.html"
                target="_blank"
                >Vite Documentation</a
            >
            <a
                class="px-2 text-green-600 hover:underline"
                href="https://v3.vuejs.org/"
                target="_blank"
                >Vue 3 Documentation</a
            >
            <a
                class="px-2 text-green-600 hover:underline"
                href="https://tailwindcss.com/docs"
                target="_blank"
                >TailwindCSS Documentation</a
            >
            <a
                class="px-2 text-green-600 hover:underline"
                href="https://github.com/tailwindlabs/tailwindcss-jit"
                target="_blank"
                >TailwindCSS JIT Documentation</a
            >
        </div>

        <button
            class="px-2 py-1 border-2 border-green-600 rounded"
            @click="state.count++"
        >
            count is: {{ state.count }}
        </button>
        <p>
            Edit
            <code>components/HelloWorld.vue</code> to test hot module
            replacement.
        </p>
    </div>
</template>

<script setup>
import { defineProps, reactive } from "vue";

defineProps({
    msg: String,
});

const state = reactive({ count: 0 });
</script>
