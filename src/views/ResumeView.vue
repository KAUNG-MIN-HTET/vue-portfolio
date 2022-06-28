<template>
    <div class="resume">
        <div>
            <h2 class="animate__animated animate__fadeInDown">Here is my resume!</h2>
            <div class="shortline-cus my-3 animate__animated animate__fadeInLeft"></div>
            <img src="../assets/resume.png" alt="resume" class="animate__animated animate__flipInX" />
            <a href="../assets/resume.png" download="KAUNG-MIN-HTET-RESUME" class="btn btn-primary mt-3 animate__animated animate__fadeInDown">
                Download Resume
            </a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .resume {
        width: 100%;
        height: 100%;
        padding: 0 100px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    img {
        width: 250px;
        display: block;
        border-radius: 10px;
    }
    .shortline-cus {
        width: 250px;
        height: 1px;
        background: white;
    }
    @media screen and (max-width: 500px) {
        h2 {
            text-align: center;
            font-size: 20px;
        }
        img {
            width: 150px;
            margin: 0 auto;
        }
        .btn {
            width: 200px;
            display: block;
            margin: auto;
            font-size: 14px;
        }
    }
</style>