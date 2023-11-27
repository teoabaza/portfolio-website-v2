<template>
  <div class="not-found-page">
    <img src="@/assets/images/not-found.gif" class="not-found-img"/>
    <button id="back-btn" @click="goBack">Go Back</button>
  </div>
</template>

<script setup>

function goBack(){
  window.history.back();
}

</script>

<style scoped>
.not-found-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.not-found-img {
  max-width: 60vw;
}
#back-btn {
  background-color: transparent;
  color: #E1E1E1;
  border: 2px solid #E1E1E1;
  font-family: 'Urbanist', Arial, Helvetica, sans-serif;
  font-size: 1rem;
  font-weight: 600;
  border-radius: 10px;
  padding: 1rem 2rem;
  margin: 2rem 0;
  box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
  cursor: pointer;
  transition: transform 0.2s ease-in-out;
}
#back-btn:hover {
  transform: translateY(-5px);
}
</style>
