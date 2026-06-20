<script setup>
defineProps({
  hero: {
    type: Object,
    required: true,
  },
})
</script>

<template>
  <section class="hero-banner">
    <div>
      <p class="eyebrow">Conservation Workflow</p>
      <h3>{{ hero.title }}</h3>
      <p class="description">{{ hero.description }}</p>
    </div>
    <div class="hero-highlight">
      <span>{{ hero.backlogLabel }}</span>
      <strong>{{ hero.backlogValue }}</strong>
      <p>{{ hero.note }}</p>
    </div>
  </section>
</template>

<style scoped>
.hero-banner {
  display: grid;
  grid-template-columns: 1.4fr 0.8fr;
  gap: 20px;
  margin-bottom: 24px;
}

.hero-banner > div {
  border-radius: 26px;
  padding: 26px;
  border: 1px solid rgba(79, 57, 32, 0.12);
  background: rgba(255, 250, 242, 0.88);
}

.eyebrow {
  margin: 0 0 12px;
  text-transform: uppercase;
  letter-spacing: 0.22em;
  font-size: 0.78rem;
  color: #82684b;
}

h3 {
  margin: 0;
  font-size: clamp(1.7rem, 3vw, 2.7rem);
  line-height: 1;
}

.description {
  margin: 14px 0 0;
  color: #5f4c33;
}

.hero-highlight {
  background: linear-gradient(180deg, rgba(121, 88, 47, 0.96), rgba(88, 61, 29, 0.96));
  color: #fff8eb;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
}

.hero-highlight span {
  font-size: 0.82rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

.hero-highlight strong {
  margin: 12px 0 8px;
  font-size: 3rem;
  line-height: 1;
}

.hero-highlight p {
  margin: 0;
  color: rgba(255, 248, 235, 0.82);
}

@media (max-width: 900px) {
  .hero-banner {
    grid-template-columns: 1fr;
  }
}
</style>
