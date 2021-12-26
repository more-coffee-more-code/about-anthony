<template>
<!-- todo: animate content with Intersection observer -->
  <main class="home">
    <section-landing/>
    <section-skills/>
    <section-projects/>
    <section-contact/>
  </main>
</template>

<script>
// @ is an alias to /src
import SectionContact from '../components/section-contact'
import SectionLanding from '../components/section-landing'
import SectionSkills from '../components/section-skills'
import SectionProjects from '../components/section-projects'

export default {
  name: 'home',
  components: {
    SectionLanding,
    SectionSkills,
    SectionContact,
    SectionProjects
  }
}
</script>
