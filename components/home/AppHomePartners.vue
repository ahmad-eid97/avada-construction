<template>
    <section class="partners">
        <div class="container">
            <div class="row intro-text">
                <h2>Trusted Partners</h2>
                <div class="col-12 seprator">

                </div>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua ut enim ad minim veniam.
                </p>
            </div>
        </div> 
        <div class="row m-0">
            <swiper
                :options="swiperOption"
                :breakpoints="breakpoints"
            >
                <swiper-slide>
                    <div class="item">
                        <img class="imgo" src="https://avada.theme-fusion.com/construction/wp-content/uploads/sites/55/2015/12/home-logo10-219096700-320x202.png" width="150" height="150">
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="item">
                        <img class="imgo" src="https://avada.theme-fusion.com/construction/wp-content/uploads/sites/55/2015/12/home-logo2-219096700-320x202.png" width="150" height="150">
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="item">
                        <img class="imgo" src="https://avada.theme-fusion.com/construction/wp-content/uploads/sites/55/2015/12/home-logo1-219096700-320x202.png" width="150" height="150">
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="item">
                        <img class="imgo" src="https://avada.theme-fusion.com/construction/wp-content/uploads/sites/55/2015/12/home-logo9-219096700-320x202.png" width="150" height="150">
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="item">
                        <img class="imgo" src="https://avada.theme-fusion.com/construction/wp-content/uploads/sites/55/2015/12/home-logo11-219096700-320x202.png" width="150" height="150">
                    </div>
                </swiper-slide>
            </swiper>
        </div>
    </section>
</template>

<script>
// import carousel from 'vue-owl-carousel'

export default {
    name: 'AppHomePartners',
    components: { 
    //   carousel,
    },
    data() {
        return {
            swiperOption: {
                loop: true,
                slidesPerView: 5,
                spaceBetween: 50,
                breakpoints: {
                    // when window width is >= 320px
                    100: {
                    slidesPerView: 2,
                    spaceBetween: 5,
                    },
                    // when window width is >= 480px
                    480: {
                    slidesPerView: 3,
                    spaceBetween: 5,
                    },
                    // when window width is >= 640px
                    640: {
                    slidesPerView: 4,
                    spaceBetween: 5,
                    },
                    992: {
                    slidesPerView: 5,
                    spaceBetween: 5,
                    },
                    1200: {
                    slidesPerView: 5,
                    spaceBetween: 5,
                    },
                }
            },
        }
    }
}
</script>
<style>

    .partners {
        padding-top: 90px;
        margin-top: 0px;
        padding-right: 0;
        padding-bottom: 100px;
        margin-bottom: 0px;
        padding-left: 0;
    }
    .partners .intro-text {
        padding: 0 15% !important;
    }
    .partners h2 {
        font-weight: 400;
        line-height: 41.6px;
        letter-spacing: 1px;
        text-transform: capitalize;
        margin-bottom: 20px;
    }
    .partners .seprator {
        align-self: center;
        margin-left: auto;
        margin-right: auto;
        margin-top: 0px;
        margin-bottom: 30px;
        width: 100%;
        max-width: 206px;
        border-color: var(--main-color);
        border-top-width: 2px;
        border-top-style: solid
    }
    .partners p {
        color: rgb(116, 116, 116);
        font-size: 15px;
        font-weight: 500;
        line-height: 34.05px;

    }

    .partners .owl-carousel .item img {
        max-height: 115px;
        vertical-align: middle;
        width: auto;
        display: inline;
    }


</style>