<template>
  <a
    class="font-semibold text-center py-2 hover:bg-opacity-0 focus:bg-opacity-0 ease-in-out duration-300"
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
