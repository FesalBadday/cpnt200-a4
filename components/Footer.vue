<template>
  <footer class="grid justify-items-center bg-purple-900 text-white p-6">
    <p>&copy; {{ pageInfo.author }}</p>
  </footer>
</template>
<script>
export default {
  props: ['pageInfo']
}
</script>