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
                        <a class="nav-link text-light" @click="toPlatform">Platform</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-light" @click="toFlow">Flow User</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-light" @click="toFooter">Hubungi</a>
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
        this.teknologi = document.getElementById("teknologi");
        this.platform = document.getElementById("platform");
        this.flow = document.getElementById("flow");
        this.footer = document.getElementById("footer");
    },
    methods: {
        hideMenu() {
            let menuContainer = document.getElementById('navbarNav')
            menuContainer.classList.remove("show")
        },
        toServices() {
            this.services.scrollIntoView({
                behavior: 'smooth',
                block: 'start',
                inline: 'nearest',
            });
            this.hideMenu()
        },
        toBenefit() {
            this.benefit.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
            this.hideMenu()
        },
        toTeknologi() {
            this.teknologi.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
            this.hideMenu()
        },
        toPlatform() {
            this.platform.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
            this.hideMenu()
        },
        toFlow() {
            this.flow.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
            this.hideMenu()
        },
        toFooter() {
            this.footer.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
            this.hideMenu()
        },
    }

}
</script>

<style>
.navbar {
    background-color: #A4DEF9;
    font-size: 18px;
}


</style>