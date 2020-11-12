<template>
    <div class="teknologi-container" id="teknologi">
        <div class="teknologi">
            <h3 class="teknologi-title">
                Teknologi yang Digunakan
            </h3>
            <p class="teknologi-paragraf">
                Bimbinganbareng menggunakan teknologi dan stack  yang paling banyak digunakan di dunia kerja dan di dunia Startup, diantaranya sebagai berikut.
            </p>
        </div>
        <div class="teknologi-content">
            <div class="teknologi-vuejs">
                <img 
                    class="image-vuejs"
                    src="~/assets/image/image-vuejs.png" 
                    alt=""
                >
                <p class="title-vuejs">Vue js</p>
            </div>
            <div class="teknologi-reactjs">
                <img 
                    class="image-reactjs"
                    src="~/assets/image/image-reactjs.png" 
                    alt=""
                >
                <p class="title-reactjs">React js <br> React Native</p>
            </div>
            <div class="teknologi-nodejs">
                <img 
                    class="image-nodejs"
                    src="~/assets/image/image-nodejs.png" 
                    alt=""
                >
                <p class="title-nodejs">Node js</p>
            </div>
            <div class="teknologi-golang">
                <img 
                    class="image-golang"
                    src="~/assets/image/image-golang.png" 
                    alt=""
                >
                <p class="title-golang">Golang</p>
            </div>
            <div class="teknologi-phyton">
                <img 
                    class="image-phyton"
                    src="~/assets/image/image-phyton.png" 
                    alt=""
                >
                <p class="title-phyton">Phyton</p>
            </div>

        </div>

    </div>

</template>

<script>
export default {

}
</script>

<style>
.teknologi-container {
    margin-top: 130px;
    background-color: #F8F9FA;
    font-family: nunito;
}
.teknologi {
    width: 70%;
    margin-left: 15%;
    text-align: center;
}
.teknologi-title  {
    font-size: 32px;
    padding-top: 50px;
}
.teknologi-paragraf {
    font-size: 22px;
    margin-top: 30px;
}
.teknologi-vuejs,
.teknologi-reactjs,
.teknologi-nodejs,
.teknologi-golang,
.teknologi-phyton {
    justify-content: center;
    text-align: center;
    font-size: 20px;
}
@media (min-width: 800px) {
    .teknologi-content {
        display: flex;
        width: 90%;
        margin-left: 5%;
        justify-content: space-around;
        padding: 50px;
    }
    .image-golang {
        width: 120px;
    }
    .image-vuejs {
        margin-top: 40px;
        width: 80px;
    }
    .image-reactjs {
        width:200px;
    }
    .image-nodejs {
        width: 220px;
    }
    .image-phyton {
        width: 95px;
        margin-top: 15px;
    }
    .title-vuejs {
        margin-top: 5px;
    }
    .title-reactjs {
        margin-top: -20px;
    }
    .title-nodejs {
        margin-top: 10px;
    }

    .title-phyton {
        margin-top: 15px;
    }
}
</style>