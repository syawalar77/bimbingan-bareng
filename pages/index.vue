<template>
    <div>
      <Header/>
      <Introduction/>
      <Services/>
      <Benefit/>
      <Teknologi/>
      <Platform/>
      <Flow/>
      <Registrasi/>
      <Footer/>
    </div>
</template>

<script>
import Header from '~/components/organisms/Header.vue'
import Introduction from '~/components/organisms/Introduction.vue'
import Services from '~/components/organisms/Services.vue'
import Benefit from '~/components/organisms/Benefit.vue'
import Teknologi from '~/components/organisms/Teknologi.vue'
import Platform from '~/components/organisms/Platform.vue'
import Flow from '~/components/organisms/Flow-user.vue'
import Registrasi from '~/components/organisms/Registrasi.vue'
import Footer from '~/components/organisms/Footer.vue'


export default {
  components: {
    Header,
    Introduction,
    Services,
    Benefit,
    Teknologi,
    Platform,
    Flow,
    Registrasi,
    Footer,
  }
}
</script>

<style>

</style>