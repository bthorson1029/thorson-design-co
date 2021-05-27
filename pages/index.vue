<template>
  <div class="container">
    <div class="hero-container">
      <h1 class="title">{{ heroMain }} </h1>
      <p class="subtitle"> {{heroSubText}} </p>
    </div>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'Thorson Design Co.',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'UI, UX, Development'
        }
      ]
    }
  },
  data() {
    return {
      heroMain: 'Thorson Design Co.',
      heroSubText: `Hi, my name is Bryce Thorson, and I'm a software designer and developer living and working in Atlanta.
	I help agencies, startups & businesses large and small bring their ideas to life through a refined design & development process.`
    }
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  & .hero-container {
    display: flex;
    flex-direction: column;
    max-width: calc(100vw - 6rem);
  }
  & .title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
  }
  & .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }
}



.links {
  padding-top: 15px;
}
</style>
