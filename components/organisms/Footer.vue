<template>
    <div class="footer-container">
        <div class="footer-content">
            <div class="first-footer">
                <h5 class="first-footer-title">
                    Bimbinganbareng.com
                </h5>
                <p class="first-footer-paragraf">
                    Bimbinganbareng.com adalah jenis pelayanan jasa membing dan mentoring kebutuhan penyelesaian projek berupa Tugas Akhir, Tugas Kampus maupun Penelitian dengan tujuan memberikan bekal hardskill yang mumpuni untuk mereka agar lebih cepat dan lebih mudah dalam menyelesaikan projeknya.
                </p>

            </div>
            <div class="second-footer">
                <div>

                    <div class="second-footer-medsos">
                        <h5>
                            Media Sosial
                        </h5>
                        <a href="https://www.instagram.com/_akbrswalarr/">
                        <img 
                            class="footer-image"
                            src="~assets/image/instagram.png"
                            alt=""
                        >
                        </a>
                        <a href="https://www.facebook.com/syawal.cittruss">
                        <img 
                            class="footer-image"
                            src="~assets/image/facebook.png" 
                            alt=""
                        >
                        </a>

                    </div>
                    <div class="second-footer-address">
                        <h5 class="second-footer-title">
                            Alamat
                        </h5>
                        <p class="second-footer-paragraf">
                            Jl. Letda Sudjono No. 273, Medan Tembung Medan, Sumatera Utara
                        </p>
                    </div>
                </div>
                <div class="second-footer-contact">
                    <h5>
                        Hubungi Kami
                    </h5>
                    <div class="medsos-content">
                        <img 
                            class="footer-image"
                            src="~assets/image/whatsapp.png" 
                            alt=""
                        >
                        <a href="https://wa.me/6281397110834" class="medsos-content-paragraf">
                            081397110834
                        </a>
                    </div>

                </div>

            </div>
        </div>
        <div class="third-footer">
            <p class="third-footer-content font-weight-bold">
                © Copyright 2020 Bimbinganbareng.com
            </p>

        </div>

    </div>
</template>

<script>
export default {

}
</script>

<style>
.footer-container {
    background-color: #F8F9FA;
    margin-top: 100px;
    font-family: nunito;
}
.medsos-content {
    display: flex;
}
.footer-image {
    width: 40px;
}
.first-footer-paragraf,
.footer-image,
.second-footer-address,
.second-footer-paragraf {
    margin-top: 10px;
}
.medsos-content-paragraf {
    margin-top: 15px;
    margin-left: 10px;
}
.third-footer {
    background-color: #E2E2E2;
    padding-top: 5px;
}

@media (min-width: 800px) {
    .third-footer {
        margin-top: 70px;
        height: 50px;
    }
    .footer-content {
        width: 80%;
        margin-left: 10%;
        display: flex;
        justify-content: space-between;
    }
    .first-footer {
        width: 450px;
        margin-top: 70px;
    }
    .second-footer {
        width: 350px;
        margin-top: 70px;
    }
    .third-footer-content {
        width: 80%;
        margin-left: 10%;
        padding-top: 10px;
    }
}
@media (max-width: 800px) {
    .first-footer,
    .second-footer,
    .medsos-content {
        width: 100%;
        padding: 50px;
        text-align:  center;
        justify-content: center;
    }
    .third-footer {
        width: 100%;
        padding: 10px;
    }
    .third-footer-content {
        width: 100%;
        text-align: center;
    }
}

</style>