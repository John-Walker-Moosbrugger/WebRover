<template>
<div class="container">
    <h2 class="subtitle subtitle__white video__title">This is CubeRover</h2>
    <div class="video-container" :style="{ width: video.width, height: video.height }">
        <iframe class = "video-video"
            src="https://www.youtube.com/embed/kGe57-FPU1I"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen>
        </iframe>
    </div>
</div>
</template>

<script>
export default {
  data () {
    return {
      video: {
        width: 0,
        height: 0
      }
    }
  },
  methods: {
    handleResize () {
      if (window.innerWidth <= 1140) {
        var width = window.innerWidth * 0.8
        var height = width * 9 / 16

        this.video.width = width + 'px'
        this.video.height = height + 'px'
      } else {
        this.video.width = '940px'
        this.video.height = '528.75px'
      }
    }
  },
  beforeMount () {
    window.addEventListener('resize', this.handleResize)
    this.handleResize()
  },
  destroyed () {
    window.removeEventListener('resize', this.handleResize)
  }
}
</script>

<style scoped lang="scss">
.container {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.video-video {
    width: 100%;
    height: 100%;
}

.video__title {
    transform: translateY(2rem);
}
</style>
