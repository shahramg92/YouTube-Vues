<template>
  <ul>
    {{ videosList.length }}
  </ul>
</template>

<script>
export default {
  name: 'VideoList',
  props: {
    videosList: Array
  }
};
</script>

<style></style>
