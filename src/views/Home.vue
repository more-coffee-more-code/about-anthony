<template>
<!-- todo: animate content with Intersection observer -->
  <div class="home">
    <section-landing/>
    <section-skills/>
    <section-contact/>
  </div>
</template>

<script>
// @ is an alias to /src
import SectionContact from '../components/section-contact'
import SectionExperienceDev from '../components/section-experience-dev'
import SectionExperienceQa from '../components/section-experience-qa'
import SectionLanding from '../components/section-landing'
import SectionSkills from '../components/section-skills'

export default {
  name: 'home',
  components: {
    SectionLanding,
    SectionSkills,
    SectionExperienceDev,
    SectionExperienceQa,
    SectionContact
  }
}
</script>
