<template>
  <a
    class="font-bold rounded-lg shadow-lg text-center py-2 hover:bg-opacity-70 ease-in-out duration-300"
    :href="link"
    target="_blank"
  >
    {{ text }}
  </a>
</template>

<script>
export default {
  props: ["text", "link"],
};
</script>
