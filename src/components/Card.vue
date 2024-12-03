<script setup>

const props = defineProps({
    title: {
        type: String,
        required: true
    },
    author: {
        type: String,
        required: true
    },
    content: {
        type: String,
        required: true
    },
    date: {
        type: String,
        required: true
    }
})



</script>
<template>
    <div class="flex bg-red-300 border flex-col gap-2 tex-black p-10 rounded-3xl">

        <h2>{{ title }}</h2>
        <h3>{{ author }}</h3>


        <p>{{ date }}</p>
        <p>{{ content }}</p>

    </div>

</template>
