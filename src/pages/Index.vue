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

            <div class="timelineItem__wrapper clearfix">
              <timeline-item date="2018" title="SAWI">Intérvant pour la formation "Création de thème WordPress" de Procom</timeline-item>
              <timeline-item date="2016" title="8bitstudio">Hello</timeline-item>
              <timeline-item date="2014" title="Base7booking">Hello</timeline-item>
              <timeline-item date="2012" title="Suisseo">Hello</timeline-item>
              <timeline-item date="2009" title="Solugest">Hello</timeline-item>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="realisations" class="py-big">
      <div class="container">
        <div class="row">
          <div class="col-12 col-md-10 offset-md-1">
            <h1>Mes réalisations</h1>
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
import TimelineItem from '~/components/TimelineItem.vue'
import Checklist from '~/components/Checklist.vue'

import Skills from '~/data/Skills.json'

export default {
  data () {
    return {
      Skills
    }
  },
  metaInfo: {
    title: 'Hello, world!'
  },
  components: {
    Banner,
    TimelineItem,
    Checklist
  }
}
</script>

