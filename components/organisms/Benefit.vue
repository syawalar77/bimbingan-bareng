<template>
    <div class="benefit-container" id="benefit">
        <div class="firts-benefit">
            <img 
                class="first-benefit-image"
                src="~/assets/image/graduation.png" 
                alt=""
            >
            <div class="first-benefit-content">
                <h3 class="first-benefit-title">Lebih Mudah Menyelesaikan Tugas Akhir</h3>
                <p class="first-benefit-paragraf">Sebagai mentor dan pembimbing, Bimbinganbareng membantu kamu dari sisi teknikal dalam menyelesaikan projek kamu </p>
            </div>
        </div>
        <div class="second-benefit">
            <img 
                class="second-benefit-image"
                src="~/assets/image/coding.png" 
                alt=""
            >
            <div class="second-benefit-content">
                <h3 class="second-benefit-title">Hardskill Software Development Website dan Aplikasi Mobile</h3>
                <p class="second-benefit-paragraf">Dengan menggunakan layanan Bimbinganbareng, selain kamu dibantu menyelesaikan projek, kamu akan dimentoring tentang proses development sebuah Website ataupun Aplikasi Mobile</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.benefit-container {
    margin-top: 150px;
    padding-top: 50px;
}
@media (min-width: 800px) {
    .firts-benefit,
    .second-benefit {
        width: 90%;
        background-color: #F8F9FA;
        display: flex;
        padding: 30px;
    }
    .firts-benefit {
        justify-content: space-evenly;

    }
    .second-benefit {
        margin-top: 100px;
        margin-left: 10%;
    }
    .first-benefit-title,
    .second-benefit-title {
        font-size: 27px;
    }
    .first-benefit-paragraf,
    .second-benefit-paragraf {
        font-size: 19px;
    }
    .first-benefit-image,
    .second-benefit-image {
        width: 370px;
    }
    .second-benefit-image {
        margin-left: 40px;
    }
    .first-benefit-image {
        margin-left: 50px;
    }
    .first-benefit-content,
    .second-benefit-content {
        width: 400px;
        margin-top: 70px;
    }
    .second-benefit-content {
        margin-left: 80px;
    }
}
@media (max-width: 800px) {
    .first-benefit-image,
    .second-benefit-image {
        width: 100%;
        padding: 50px;
        text-align: center;
    }
    .first-benefit-content,
    .second-benefit-content {
        width: 100%; 
        padding: 50px;
        text-align: center;
        margin-top: -7x0px;
    }

}
</style>