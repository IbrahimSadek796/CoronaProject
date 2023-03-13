<script setup>
// header
import NavHead from './components/nav-header.vue'

// component
import CorHome from './components/corona-components/coro-home.vue'
import CorAbout from './components/corona-components/cor-about.vue'
import CorTrans from './components/corona-components/cor-transmission.vue'
import CorSymptoms from './components/corona-components/cor-symptoms.vue'
import CorPrevention from './components/corona-components/cor-prevention.vue'
import CorProtact from './components/corona-components/cor-protact.vue'
import CorSteps from './components/corona-components/cor-steps.vue'
import CorTreat from './components/corona-components/cor-treat.vue'
import CorDont from './components/corona-components/cor-dont.vue'
import CorLatest from './components/corona-components/cor-latest.vue'
import CorQuestion from './components/corona-components/cor-question.vue'

// footer
import CorFooter from './components/cor-footer.vue'
</script>

<template>
  <header>
    <NavHead/>
  </header>

  <body class="bg-light">
    <CorHome/>
    <CorAbout/>
    <CorTrans/>
    <CorSymptoms/>
    <CorPrevention/>
    <CorProtact/>
    <CorSteps/>
    <CorTreat/>
    <CorDont/>
    <CorQuestion/>
    <CorLatest/>
  </body>

  <footer>
    <CorFooter/>
  </footer>
</template>

<style scoped>


</style>
