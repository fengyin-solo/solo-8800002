<script setup>
defineProps({
  items: {
    type: Array,
    required: true,
  },
})
</script>

<template>
  <div class="environment-grid">
    <article
      v-for="item in items"
      :key="item.label"
      class="environment-card"
    >
      <span>{{ item.label }}</span>
      <strong>{{ item.value }}</strong>
      <p>{{ item.note }}</p>
    </article>
  </div>
</template>

<style scoped>
.environment-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 14px;
}

.environment-card {
  padding: 18px;
  border-radius: 18px;
  background: #fbf5ea;
  border: 1px dashed rgba(121, 88, 47, 0.22);
}

span,
strong,
p {
  display: block;
  margin: 0;
}

span {
  font-size: 0.82rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

strong {
  margin-top: 12px;
  font-size: 2rem;
}

p {
  margin-top: 8px;
  color: #6a5439;
}

@media (max-width: 960px) {
  .environment-grid {
    grid-template-columns: 1fr;
  }
}
</style>
