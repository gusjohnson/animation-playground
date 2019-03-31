<template>
  <div>
    <b-tabs class="nav-tabs nav-justified" pills>
      <b-tab title="Animation 1">
        <animation-1 />
      </b-tab>
      <b-tab title="Animation 2">
        <animation-2 />
      </b-tab>
    </b-tabs>
  </div>
</template>

<script>
import Animation1 from '@/components/Animation1'
import Animation2 from '@/components/Animation2'

export default {
  name: 'NavBar',
  components: {
    Animation1,
    Animation2
  }
}
</script>