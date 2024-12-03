<script setup>
import Card from "./components/Card.vue";

const blogs = [
  {
    title: "Exploring the World of AI",
    author: "Alice Johnson",
    date: "2023-05-15",
    content: "Artificial Intelligence is shaping the future in unexpected ways. From self-driving cars to advanced machine learning algorithms, AI is revolutionizing industries. This blog dives into the latest trends and advancements in AI technology, exploring how they can impact everyday life."
  },
  {
    title: "The Importance of Mental Health",
    author: "David Smith",
    date: "2023-07-21",
    content: "In today's fast-paced world, maintaining mental health has become increasingly important. This article explores various strategies for improving mental well-being, including mindfulness practices, exercise, and social connections, all of which contribute to a balanced and healthy lifestyle."
  },
  {
    title: "A Guide to Sustainable Living",
    author: "Emily Green",
    date: "2022-11-03",
    content: "Sustainability is more than just a trend; it's a necessity. This post provides practical tips for adopting an eco-friendly lifestyle, from reducing waste to embracing renewable energy sources. Learn how small changes can lead to a more sustainable and environmentally friendly future."
  }
];



</script>

<template>
  <div class="flex flex-col gap-4 p-4">
    <Card v-for="(blog, index) in blogs" :key="index" :title="blog.title" :author="blog.author" :date="blog.date"
      :content="blog.content" />
  </div>

</template>
