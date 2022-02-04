<template>
  <div>
    <c-header />
    <hero-1 />

      <hero-9 />
    <blog />
    <features-1 />
  </div>
</template>

<script>
import Blog from '~/components/blog.vue'
import cHeader from '~/components/cHeader.vue'
import Features1 from '~/components/features1.vue'

import Hero1 from '~/components/hero1.vue'
import Hero9 from '~/components/hero9.vue'
export default {
  components: { cHeader,  Hero1, Features1, Hero9, Blog },
  name: 'IndexPage'
}
</script>
