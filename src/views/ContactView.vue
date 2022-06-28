<template>
    <div class="contact h-100">
        <div>
            <h2 class="animate__animated animate__fadeInDown">
                Contact me to employ fast!
            </h2>
            <div class="shortline-cus my-3 animate__animated animate__fadeInLeft"></div>
            <p class="animate__animated animate__fadeInDown"><span class="text-primary">Email: </span>kaungminhtet2712@gmail.com</p>
            <p class="animate__animated animate__fadeInDown"><span class="text-primary">Phone: </span>09424497340</p>
            <div class="d-flex">
                <a href="mailto:kaungminhtet2712@gmail.com" class="btn btn-primary link-cus animate__animated animate__flipInX" >
                    <i class="fa-solid fa-envelope"></i>
                    Email Me
                    </a>
                <a href="tel:09424497340" class="btn btn-primary ms-3 link-cus animate__animated animate__flipInX" >
                    <i class="fa-solid fa-phone"></i>
                    Call Me
                </a>
            </div>
            <div class="social-links mt-3">
                <a href="https://www.facebook.com/kaung.minhtet.5283" target="_blank" class="btn btn-outline-primary rounded-circle me-2 animate__animated animate__rollIn">
                    <i class="fa-brands fa-facebook"></i>
                </a>
                <a href="https://github.com/KAUNG-MIN-HTET" target="_blank" class="btn btn-outline-primary rounded-circle me-2 animate__animated animate__rollIn">
                    <i class="fa-brands fa-github"></i>
                </a>
                <a href="https://www.linkedin.com/in/kaung-min-htet-805884218/" target="_blank" class="btn btn-outline-primary rounded-circle me-2 animate__animated animate__rollIn">
                    <i class="fa-brands fa-linkedin"></i>
                </a>
                <a href="https://www.instagram.com/kaung.minhtet.5283/" target="_blank" class="btn btn-outline-primary rounded-circle me-2 animate__animated animate__rollIn">
                    <i class="fa-brands fa-instagram"></i>
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .contact {
        width: 100%;
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
        .contact {
            padding: 0 50px;
            text-align: center;
            font-size: 14px;
        }
        .link-cus {
            display: inline-block;
            width: 120px;
            padding: 5px;
            font-size: 16px;
        }
        h2 {
            font-size: 20px;
        }
    }
</style>