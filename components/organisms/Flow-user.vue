<template>
    <div class="flow-container" id="flow">
        <div class="flow-title text-center">
            <h2>Flow Pelayanan User </h2>
        </div>
        <div class="flow-content">
            <div class="flow-daftar text-center">
                <img 
                    class="flow-daftar-image"
                    src="~/assets/image/flow-daftar.png" 
                    alt=""
                >
                <p class="mt-4 text-center text-light">
                    Daftar
                </p>

            </div>
            <div class="flow-konsultasi text-center">
                <img 
                    class="flow-konsultasi-image"
                    src="~/assets/image/flow-konsultasi.png" 
                    alt=""
                >
                <p class="mt-4 text-center text-light">
                    konsultasi <br> Project
                </p>
            </div>
            <div class="flow-nego text-center">
                <img 
                    class="flow-nego-image"
                    src="~/assets/image/flow-nego.png" 
                    alt=""
                >
                <p class="mt-4 text-center text-light">
                    Negoisasi
                </p>
            </div>
            <div class="flow-payment text-center">
                <img 
                    class="flow-payment-image"
                    src="~/assets/image/flow-payment.png" 
                    alt=""
                >
                <p class="mt-4 text-center text-light">
                    Pembayaran
                </p>
            </div>
            <div class="flow-mentoring text-center">
                <img 
                    class="flow-mentoring-image"
                    src="~/assets/image/flow-mentoring.png" 
                    alt=""
                >
                <p class="mt-4 text-center text-light">
                    Mentoring & <br> Development
                </p>
            </div>
            <div class="flow-finish text-center">
                <img 
                    class="flow-finish-image"
                    src="~/assets/image/flow-finish.png" 
                    alt=""
                >
                <p class="mt-4 text-center text-light">
                    Selesai
                </p>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.flow-container {
    background-color: #A4DEF9;
    font-family: nunito;
}
@media (max-width: 800px) {
    .flow-content {
        display: flex;
        justify-content: space-around;
    }
}
@media (max-width: 578px) {
    .flow-content {
        display: block;
        margin-top: 50px;
    }
    .flow-container {
        padding-top: 50px;
    }
}
@media (min-width: 800px) {
    .flow-container {
        background-color: #A4DEF9;
        height: 400px;
        margin-top: 140px;
}
    .flow-title {
        width: 70%;
        margin-left: 15%;
        text-align: center;
        padding-top: 60px;
    }
    .flow-content {
        display: flex;
        width: 90%;
        margin-left: 5%;
        justify-content: space-around;
        margin-top: 60px;
    }
    .flow-daftar-image,
    .flow-konsultasi-image,
    .flow-nego-image,
    .flow-payment-image,
    .flow-mentoring-image,
    .flow-finish-image {
        width: 90px;
    }


}

</style>