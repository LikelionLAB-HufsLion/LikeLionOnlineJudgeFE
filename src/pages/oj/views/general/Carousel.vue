<template>

<div>
  <b-carousel

    id="carousel-fade"
    style="text-shadow: 1px 1px 2px #333;"
    fade
    indicators
    img-width="1024"
    img-height="480"
    interval="2000"
  >
    <b-carousel-slide caption="" img-src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F018d9a4f-197f-459d-b224-eb4787f63e5f%2F1.jpg" />
    <b-carousel-slide caption="Hack Your Life!" img-src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fcaf54475-f897-4c9d-92e5-d21438fa0b5f%2F2.jpg"/>
    <b-carousel-slide caption="" img-src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fd7c685bf-551b-44ac-9cf0-81e17db5e610%2F3.jpg" />

  </b-carousel>
</div>

</template>

<script>
  export default {
    data () {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart (slide) {
        this.sliding = true
      },
      onSlideEnd (slide) {
        this.sliding = false
      }
    }
  }
</script>