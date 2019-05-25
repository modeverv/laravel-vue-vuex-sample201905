<template>
    <div>
        <h1>Photo Detail</h1>
        <img :src="ssrc"/>
    </div>
</template>

<script>

export default {
  props: {
    id: null
  },
  computed: {
    ssrc() {
      return `https://s3-ap-northeast-1.amazonaws.com/vuesplash-lovesaemi/${this.id}.jpeg`
    },
  }
};
</script>
