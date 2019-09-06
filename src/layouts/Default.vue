<template>
  <div class="app">
      <header role="banner" class="siteHeader bg-black">
        <div class="container">
          <div class="row align-items-end">
            <div class="col-md-5 offset-md-1">
              <h1 class="siteHeader__name nosep">Mathieu Zwygart</h1>
            </div>

            <div class="col-md-6">
              <nav role="navigation">
                <Menu />
              </nav>
            </div>
          </div>
          
    
          
        </div>
    </header>

    <main role="main">
      <slot/>
    </main>
  </div>
</template>

<style lang="scss">
.siteHeader {
  padding: 5rem 0;

  &__name {
    font-size: 1.8rem;
    font-weight: 700;
    margin: 0;
  }
}
</style>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<script>
import Menu from '~/components/Menu.vue'

export default {
  components: {
    Menu
  }
}
</script>