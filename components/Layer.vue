<template>
  <div class="grid place-items-center h-screen">
    <h1 class="text-4xl font-bold">
      I am rendered on the <strong>{{ renderedOn }}</strong> side
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
