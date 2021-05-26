<template>
  <div class="center example-nav">
    <vs-navbar
      v-model="active"
      target-scroll="#padding-scroll-content"
      padding-scroll
      center-collapsed
      square
    >
      <template #left> LOGO </template>
      <vs-navbar-item id="guide" :active="active == 'guide'">
        Início
      </vs-navbar-item>
      <vs-navbar-item id="docs" :active="active == 'docs'">
        Sobre
      </vs-navbar-item>
      <vs-navbar-item id="components" :active="active == 'components'">
        Projetos
      </vs-navbar-item>
      <template #right>
        <vs-button>Contate-me</vs-button>
      </template>
    </vs-navbar>
    <div id="padding-scroll-content" class="square">
      <Nuxt />
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    active: 'guide',
  }),
}
</script>
<style scoped>
.square {
  max-height: 100vh;
  width: 100%;
  position: relative;
  overflow: auto;
  padding-top: 7rem;
}
.example-nav {
  background: #f0f0f0 !important;
  padding: 0 !important;
  position: relative;
  overflow: hidden;
}
.center {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 20px;
  flex-wrap: wrap;
}
</style>
