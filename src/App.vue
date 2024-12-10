
<template>
  <h2>Full Name - {{fullName}}</h2>
</template>

<script>
  export default {
    name: 'App',
    components: {},
    data(){
      return {
        firstName: "Will",
        lastName: "Nice",
      }
    },
    computed : {
      fullName(){
        return `${this.firstName} ${this.lastName}`
      }
    }
  }
</script>



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
