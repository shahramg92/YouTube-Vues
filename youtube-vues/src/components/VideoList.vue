<template>
  <ul>
    <VideoListItem v-for="video in videosList">
    </VideoListItem>
  </ul>
</template>

<script>
import VideoListItem from './VideoListItem';

export default {
  name: 'VideoList',
  components: {
    VideoListItem
  },
  props: {
    videosList: Array
  }
};
</script>

<style></style>
