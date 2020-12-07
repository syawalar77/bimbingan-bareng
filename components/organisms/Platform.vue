<template>
    <div class="platform-container" id="platform">
        <div class="platform-title">
            <h2>
                Platform yang Didukung
            </h2>
            <p class="platform-title-paragraf">
                Ada dua platform yang didukung dan menjadi target pelayanan dari Bimbinganbareng, yaitu sebagai berikut.
            </p>
        </div>
        <div class="platform-content">
            <div class="first-platform">
                <img 
                    class="first-platform-image"
                    src="~/assets/image/platform-first.png" 
                    alt=""
                >
                <div class="first-platform-content">
                    <h3 class="first-content-title">
                        Website,Desktop Maupun Mobile
                    </h3>
                    <p class="first-content-paragraf ">
                        Projek yang dihasilkan berupa website yang kompatible dengan layar apapun (Desktop, Mobile, maupun tablet)
                    </p>
                </div>
            </div>
            <div class="second-platform">
                <div class="second-platform-content">
                    <h3 class="second-content-title">
                        Aplikasi Mobile,Android
                    </h3>
                    
                    <p class="second-content-paragraf">
                        Projek yang dihasilkan berupa aplikasi mobile yang dapat digunakan di smartphone. Untuk saat ini masih mendukung environment Android.
                    </p>

                </div>
                <img 
                    class="second-platform-image"
                    src="~/assets/image/platform-second.png"
                    style="max-width:400px;" 
                    alt=""
                >
            </div>

        </div>

    </div>
</template>

<script>
export default {

}
</script>

<style>
.platform-container {
    padding-top: 60px;
}
@media (min-width: 800px) {
    .platform-title {
        width: 70%;
        margin-left: 15%;
        text-align: center;
    }

    .platform-title-paragraf {
        font-size: 22px;
    }

    .first-platform-image {
        width: 400px;
        margin-left: 10%;
        
    }
    .second-platform-image {
        width: 238px;
        margin-right: 10%;
    }
    .first-platform,
    .second-platform {
        display: flex;
        width: 90%;
        justify-content: space-evenly;
    }
    .first-platform,
    .platform-container {
        margin-top: 100px;
    }
    .second-platform {
        margin-left: 10%;
        margin-top: 80px;
    }
    .first-platform-content,
    .second-platform-content {
        width: 400px;

    }
    .second-content-title {
        margin-top: 100px;
    }
    .first-content-title {
        margin-top: 40px;
    }
    .first-content-paragraf,
    .second-content-paragraf {
        font-size: 19px ;
    }
}

@media (max-width: 800px) {
    .platform-title,
    .first-content-title,
    .second-content-title,
    .first-content-paragraf,
    .second-content-paragraf,
    .first-platform-image,
    .second-platform-image {
        width: 100%;
        padding: 50px;
        text-align: center;
    }
    .first-content-title,
    .second-content-title {
        margin-top: -50px;
    }
    .first-content-paragraf,
    .second-content-paragraf,
    .first-platform-image,
    .second-platform-image {
        margin-top: -80px;
    }
    
}
</style>