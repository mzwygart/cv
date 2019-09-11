<template>
  <Layout>
    <Banner/>

    <section id="competences" class="container--overSized negativeTopMargin bg-white py-big">
      <div class="container">
        <div class="row">
          <div class="col-md-10 offset-md-1">
            <h1>Mes compétences</h1>
          </div>
          <div class="col-md-5 offset-md-1">
            <h2>Développeur front-end</h2>

            <Checklist :items="Skills.developerSkills" />
          </div>

          <div class="col-md-5">
            <h2>UI designer</h2>

            <Checklist :items="Skills.designerSkills" />
          </div>
        </div>
      </div>
    </section>

    <section id="parcours" class="bg-black py-big">
      <div class="container">
        <div class="row">
          <div class="col-12 col-md-10 offset-md-1">
            <h1>Mon parcours</h1>

            <Timeline :entries="ProfessionalExperiences.entries" />

          </div>
        </div>
      </div>
    </section>

    <section id="realisations" class="py-big">
      <div class="container">
        <div class="row">
          <div class="col-12 col-md-10 offset-md-1">
            <h1>Mes réalisations</h1>

            <Portfolio :projects="Projects.entries" />
          </div>
        </div>
      </div>
    </section>

    <section id="contact" class="py-big">
      <div class="container">
        <div class="row">
          <div class="col-12 col-md-10 offset-md-1">
            <h1>Me contacter</h1>
          </div>
        </div>
      </div>
    </section>
    
    
    
    
    
    

    
  </Layout>
</template>

<script>
import Banner from '~/components/Banner.vue'
import Checklist from '~/components/Checklist.vue'
import Timeline from '~/components/Timeline.vue'
import Portfolio from '~/components/Portfolio.vue'

import Skills from '~/data/Skills.json'
import ProfessionalExperiences from '~/data/ProfessionalExperiences.json'
import Projects from '~/data/Projects.json'

export default {
  data () {
    return {
      Skills,
      ProfessionalExperiences,
      Projects
    }
  },
  metaInfo: {
    title: 'Hello, world!'
  },
  components: {
    Banner,
    Checklist,
    Timeline,
    Portfolio
  }
}
</script>

