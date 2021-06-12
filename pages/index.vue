<template>
  <section>
    <h1>Добро пожаловать на IT Manager!<br>Здесь Вы можете найти специалиста для Вашего проекта.</h1>
    <div class="navigation-button">
      <nuxt-link class="btn btn-primary" to="/employers">Найти работника</nuxt-link>
      <nuxt-link class="btn btn-primary" to="/applicants">Завести анкету</nuxt-link>
    </div>
  </section>
</template>

<style scoped>
  section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: calc(100vh - 256px);
  }

  @media screen and (max-width: 616px) {
    section {
    height: calc(100vh - 340px);
  }
  }
  
  @media screen and (max-width: 436px) {
    section {
    height: calc(100vh - 412px);
  }
  }

  h1 {
    text-align: center;
  }

  .navigation-button a {
    font-size: 22px;
    padding: 10px 40px;
    margin: 0 10px;
  }

  .navigation-button {
    margin-top: 40px;
  }

  @media screen and (max-width: 767px) {
    
    .navigation-button {
    text-align: center;
  }

    .navigation-button a {
      margin: 10px;
  }
  }
</style>
