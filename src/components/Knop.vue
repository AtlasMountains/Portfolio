<template>
  <a
    class="py-2 font-semibold text-center duration-300 ease-in-out hover:bg-opacity-0 focus:bg-opacity-0"
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
