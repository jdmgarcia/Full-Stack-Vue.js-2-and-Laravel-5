<template>
  <div class="listing-summary">
    {{ listing.address }}
  </div>
</template>

<script>
export default {
  props: ['listing'],
}
</script>