<template>
    <div class="registration-container">
        <h2 class="title-registration">Daftar Sekarang</h2>
        <div class="registration">
            <div class="registration-form">
                <FromInput
                    class="input"
                    label="Nama Lengkap"
                    placeholder="contoh: Taufik Hidayat"
                
                />
                <FromInput
                    class="input"
                    label="Email"
                    placeholder="Taufik@gmail.com"
                
                />
                <FromInput
                    class="input"
                    type="number"
                    label="Ponsel (WhatsApp)"
                    placeholder="081234567890"
                
                />
                <FromInput
                    class="input"
                    label="Judul Projek"
                    placeholder="contoh: Website portal berita kampus"
                
                />
                <div class="form-group">
                    <label for="exampleInputPassword1">Deskripsi Tentang Projek</label>
                    <textarea
                        type="text" 
                        class="form-control input textarea" 
                        id="exampleFormControlTextarea1"
                        rows="5"
                        placeholder="Contoh:  Jadi saya ingin membuat projek tugas akhir berupa web berita portal kampus."
                    >
                    </textarea>
                </div>
                <button
                    class="btn btn-warning text-light btn-regstration"
                >
                    <span
                        class="text-dark"
                        role="status"
                        aria-hidden="true"
                    ></span>
                    Daftar
                </button>

            </div>
            <img
                class="registration-image" 
                src="~/assets/image/registration.png" 
                alt=""
            >
        </div>
       
    </div>
</template>

<script>
import FromInput from '~/components/atoms/From-input.vue'
export default {
    components : {
        FromInput,
    },
    

}
</script>

<style>
.registration-container {
    font-family: nunito;
}
@media (min-width: 800px) {
    .registration-container {
        width: 90%;
        margin-left: 5%;
        margin-top: 100px;

    }
    .registration  {
        display: flex;
        justify-content: space-between;
    }
    .title-registration {
        margin-left: 10%;
    }
    .registration-form {
        width: 300px;
        margin-left: 10%;
        margin-top: 30px;
    }
    .registration-image {
        width: 500px;
    }
    
}
@media (max-width: 800px) {
    .registration-container {
        width: 100%;
        margin-top: 100px;

    }
    .registration-form {
        width: 100%;
        padding: 50px;
    }
}
@media (max-width: 600px) {
    .registration-image,
    .registration-form {
        width: 100%;
        padding: 50px;
        margin-top: -30px;
    }
    .title-registration {
        width: 100%; 
        padding: 0 50px;
    }
}
    .btn-regstration {
        background: #A4DEF9;
        border-radius: 5px;
        width: 140px;
        margin-top: 20px;
    }



</style>