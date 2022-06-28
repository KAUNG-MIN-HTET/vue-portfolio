<template>
  <div class="about">
    <div>
      <h3 class="animate__animated animate__fadeInDown">
        Born in 1999. Raised in yangon. Been hard at work since 2019.
      </h3>
      <div class="shortline-cus my-3 animate__animated animate__fadeInLeft"></div>
      <p class="animate__animated animate__fadeInDown">
        I’m Kaung Min Htet. A creative designer and  a web developer currently finding job opportunities to build creative and interactive website for your company.
      </p>
      <p class="animate__animated animate__fadeInDown">
        Proficient in Graphic Design, Microsoft Office, Programming, Data Analysis.
      </p>
      <p class="animate__animated animate__fadeInDown">
        I enjoy a good cup of coffee, watching good movies and anime. Playing video games or do anything music related.
      </p>
      <p class="text-primary animate__animated animate__fadeInUp">
        Always Create.<br />
        Art. Food. Whatever. Enjoy the beauty of it.
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .about {
    width: 100%;
    height: 100%;
    padding: 0 100px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .shortline-cus {
    width: 100%;
    height: 1px;
    background: white;
  }

  @media screen and (max-width: 500px) {
    .about {
      text-align: center;
      padding: 0 20px;
    }
    h3 {
      font-size: 18px;
    }
    p {
      font-size: 14px;
    }
  }
</style>
