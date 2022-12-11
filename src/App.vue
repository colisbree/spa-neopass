<template>

  <header>
    <navbar></navbar>
  </header>

  <main>
    <div class="container px-4 py-8 mx-auto">
      <section-accueil></section-accueil>
      <section-quest-ce-que></section-quest-ce-que>
      <section-intersticiel-1></section-intersticiel-1>
      <section-en-chiffres></section-en-chiffres>
    </div>
    <section-contact></section-contact>
  </main>
  <footer>
    <section-footer></section-footer>
  </footer>

</template>

<script setup>
  import navbar from "./components/Navbar.vue"
  import SectionAccueil from "./components/SectionAccueil.vue"
  import sectionQuestCeQue from "./components/SectionQuestCeQue.vue"
  import SectionIntersticiel1 from "./components/SectionIntersticiel1.vue"
  import sectionEnChiffres from "./components/SectionEnChiffres.vue"
  import sectionContact from "./components/SectionContact.vue"
  import SectionFooter from "./components/Footer.vue"
</script>

<style scoped>

</style>
