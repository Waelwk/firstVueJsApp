
<script>
  export default {
  data() {
    return {
      nom : '',
      prenom : '',
      show: false
    }
  },
  methods: {
    
  }
}

</script>

<template> 
  <main>
   <p>Nom :</p>
  <input v-model="nom" placeholder="saisir votre nom" />
  <br>
  <p>Prenom :</p>
  <input v-model="prenom" placeholder="saisir votre prenom" /><br>
  <button v-on:click="show = !show">Click</button>
  <p  >Bonjour {{nom}} {{prenom}}</p>
  <p id="para" v-if="show">Bonjour {{nom}} {{prenom}}</p>

  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
