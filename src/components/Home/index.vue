<template>
  <div class="container">
    <h1>Le P'tit Homme en Bleu</h1>
    <Login />
  </div>
  <p>En France, on estimait en 2017, que le nombre d'individus atteint d'un trouble du spectre autistique s'élevait à environ 700 000 individus. Sur ces 700k individus, 600 000 étaient des adultes, et seulement 75 000 d'entre eux seraient identifiés.</p>
    <p>En 2010, adultes et enfants confondus, seuls 75 000 individus étaient diagnostiqués comme atteint d'un trouble du spectre autistique. Moins de 20 % de ces personnes bénéficiaient d'un accompagnement au sein d'une structure dédiée à l'autisme.</p>
    <p>Pourtant, tous s'accordent à le dire, plus le diagnostic est posé tôt, plus l'accompagnement sera fait rapidement, meilleures seront les chances pour ses enfants de s'intégrer et de vivre en communauté, en étant le plus indépendant possible.</p>
    <p>Malgré trois plans autisme qui n'ont guère apporté de progrès, il existe depuis le 6 avril 2018 une stratégie autisme. Sept personnes sont chargées d'améliorer le dépistage, la prise en charge et le suivi des personnes atteintes d'un trouble du spectre autistique. Pourtant, il est coutume de dire qu'il existe autant de forme d'autisme que d'individus atteint de cet handicap.</p>
    <p>C'est dans le but de vulgariser cet handicap, et si possible de venir en aide aux familles qui le vivent aux quotidiens, que nous avons décidé avec ma femme de créer ce Blog. Le but, essayer de centraliser les informations permettant de le détecter, de trouver les spécialistes capables de venir en aide, aider dans les démarches pour permettre à tous de pouvoir prétendre aux aides d'accompagnement pour payer les divers professionnels nécessaires pour un bon suivi..</p>
    <p>Impossible de tout faire dès le début, nous sommes nous-mêmes en plein dans l'apprentissage de ces différents chantiers pour l'accompagnement de notre fils Soann. Au fur et à mesure de notre apprentissage, ce Blog sera mis à jour pour vous faciliter la tâche, vous éviter les déboires ou difficultés que nous avons nous-mêmes rencontrés, et vous faire gagner un temps précieux.</p>
    <p>Nous vous souhaitons la Bienvenue pour suivre les aventures de Soann.</p>
</template>

<script>
  import Login from './Login.vue';

  export default {
  components: { Login },
    name: 'Home'
  }
</script>

<style scoped>
  .container {
  display: flex;
  flex-wrap: nowrap;
  align-items: center;
  height: calc(100vh - 5rem);
  }

  h1 {
    font-family: 'Playfair Display', serif;
    font-size: 6rem;
    text-align: center;
    font-weight: bold;
    color: #060668;
    text-shadow: black 1px 1px 1px;
  }

  p {
  font-size: 1.5rem;
  color: #060668;
  margin: 1.5rem;
  margin-bottom: 0;
  line-height: 2rem;
  padding-bottom: 1rem;
  }
</style>