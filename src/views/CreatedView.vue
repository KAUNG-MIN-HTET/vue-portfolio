<template>
    <div class="created">
        <div>
            <h2 class="animate__animated animate__fadeInDown">This website was created using</h2>
            <div class="shortline-cus my-3 animate__animated animate__fadeInLeft"></div>
            <div class="icons  animate__animated animate__heartBeat">
                <span class="bg-primary text-dark pt-2 pb-1 px-2 pt-md-4 pb-md-2 px-md-3 rounded">
                    <i class="fa-brands fa-vuejs"></i>
                </span>
                <span class="bg-primary text-dark pt-2 pb-1 px-2 pt-md-4 pb-md-2 px-md-3 rounded ms-3">
                    <i class="fa-brands fa-bootstrap"></i>
                </span>
            </div>

            <h2 class="mt-3 mt-md-5 animate__animated animate__fadeInDown">Built wireframe using</h2>
            <div class="shortline-cus my-3 animate__animated animate__fadeInLeft"></div>
            <div class="icons  animate__animated animate__heartBeat">
                <span class="bg-primary text-dark pt-2 pb-1 px-2 pt-md-4 pb-md-2 px-md-3 rounded">
                    <i class="fa-brands fa-figma"></i>
                </span>
            </div>

            <p class="mt-3 mt-md-5 text-primary animate__animated animate__fadeInUp">
                Build awesome things!<br />
                Be creative!
            </p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.created {
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

i {
    font-size: 40px;
}

@media screen and (max-width: 500px) {
    .created {
        text-align: center;
        padding: 0 20px;
    }

    h2 {
        font-size: 20px;
    }

    p {
        font-size: 14px;
    }

    i {
        font-size: 20px;
    }
}
</style>