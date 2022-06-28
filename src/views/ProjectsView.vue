<template>
    <div class="projects">
        <div class="content-cus">
            <h1 class="cus-text mb-3 animate__animated animate__fadeInDown">My recent projects</h1>
            <div class="shortline-cus my-3 animate__animated animate__fadeInLeft"></div>
            <div id="carouselExampleIndicators" class="carousel slide animate__animated animate__flipInX" data-bs-ride="true">
                <div class="carousel-indicators">
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0"
                        class="active" aria-current="true" aria-label="Slide 1"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"
                        aria-label="Slide 2"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"
                        aria-label="Slide 3"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3"
                        aria-label="Slide 4"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="4"
                        aria-label="Slide 5"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="5"
                        aria-label="Slide 6"></button>
                </div>
                <div class="carousel-inner cus-radius">
                    <div class="carousel-item active custom-hover">
                        <img src="../assets/tracker19.png" class="d-block w-100 cus-radius" alt="tracker">
                        <div class="custom-hover-container">
                            <div>
                                <h2>Covid19 Tracker</h2>
                                <a href="https://tracker19-kenny.netlify.app/" target="_blank" class="btn btn-primary">Check -></a>
                            </div>
                        </div>
                    </div>
                    <div class="carousel-item custom-hover">
                        <img src="../assets/exchange.png" class="d-block w-100 cus-radius cus-radius" alt="exchg">
                        <div class="custom-hover-container">
                            <div>
                                <h2>Exchange-Calculator</h2>
                                <a href="https://kmhexhcalc.netlify.app/" target="_blank" class="btn btn-primary">Check -></a>
                            </div>
                        </div>
                    </div>
                    <div class="carousel-item custom-hover">
                        <img src="../assets/mui.png" class="d-block w-100 cus-radius" alt="mui">
                        <div class="custom-hover-container">
                            <div>
                                <h2>React-mui</h2>
                                <a href="https://kenny-mui.netlify.app/" target="_blank" class="btn btn-primary">Check -></a>
                            </div>
                        </div>
                    </div>
                    <div class="carousel-item custom-hover">
                        <img src="../assets/taptap-music.png" class="d-block w-100 cus-radius" alt="taptap">
                        <div class="custom-hover-container">
                            <div>
                                <h2>TapTap-Music</h2>
                                <a href="https://taptap-music.netlify.app/" target="_blank" class="btn btn-primary">Check -></a>
                            </div>
                        </div>
                    </div>
                    <div class="carousel-item custom-hover">
                        <img src="../assets/portfolio2.png" class="d-block w-100 cus-radius" alt="portfolio2">
                        <div class="custom-hover-container">
                            <div>
                                <h2>Portfolio</h2>
                                <a href="https://profilekmh.netlify.app/" target="_blank" class="btn btn-primary">Check -></a>
                            </div>
                        </div>
                    </div>
                    <div class="carousel-item custom-hover">
                        <img src="../assets/portfolio.png" class="d-block w-100 cus-radius" alt="portfolio">
                        <div class="custom-hover-container">
                            <div>
                                <h2>Portfolio-Test</h2>
                                <a href="https://kaung-portfolio.netlify.app/" target="_blank" class="btn btn-primary">Check -></a>
                            </div>
                        </div>
                    </div>
                </div>
                <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators"
                    data-bs-slide="prev">
                    <span class="carousel-control-prev-icon text-dark" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators"
                    data-bs-slide="next">
                    <span class="carousel-control-next-icon text-dark" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HomeView',
}
</script>

<style lang="scss" scoped>
.projects {
    width: 100%;
    height: 100%;
    padding: 0 0 0 100px;
    display: grid;
    place-items: center;
}

.cus-radius {
    border-radius: 10px !important;
}

.content-cus {
    width: 100%;
}

.delay-1 {
    animation-delay: 0.2s;
}

.delay-2 {
    animation-delay: 0.4s;
}

.delay-3 {
    animation-delay: 0.6s;
}

.delay-4 {
    animation-delay: 0.8s;
}

// custom
.custom-hover {
    postition: relative;
}


.custom-hover-container {
    width: 100%;
    height: 100%;
    background-color: #00000070;
    backdrop-filter: blur(2px);
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    bottom: -100%;
    left: 0;
    transform: scale(0);
    transition: all 0.5s;
}

.custom-hover:hover .custom-hover-container {
    bottom: 0;
    left: 0;
    transform: scale(1);
}
.shortline-cus {
        width: 100%;
        height: 1px;
        background: white;
    }

@media screen and (max-width: 500px) {
    .projects {
        padding: 0 30px 0 50px;
    }

    .cus-text {
        font-size: 20px;
        text-align: center;
    }
}

@media screen and (max-width: 1200px) {
    .projects {
        padding: 0 0 0 25px;
    }

    .cus-text {
        font-size: 24px;
        text-align: center;
    }

}
</style>