<template>
    <div class="section">
        <div class="carousel">
            <div class="carousel-inner">
                <input class="carousel-open" type="radio" id="carousel-1" name="carousel" aria-hidden="true" hidden="" checked="checked">
                <div class="carousel-item">
                    <div class="img_wrapper">
                        <img src="../assets/img/img1.png">
                    </div>
                </div>
                <input class="carousel-open" type="radio" id="carousel-2" name="carousel" aria-hidden="true" hidden="">
                <div class="carousel-item">
                    <div class="img_wrapper">
                        <img src="../assets/img/img1.png">
                    </div>
                </div>
                <input class="carousel-open" type="radio" id="carousel-3" name="carousel" aria-hidden="true" hidden="">
                <div class="carousel-item">
                    <img src="http://fakeimg.pl/2000x800/F90/fff/?text=Carousel">
                </div>
                <label for="carousel-3" class="carousel-control prev control-1">‹</label>
                <label for="carousel-2" class="carousel-control next control-1">›</label>
                <label for="carousel-1" class="carousel-control prev control-2">‹</label>
                <label for="carousel-3" class="carousel-control next control-2">›</label>
                <label for="carousel-2" class="carousel-control prev control-3">‹</label>
                <label for="carousel-1" class="carousel-control next control-3">›</label>
                
    </div>

    <ol class="carousel-indicators">
                    <li>
                        <label for="carousel-1" class="carousel-bullet">•</label>
                    </li>
                    <li>
                        <label for="carousel-2" class="carousel-bullet">•</label>
                    </li>
                    <li>
                        <label for="carousel-3" class="carousel-bullet">•</label>
                    </li>
                </ol>

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

    background: linear-gradient(
        90deg,
        rgba(4, 12, 28, 0.65) 26.59%,
        rgba(0, 0, 0, 0) 75.7%
    );
    z-index: 9;

}

.carousel-item img {
    display: block;
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
    color: #428bca;
}

#title {
    width: 100%;
    position: absolute;
    padding: 0px;
    margin: 0px auto;
    text-align: center;
    font-size: 27px;
    color: rgba(255, 255, 255, 1);
    font-family: 'Open Sans', sans-serif;
    z-index: 9999;
    text-shadow: 0px 1px 2px rgba(0, 0, 0, 0.33), -1px 0px 2px rgba(255, 255, 255, 0);
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
    z-index: 10;
}
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

</style>
