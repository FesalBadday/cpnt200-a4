<template>
  <footer class="flex justify-center bg-purple-900 text-white p-6 gap-x-1">
    <p>{{ new Date().getFullYear() }}</p>
    <div v-html="`<p>&copy; ${pageInfo.author}</p>`" />
  </footer>
</template>
<script>
export default {
  props: ["pageInfo"],
};
</script>