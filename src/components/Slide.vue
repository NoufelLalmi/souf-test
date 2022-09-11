<template>
    <div class="section">
        <div>
            <div class="section_text">
            <div class="section_title">
            Real Impact. Real Experiance
            </div>
            <div class="section_subtitle">
            Watch Success Stories from plus Custmers
            </div>
        </div>
        <div class="carousel">
            <div class="carousel-inner">
                <input class="carousel-open" type="radio" id="carousel-1" name="carousel" aria-hidden="true" hidden="" checked="checked">
                <div class="carousel-item">

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
                        <img src="../assets/img/img1.png">
                   
                </div>
                <!-- slide 2 -->
                <input class="carousel-open" type="radio" id="carousel-2" name="carousel" aria-hidden="true" hidden="">
                <div class="carousel-item">
                        <div class="img_wrapper">
                            
                            <div class="text_wrapper">
                                <div class="title_wrapper">
                                    <span class="slide_subtitle">Lorem epsom22</span>
                                    <span class="slide_title"> Lorem ipsum dolor22</span>
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
                        <img src="../assets/img/img1.png">
                    
                </div>
                
                    <label for="carousel-3" class="carousel-control prev control-1">‹</label>
                                <label for="carousel-2" class="carousel-control next control-1">›</label>
                                <label for="carousel-1" class="carousel-control prev control-2">‹</label>
                                <label for="carousel-3" class="carousel-control next control-2">›</label>
                                <label for="carousel-2" class="carousel-control prev control-3">‹</label>
                                <label for="carousel-1" class="carousel-control next control-3">›</label>
            
        
        </div>
        
        <!-- <ol class="carousel-indicators">
                    <li>
                        <label for="carousel-1" class="carousel-bullet">•</label>
                    </li>
                    <li>
                        <label for="carousel-2" class="carousel-bullet">•</label>
                    </li>
                    <li>
                        <label for="carousel-3" class="carousel-bullet">•</label>
                    </li>
                </ol> -->
        </div>

        <div class="thumbnail_container">
            <ol class="carousel-indicators">
                <li>
                    <div for="carousel-1" class="thumbnail_wrapper carousel-bullet">
                    <div class="thumbnail_img_wrapper">
                        <div class="thumbnail_img"></div>
                    </div>
                    <div class="thumbnail_title">
                        Watch Success Stories from plus Custmers
                    </div>
                </div>
                </li>
                <li>
                    <div for="carousel-2" class="thumbnail_wrapper carousel-bullet">
                    <div class="thumbnail_img_wrapper">
                        <div class="thumbnail_img">
                        </div>
                    </div>
                    <div class="thumbnail_title__active">
                        Watch Success Stories from plus Custmers
                    </div>
                </div>
                </li>
            </ol>
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
.section_text {
/* identical to box height, or 125% */
text-align: start !important;
letter-spacing: -0.02em;
}

.section_title {
font-weight: 700;
font-size: 48px;
line-height: 60px;
/* identical to box height, or 125% */

display: flex;
align-items: center;
letter-spacing: -0.02em;

/* text color */

color: #040C1C;
}
.section_subtitle {
font-weight: 400;
font-size: 24px;
line-height: 32px;
/* identical to box height, or 133% */

display: flex;
align-items: center;

color: #475467;

}
.slide_wrapper {
    width: 1140px;
    height: 430px;
    position: relative;
    border-radius: 12px;
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
    text-align: start;
}
.title_wrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 0px;
    width: 406px;
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

.carousel {
    position: relative;
    margin-top: 26px;
}

.carousel-inner {
    position: relative;
    overflow: hidden;
    width: 100%;   
    border-radius: 15px;
}

.carousel-open:checked + .carousel-item {
    position: static;
    opacity: 100;
}

.carousel-item {
    position: absolute;
    opacity: 0;
    -webkit-transition: opacity 0.6s ease-out;
    transition: opacity 0.6s ease-out;

    width: 1140px;
    height: 430px;
    border-radius: 12px;
}

.carousel-item img {
    overflow: none;
    height: auto;
    max-width: 100%;
}

.carousel-control {
    background: rgba(0, 0, 0, 0.28);
    border-radius: 50%;
    color: #fff;
    cursor: pointer;
    display: none;
    font-size: 40px;
    height: 40px;
    line-height: 35px;
    position: absolute;
    top: 50%;
    -webkit-transform: translate(0, -50%);
    cursor: pointer;
    -ms-transform: translate(0, -50%);
    transform: translate(0, -50%);
    text-align: center;
    width: 40px;
    z-index: 10;
}

.carousel-control.prev {
    left: 2%;
}

.carousel-control.next {
    right: 2%;
}

.carousel-control:hover {
    background: rgba(0, 0, 0, 0.8);
    color: #aaaaaa;
}

#carousel-1:checked ~ .control-1,
#carousel-2:checked ~ .control-2,
#carousel-3:checked ~ .control-3 {
    display: block;
}

.carousel-indicators {
    list-style: none;
    margin: 0;
    padding: 0;
    position: absolute;
    bottom: 2%;
    left: 0;
    right: 0;
    text-align: center;
    z-index: 10;
}

.carousel-indicators li {
    display: inline-block;
    margin: 0 5px;
}

.carousel-bullet {
    color: #fff;
    cursor: pointer;
    display: block;
    font-size: 35px;
}

.carousel-bullet:hover {
    color: #aaaaaa;
}

#carousel-1:checked ~ .control-1 ~ .carousel-indicators li:nth-child(1) .carousel-bullet,
#carousel-2:checked ~ .control-2 ~ .carousel-indicators li:nth-child(2) .carousel-bullet,
#carousel-3:checked ~ .control-3 ~ .carousel-indicators li:nth-child(3) .carousel-bullet {
    color: #428bca !important;
}


</style>
