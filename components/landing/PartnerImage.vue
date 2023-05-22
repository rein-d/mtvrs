<template>
  <div>
    <a href="https://t.me/rusmetaverse" class="landing-block-card-logo-link" target="_self">
      <img :src="require(`~/assets/img/partner/${img}`)" class="sm:w-1/2 lg:w-72 mx-auto" alt="">
    </a>
  </div>
</template>
<script>
export default {
  props: {
    img: {
      type: String,
      default: '',
    },
  },
}
</script>
