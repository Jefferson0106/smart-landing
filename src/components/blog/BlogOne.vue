<script setup>

import { onMounted, ref} from 'vue'

import axios from "axios";

const blogs = ref([]);

onMounted(async () => {
  const { data: fetchedblogs } = await axios.get("/data/blogs.json");
  blogs.value = fetchedblogs.blogs;
});

</script>

<template>
  <div class="single-slide-item">
    <h1 style="color: beige;">FAQ</h1>
    <p class="negro">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
    <p class="negro">Eius dolore laborum labore cum modi nesciunt? Ut aliquam odit pemque repellendus?</p>
    <div class="image-container">
      <img class="nino" src="/assets/img/bot.png" alt="Friendly Robot">
      
      <img class="imagen" src="/assets/img/mensaje.png" alt="Sample Image">
    </div>
  </div>
</template>

<style scoped>
.image-container {
  position: relative;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  max-width: 100%; /* Ensure the container doesn't exceed the page width */
}

.mensaje {
  position: absolute;
  top: 30%;
  left: 60%;
  color: bisque;
  font-size: 24px;
  text-align: center;
  padding: 10px;
  border-radius: 5px;
}

.nino {
  width: 50%;
}

.imagen {
  width: 40%;
}

.negro {
  color: #000;
}
</style>
