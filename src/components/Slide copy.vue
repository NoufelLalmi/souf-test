<template>
    <div class="section">
        <div class="slide_wrapper">
            <div class="img_wrapper">
                <div class="text_wrapper">
                    <div class="title_wrapper">
                        <span class="slide_subtitle">Lorem epsom</span>
                        <span class="slide_title"> Lorem ipsum dolor</span>
                    </div>
                    <span class="slide_description"
                        >Lorem ipsum dolor sit amet, consectetur adipiscing
                        elit. Nunc euismod condimentum gravida aliquet venenatis
                        suspendisse pulvinar tortor sed. Et, hac ac at nisl sed
                        nullam sit gravida. Quam tempus elit, consectetur nibh
                        sodales sed arcu.</span
                    >
                    <div class="slide_action">
                        <span>Watch testimonial</span>
                        <img src="../assets/img/play.png" alt="" />
                    </div>
                </div>
            </div>
        </div>

        <div class="thumbnail_container">
            <div class="thumbnail_wrapper">
                <div class="thumbnail_img_wrapper">
                    <div class="thumbnail_img"></div>
                </div>
                <div class="thumbnail_title">
                    Watch Success Stories from plus Custmers
                </div>
            </div>
            <div class="thumbnail_wrapper">
                <div class="thumbnail_img_wrapper">
                    <div class="thumbnail_img">
                    </div>
                </div>
                <div class="thumbnail_title__active">
                    Watch Success Stories from plus Custmers
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style scoped>
.section {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px;
    gap: 24px;
}
.slide_wrapper {
    width: 1140px;
    height: 430px;
    position: relative;
    border-radius: 12px;

    background-image: url("../assets/img/img1.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;

    /* Inside auto layout */

    -webkit-transition: opacity 0.6s ease-out;
    transition: opacity 0.6s ease-out;
}
.img_wrapper {
    width: 1140px;
    height: 430px;
    position: absolute;
    border-radius: 12px;
    background: linear-gradient(
        90deg,
        rgba(4, 12, 28, 0.65) 26.59%,
        rgba(0, 0, 0, 0) 75.7%
    );
}

.text_wrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 0px;
    gap: 24px;
    position: absolute;
    width: 406px;
    height: 214px;
    left: 46px;
    top: 108px;
    color: white;
}
.title_wrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 0px;
    width: 267px;
    height: 70px;

    flex: none;
    order: 0;
    flex-grow: 0;
}
.slide_title {
    font-weight: 500;
    font-size: 30px;
    line-height: 38px;
}
.slide_subtitle {
    font-weight: 500;
    font-size: 24px;
    line-height: 32px;
}
.slide_description {
    font-weight: 400;
    font-size: 14px;
    line-height: 20px;
}

.slide_action {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    padding: 0px;
    gap: 12px;
    /* Inside auto layout */
    flex: none;
    order: 1;
    flex-grow: 0;
}

/* mini slide */
.thumbnail_container {
    display: flex;
    flex-direction: row;
    align-items: baseline;
    padding: 0px;
    gap: 16px;

    width: 516px;
    height: 146px;

    /* Inside auto layout */

    flex: none;
    order: 1;
    flex-grow: 0;
}
.thumbnail_wrapper {
    width: 115px;
    height: 80px;
    margin: 0px 11px;
    display: flex;
    flex-direction: column;
    align-items: center;
    border-radius: 15%;

    /* Inside auto layout */

    flex: none;
    order: 0;
    flex-grow: 0;
}
.thumbnail_img_wrapper {
    position: relative;
    width: 105px;
    height: 80px;
    left: -0.42px;
    top: 0px;
    background: rgba(255, 255, 255, 0.34);

}
.thumbnail_img {
    width: 105px;
    height: 80px;
    left: -0.42px;
    top: 0px;
    border-radius: 6px;
    background-image: url("../assets/img/img1.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;

    
}
.thumbnail_title__active {
    font-weight: 700;
    font-size: 14px;
    line-height: 20px;
    margin-top: 6px;
    /* or 143% */

    display: flex;
    align-items: center;
    text-align: center;

    /* text color */

    color: #040c1c;
}
.thumbnail_title {
    font-weight: 500;
    font-size: 14px;
    line-height: 20px;
    margin-top: 6px;
    /* or 143% */

    display: flex;
    align-items: center;
    text-align: center;

    color: #999ca1;
}
</style>
