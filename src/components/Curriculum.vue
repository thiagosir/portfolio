<template>
  <div class="container">
    <a href="/CurriculoTester.pdf" download class="download">
      <button class="curriculum">
        <span class="text">Download CV</span>
        <svg width="25px" height="25px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M12 3V16M12 16L16 11.625M12 16L8 11.625" stroke="#1C274C" stroke-width="1.5" stroke-linecap="round"
            stroke-linejoin="round" />
          <path
            d="M15 21H9C6.17157 21 4.75736 21 3.87868 20.1213C3 19.2426 3 17.8284 3 15M21 15C21 17.8284 21 19.2426 20.1213 20.1213C19.8215 20.4211 19.4594 20.6186 19 20.7487"
            stroke="#1C274C" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
        </svg>
      </button>
    </a>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 15.625rem;
  width: 100%;
}

.curriculum {
  display: flex;
  justify-content: center;
  align-items: center;

  cursor: pointer;

  background-color: #6197f4;
  border-style: none;
  border-radius: .3125rem;

  width: 11.25rem;
  height: 3.75rem;
}

.curriculum:hover {
  background-color: #4972b8;
  transition: 0.5s;
}

.text {
  margin-right: .3125rem;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  font-size: 1.125rem;
  text-decoration: none;
  color: black;
}

.download {
  text-decoration: none;
}

</style>