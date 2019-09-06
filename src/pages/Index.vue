<template>
  <Layout>
    <Banner/>

    <section id="competences" class="container--overSized negativeTopMargin bg-white">
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

    <section class="bg-black">
      <div class="container">
        <div class="row">
          <div class="col-10 offset-md-1">
            <h1>Mon parcours</h1>
            <p>2018 Intérvant pour la formation "Création de thème WordPress" de Procom
    Depuis 2016 chez 8bitstudio</p>
          </div>
        </div>
      </div>
      
    
    </section>

    
    
    
    
    
    
    

    
  </Layout>
</template>

<script>
import Banner from '~/components/Banner.vue'

export default {
  metaInfo: {
    title: 'Hello, world!'
  },
  components: {
    Banner
  }
}
</script>

