<template>
  <div class="home">
    <div>
      <img src="@/assets/KAUNGMINHTET.png" alt="my_pic" class="image-cus animate__animated animate__flipInX" />
      <h2 class="text-center my-2 animate__animated animate__fadeInDown">KAUNG MIN HTET</h2>
      <div class="shortline-cus animate__animated animate__fadeInLeft"></div>
      <h3 class="text-primary text-center my-2 animate__animated animate__fadeInDown">Web Developer</h3>
      <p class="text-center animate__animated animate__fadeInDown">
        Self-taught junior web developer seeking for an opportunity to extend my web development and multimedia editing skills and knowledge.
      </p>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HomeView',
}
</script>

<style lang="scss" scoped>
  .home {
    width: 100%;
    height: 100%;
    padding: 0 100px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .image-cus {
    width: 150px;
    margin: 0 auto;
    display: block;
    border-radius: 10px;
  }
  .shortline-cus {
    width: 300px;
    height: 1px;
    background: white;
    margin: 0 auto;
  }
  @media screen and (max-width: 500px) {
    .home {
      padding: 0 50px;
    }
    .image-cus {
      width: 100px;
    }
    h2 {
      font-size: 20px;
    }
    h3 {
      font-size: 18px;
    }
    p {
      font-size: 14px;
    }
  }
</style>