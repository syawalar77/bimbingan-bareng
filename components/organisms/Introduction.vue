<template>
    <div class="introduction-container">
        <div class="introduction">
            <div class="introduction-left">
                <p class="introduction-paragraf text-light">
                    Membantu bimbingan, mentoring dan penyelesaian Projek, Tugas Akhir dan Penelitian berupa Website dan Aplikasi Mobile.
                </p>
                <Button 
                    titleBtn="Daftar"
                />

            </div>
            <div class="introduction-right ml-auto">
                <img 
                    class="introduction-image"
                    src="~/assets/image/intro.png" 
                    alt="image not found"
                    style="max-width:400px;"
                >
            </div>
        </div>

    </div>
</template>

<script>
import Button from '~/components/atoms/Button.vue'
export default {
    components: {
        Button,
    }
}
</script>

<style>
.introduction-container {
    background-color: #A4DEF9;
    font-family: nunito;
}
@media (min-width :800px) {
    .introduction-container {
        height: 500px;
    }

    .introduction {
        display: flex; 
        width: 70%;
        margin-left: 15%;
    }
    .introduction-paragraf {
        font-size: 27px;
        margin-top: 50px;
    }
    .introduction-left, .introduction-right {
        width: 400px;
        margin-top: 100px;
    }
}
@media (max-width: 800px) {
    .introduction-left {
        max-width: 100%!important;
        padding: 50px;
        text-align: center;
    }
    .introduction-image {
        max-width: 100%!important;
        padding: 50px;
        margin-top: -30px;
    }
}
</style>