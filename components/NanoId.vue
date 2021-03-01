<template>
  <div class="container">
    <div>
      <h1>
        Hello from <span class="name">{{ id }}</span
        >.
      </h1>
    </div>
  </div>
</template>

<script>
import { nanoid } from "nanoid";

export default {
  data() {
    return {
      id: nanoid(8),
    };
  },
};
</script>

<style scoped>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
h1 {
  font-weight: 400;
}
.name {
  color: #00C48D;
}
p {
  margin-top: 20px;
}
</style>
