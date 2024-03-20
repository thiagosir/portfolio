<script lang="ts">

export default {

}

</script>

<template>
  <div class="body_knowledges">
    <h1 class="header">Conhecimentos</h1>

  </div>
</template>
<style scoped>
.body_knowledges {
  /* margin-top: 55px; */
  height: 2000rem;
  margin-left: 400px;
  width: 60%;
  height: 350px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.header {
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  font-weight: 600;
}

@keyframes slidein {
  from {
    opacity: 0;
    transform: translateX(-50px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slideinBelow {
  from {
    opacity: 0;
    transform: translateY(50px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideinRight {
  from {
    opacity: 0;
    transform: translateX(50px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes fadein {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}
</style>