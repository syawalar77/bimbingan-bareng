<template>
    <div id="services" class="container-services">
        <div class="services-title">
            <h2 class="text-center">Pelayanan yang diberikan</h2>
            <p class="text-center services-title-paragraf">Ada beberapa kategori projek website dan aplikasi mobile yang kami layani, diantaranya sebagai berikut</p>
        </div>
        <div class="services-content">
            <div class="services-left">
                <img 
                    class="services-image"
                    src="~/assets/image/vector-left.png" 
                    alt="image not found"
                >
                <p class="services-left-paragraf">Bimbingan Projek Website atau Aplikasi Mobile untuk Tugas Akhir</p>
            </div>
            <div class="services-middle">
                <img 
                    class="services-image"
                    src="~/assets/image/vector-middle.png" 
                    alt="image not found"
                >
                <p class="services-middle-paragraf">Membantu dan Mentoring Penelitian berupa Website dan Aplikasi Mobile</p>
            </div>
            <div class="services-right">
                <img 
                    class="services-image"
                    src="~/assets/image/vector-right.png" 
                    alt="image not found"
                >
                <p class="services-right-paragraf">Tugas dan Projek Kampus berupa Website dan Mobile Aplikasi</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.container-services {
    font-family: nunito;
}
.services-title {
    width: 60%;
    margin-left: 20%;
    margin-top: 100px;
}
.services-title-paragraf {
    font-size: 22px;
}
.services-content {
    display: flex;
    width: 90%;
    margin-left: 5%;
    justify-content: space-between;
    margin-top: 60px;
}
.services-left, 
.services-middle,
.services-right {
    width: 335px;
    display: flex;
    border-radius: 40px;
    padding: 20px;
    box-shadow: inset 0px -3px 3px rgb(0, 0, 0, 0.25);
}
.services-image {
    width: 70px!important;
    height: 70px;
    margin-top: 7px;
    margin-left: 10px
}
.services-left-paragraf,
.services-middle-paragraf,
.services-right-paragraf {
    font-size: 15px;
    margin-left: 30px;
    margin-top: 10px;
}
@media (max-width: 800px) {
    .services-content {
        display: block;
        padding: 50px;
    }
    .services-left, 
    .services-middle,
    .services-right {
        width: 100%;
        margin-top: 20px;
    }
}
@media (max-width: 400px) {
    .services-left, 
    .services-middle,
    .services-right {
        width: 100%;
        margin-top: 20px;
        display: block;
        text-align: center;
    }
    .services-left-paragraf,
    .services-middle-paragraf,
    .services-right-paragraf {
        margin: 0;
    }
        
}
</style>