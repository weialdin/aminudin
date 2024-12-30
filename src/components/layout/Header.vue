<template>
  <div class="dizme_tm_header">
    <div class="container">
      <div class="inner">
        <div class="logo">
          <a href="#"
            ><img :src="`img/logo/${dark ? 'dark' : 'logo'}.png`" alt=""
          /></a>
        </div>
        <div class="menu">
          <ul class="anchor_nav">
            <li class="current"><a href="#home">Home</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li class="download_cv">
              <a href="https://wa.link/lhr7pl"><span>Hire Me</span></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderVue",
  props: {
    dark: { type: Boolean },
  },
};
</script>
