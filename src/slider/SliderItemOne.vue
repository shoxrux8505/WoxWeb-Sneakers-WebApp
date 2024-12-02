<template>
    <div class="slider-content" >
    <!-- Text Content -->
    <div class="text-content">
        <h1 class="text-3xl sm:text-4xl lg:text-5xl font-bold">Boshqacha bo'l</h1>
        <p class="text-sm ">biz bilan shaxsiy brendingizni yarating ! ⚡</p>
        <button class="py-2 px-5 bg-blue-500 text-white font-semibold rounded-full shadow-md hover:bg-violet-700 focus:outline-none focus:ring focus:ring-violet-400 focus:ring-opacity-75">
            <a href="#">More</a>
        </button>
    </div>

    <!-- Image Content -->
    <div class="img-content">
        <div class="circle ">
            <img src="./img/custm.png">
        </div>
    </div>
</div>

</template>

<style scoped>
.slider-content {
    width: 100%;
    height: 400px;
    display: flex;
    align-items: start;
    justify-content: space-around;
}

.slider-content .text-content {
    display: flex;
    align-items: flex-start;
    justify-content: flex-start;
    flex-direction: column;
    row-gap: 25px;
}

/* .slider-content .text-content h1 {
    position: absolute;
    top: 100px;
    font-size: 40px;
    text-align: center;
    font-family: "Playwrite CU", cursive;
    font-optical-sizing: auto;
    font-weight: weight;
    font-style: normal;
}

.slider-content .text-content p {
    font-family: "Playwrite CU", cursive;
    font-optical-sizing: auto;
    font-weight: weight;
    font-style: normal;
} */
.slider-content .img-content .circle{
    content: '';
    width: 500px;
    height: 495px;
    position: absolute;
    clip-path: circle(47.6% at 50% 84%);
    background: royalblue;
    top: -179px;
    right: 200px;
    z-index: -1;
    filter:  drop-shadow(0 0 10px royalblue);
    
    }
    .slider-content .img-content img{
        margin-top: 20px;
        filter: drop-shadow(0 0 10px #fff );
        
    }
</style>
