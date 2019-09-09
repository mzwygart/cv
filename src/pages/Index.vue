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
            <ul>
              <li>HTML</li>
              <li>CSS</li>
              <li>JavaScript</li>
              <li>Performance</li>
              <li>SEO</li>
              <li>Accessibilité</li>
              <li>Newsletter</li>
              <li>Versioning</li>
              <li>Automatisation</li>
            </ul>
          </div>

          <div class="col-md-5">
            <h2>UI designer</h2>
            <ul>
              <li>Wireframe</li>
              <li>Workflow</li>
              <li>Prototype</li>
              <li>Design system</li>
              <li>Design mobile</li>
              <li>Accessibilité</li>
              <li>Design d'application web</li>
            </ul>
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

export default {
  metaInfo: {
    title: 'Hello, world!'
  },
  components: {
    Banner,
    TimelineItem,
  }
}
</script>

