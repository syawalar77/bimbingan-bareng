<template>
    <div class="registration-container" id="registration">
        <h2 class="title-registration">Daftar Sekarang</h2>
        <div class="registration">
            <div class="registration-form">
                <FromInput
                    class="input"
                    label="Nama Lengkap"
                    placeholder="contoh: Taufik Hidayat"
                    :errorMessage="errorMsg.fullname"
                    v-model="fullname"
                    @keypress="checkValue('fullname')"
                />
                <FromInput
                    class="input"
                    label="Email"
                    type= "email"
                    pattern=".+@beststartupever.com"
                    placeholder="Taufik@gmail.com"
                    :errorMessage="errorMsg.email"
                    v-model="email"
                    @keypress="checkValue('email')"
                />
                <FromInput
                    class="input"
                    type="number"
                    label="Ponsel (WhatsApp)"
                    placeholder="081234567890"
                    :errorMessage="errorMsg.whatsApp"
                    v-model="whatsApp"
                    @keypress="checkValue('whatsApp')"
                />
                <FromInput
                    class="input"
                    label="Judul Projek"
                    placeholder="contoh: Website portal berita kampus"
                    :errorMessage="errorMsg.titleProject"
                    v-model="titleProject"
                    @keypress="checkValue('titleProject')"
                />
                <div class="form-group">
                    <label for="exampleInputPassword1">Deskripsi Tentang Projek</label>
                    <textarea
                        type="text" 
                        class="form-control input textarea" 
                        id="exampleFormControlTextarea1"
                        rows="5"
                        placeholder="Contoh:  Jadi saya ingin membuat projek tugas akhir berupa web berita portal kampus."
                        v-model="descProject"
                        @keypress="checkValue('descProject')"
                    >
                    </textarea>
                    <p 
                        class="error-msg" 
                        v-if="errorMessage"
                    >
                        {{ errorMessage }}
                    </p>
                </div>
                <button
                    class="btn text-light btn-registration"
                    @click.prevent="clickSubmit"
                >
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
    data() {
        return {
            fullname: '',
            email: '',
            whatsApp: '',
            titleProject: '',
            descProject: '',
            errorMessage: '',
            errorMsg: {
                fullname: '',
                email: '',
                whatsApp: '',
                titleProject: '',
            },
        }
    },
    methods: {
        validateInput() {
            if(this.fullname == '') {
                this.errorMsg.fullname = 'Nama lengkap harus diisi'
            }
            if(this.email == '') {
                this.errorMsg.email = 'Email harus diisi'
            }
            if(this.whatsApp == '') {
                this.errorMsg.whatsApp = 'WhatsApp harus diisi'
            }
            if(this.titleProject == '') {
                this.errorMsg.titleProject = 'Judul projek harus diisi'
            }
            if(this.descProject == '') {
                this.errorMessage = 'Deskripsi projek harus diisi'
            }
        },

        clickSubmit() {
            this.validateInput()
            if (this.fullname && 
                this.email && 
                this.whatsApp &&
                this.titleProject && 
                this.descProject) {
                    alert('Anda berhasil mendaftar!')
                }
        },
        checkValue(param) {
            if(param == 'fullname') {
                this.errorMsg.fullname = ''
            }
            if(param == 'email') {
                this.errorMsg.email = ''
            }
            if(param == 'whatsApp') {
                this.errorMsg.whatsApp = ''
            }
            if(param == 'titleProject') {
                this.errorMsg.titleProject = ''
            }
            if(param == 'descProject') {
                this.errorMessage = ''
            }
        }
        
    }
}
</script>

<style>
.registration-container {
    padding-top: 50px;
}
.btn-registration {
    background-color: #A4DEF9;
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