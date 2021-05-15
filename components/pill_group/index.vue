<template>
  <div class="pill_group mt-16">
    <div v-for="item in items" :key="item.id" class="a-pill">
      {{ item.value }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'PillGroup',
  props: {
    items: {
      type: Array,
      required: true,
    },
  },
}
</script>

<style scoped>
.a-pill {
  padding: 4px 12px;
  font-size: var(--body02);
  line-height: var(--lhBody02);
  font-family: roboto400;
  background-color: var(--black06);
  color: var(--black02);
  border-radius: var(--bigRadius);
  display: inline-block;
  margin-right: 8px;
  margin-bottom: 12px;
}
</style>
