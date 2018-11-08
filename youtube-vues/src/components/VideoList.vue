<template>
  <ul class="list-group col-md-4">
    <VideoListItem
      v-for="singleVideo in videosList"
      :video="singleVideo"
      :key="singleVideo.etag"
      @videoSelect="onVideoSelected"
    >
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
  },
  methods: {
    onVideoSelected(video) {
      this.$emit('videoChosen', video);
    }
  }
};
</script>

<style></style>
