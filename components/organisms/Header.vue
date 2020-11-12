<template>
    <nav class="navbar navbar-expand-lg navbar-light fixed-top">
        <div class="container">

            <a class="navbar-brand text-light" href="#">bimbinganbareng.com</a>
            <button 
                class="navbar-toggler" 
                type="button" 
                data-toggle="collapse" 
                data-target="#navbarNav" 
                aria-controls="navbarNav" 
                aria-expanded="false" 
                aria-label="Toggle navigation"
            >
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item">
                        <a class="nav-link text-light" @click="toServices">Layanan</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-light" @click="toBenefit">Keuntungan</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-light" @click="toTeknologi">Teknologi</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-light" >Disabled</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-light" @click="toPlatform">Platform</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-light" @click="toFlow">Flow User</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-light" >Hubungi</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            services: "",
            benefit: "",
            teknologi: "",
            platform: "",
            flow: "",
        }
    },
    mounted() {
        this.services = document.getElementById("services");
        this.benefit = document.getElementById("benefit");
        this.teknolgi = document.getElementById("teknologi");
        this.platform = document.getElementById("platform");
        this.flow = document.getElementById("flow");

    },
    methods: {
        toServices() {
            this.services.scrollIntoView({
                behavior: 'smooth',
                block: 'start',
                inline: 'nearest',
            });
        },
        toBenefit() {
            this.benefit.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
        },
        toTeknologi() {
            this.teknologi.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
        },
        toPlatform() {
            this.platform.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
        },
        toFlow() {
            this.flow.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
        },
    }

}
</script>

<style>
.navbar {
    background-color: #A4DEF9;
    font-size: 18px;
    font-family: nunito;

}


</style>