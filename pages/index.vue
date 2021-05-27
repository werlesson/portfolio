<template>
  <div>
    <section-main />
    <section-about />
    <section-projects />
  </div>
</template>
<script>
import SectionAbout from '~/views/sections/SectionAbout.vue'
import SectionMain from '~/views/sections/SectionMain.vue'
import SectionProjects from '~/views/sections/SectionProjects.vue'
export default {
  components: { SectionAbout, SectionMain, SectionProjects },
  data: () => ({}),
}
</script>
