<template>
  <div class="grid place-items-center h-screen bg-gradient-to-r from-pink-300 via-purple-300 to-indigo-400">
    <h1 class="text-4xl font-bold text-white">
      I am rendered on the <strong class="underline decoration-indigo-500">{{ renderedOn }}</strong> side
    </h1>
  </div>
</template>

<script>
export default {
  data() {
    return { renderedOn: process.client ? "Client" : "Server" };
  },
};
</script>
