<template>
  <div id="app">
    <div class="bg"></div>
    <ClientForm />
  </div>
</template>

<script>
import ClientForm from "./components/ClientForm.vue";

export default {
  name: "App",
  components: {
    ClientForm,
  },
};
</script>

<style lang="scss">

@import "./styles/variables.scss";
@import "./styles/reset.scss";

#app {
  position: relative;
  overflow: hidden;
  min-height: 100%;
  display: flex;
  flex-direction: column;
  padding: 0 15px;

  color: $text-color;
  font-family: sans-serif;
}

.bg {
  position:absolute;
  z-index:-1;
  top:0;
  right:0;
  bottom:0;
  left:0;

  background-image: radial-gradient(
      circle at 30% 86%,
      rgba(255, 255, 255, 0.03) 0%,
      rgba(255, 255, 255, 0.03) 8%,
      transparent 8%,
      transparent 92%
    ),
    radial-gradient(
      circle at 55% 100%,
      rgba(255, 255, 255, 0.03) 0%,
      rgba(255, 255, 255, 0.03) 8%,
      transparent 8%,
      transparent 92%
    ),
    radial-gradient(
      circle at 40% 75%,
      rgba(255, 255, 255, 0.03) 0%,
      rgba(255, 255, 255, 0.03) 6%,
      transparent 6%,
      transparent 94%
    ),
    radial-gradient(
      circle at 7% 99%,
      rgba(255, 255, 255, 0.03) 0%,
      rgba(255, 255, 255, 0.03) 6%,
      transparent 6%,
      transparent 94%
    ),
    radial-gradient(
      circle at 69% 76%,
      rgba(255, 255, 255, 0.03) 0%,
      rgba(255, 255, 255, 0.03) 6%,
      transparent 6%,
      transparent 94%
    ),
    radial-gradient(
      circle at 2% 35%,
      rgba(255, 255, 255, 0.03) 0%,
      rgba(255, 255, 255, 0.03) 6%,
      transparent 6%,
      transparent 94%
    ),
    radial-gradient(
      circle at 14% 48%,
      rgba(255, 255, 255, 0.03) 0%,
      rgba(255, 255, 255, 0.03) 6%,
      transparent 6%,
      transparent 94%
    ),
    radial-gradient(
      circle at 28% 87%,
      rgba(255, 255, 255, 0.04) 0%,
      rgba(255, 255, 255, 0.04) 4%,
      transparent 4%,
      transparent 96%
    ),
    radial-gradient(
      circle at 65% 14%,
      rgba(255, 255, 255, 0.04) 0%,
      rgba(255, 255, 255, 0.04) 4%,
      transparent 4%,
      transparent 96%
    ),
    radial-gradient(
      circle at 51% 36%,
      rgba(255, 255, 255, 0.04) 0%,
      rgba(255, 255, 255, 0.04) 4%,
      transparent 4%,
      transparent 96%
    ),
    radial-gradient(
      circle at 6% 93%,
      rgba(255, 255, 255, 0.04) 0%,
      rgba(255, 255, 255, 0.04) 4%,
      transparent 4%,
      transparent 96%
    ),
    linear-gradient(135deg, rgb(24, 196, 208), rgb(29, 24, 208));
}
</style>
