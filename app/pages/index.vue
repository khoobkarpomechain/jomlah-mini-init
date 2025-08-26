<script setup lang="ts">
const count = ref(0);
</script>

<template>
  <div class="container">
    <div class="card">
      <h1>Index page</h1>
      <p>
        Welcome to your Nuxt 3 app. Build to test and showcase telegram bot.
      </p>
      <div class="changelog">
        <p>
          <strong>Change log:</strong>
        </p>
        <p>- Add Mini app base config</p>
      </div>
      <button @click="count++">Count is: {{ count }}</button>
    </div>
  </div>
</template>

<style>
.container {
  width: 100dvw;
  height: 100dvh;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  padding: 1rem;
}

.card {
  width: 100dvw;
  max-width: 420px;
  height: auto;
  background-color: oklch(0.1766 0.028 261.692);
  border: 1px solid oklch(27.9% 0.041 260.031);
  border-radius: 1rem;
  padding: 1rem;
}

.card h1 {
  font-size: 1.25rem;
}

.card > p {
  font-size: 1rem;
  line-height: 1.5;
  margin-bottom: 1rem;
}

.card button {
  width: 100%;
  font-size: 1rem;
  padding: 0.9rem;
  border-radius: 0.5rem;
  background-color: oklch(76.9% 0.188 70.08);
  color: oklch(12.9% 0.042 264.695);
  border: 0px;
  cursor: pointer;
  font-weight: 600;
  transition: color 0.3s ease, background-color 0.3s ease;
}

.card button:hover {
  background-color: oklch(66.6% 0.179 58.318);
}

.card button:active {
  background-color: oklch(55.5% 0.163 48.998);
}

.changelog {
  background-color: oklch(13% 0.028 261.692 / 30%);
  border: 1px solid oklch(13% 0.028 261.692);
  border-radius: 1rem;
  padding: 0.5rem;
  margin-bottom: 2rem;
}
</style>
