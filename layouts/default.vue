<template>
  <div class="bodys">
    <Navbar />
    <main>
      <div class="container">
        <Nuxt />
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar'
import Footer from '@/components/Footer'
export default {
  components: {
    Navbar,
    Footer
  }
}
</script>

<style>
  .bodys {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }
  main {
    margin-top: 40px;
    flex-grow: 1;
  }

  footer {
    flex-shrink: 0;
  }

  .questionnaire {
        margin-top: 40px;
        flex-wrap: wrap;
    }

  .flex-right {
        margin-left: 60px;
    }

  @media screen and (max-width: 991px) {
      .flex-right {
          margin-left: 0;
      }
  }

  @media screen and (max-width: 767px) {
      .flex-right__item {
          flex-wrap: wrap;
      }
  }

  .applicant-photo {
        width: 220px;
        height: 250px;
        background-color: rgb(83, 83, 83);
        margin-bottom: 20px;
    }

    .applicant-photo img{
        width: 100%;
        height: 100%;
    }

</style>