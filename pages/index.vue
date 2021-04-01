<template>
  <div class="container">
    <Sphere />
    <Paragraph
      v-for="content in contents"
      :id="content.id"
      :key="content.id"
      :content="content.content"
    />
  </div>
</template>

<script>
import Sphere from '@/components/Sphere'
import Paragraph from '@/components/Paragraph'

export default {
  components: { Sphere, Paragraph },
  data() {
    return {
      title: "Le P'tit Homme en Bleu",
      contents: [
        {
          id: 'home-1',
          content:
            "En France, on estimait en 2017, que le nombre d'individus atteint d'un trouble du spectre autistique s'élevait à environ 700 000 individus. Sur ces 700k individus, 600 000 étaient des adultes, et seulement 75 000 d'entre eux auraient été identifiés.",
        },
        {
          id: 'home-2',
          content:
            "En 2010, adultes et enfants confondus, seuls 75 000 individus étaient diagnostiqués comme atteint d'un trouble du spectre autistique. Moins de 20% de ces personnes bénéficiaient d'un accompagnement au sein d'une structure dédiée à l'autisme.",
        },
        {
          id: 'home-3',
          content:
            "Pourtant, tous s'accordent à le dire, plus le diagnostic est posé tôt, plus l'accompagnement sera fait rapidement, meilleures seront les chances pour ses enfants de s'intégrer et de vivre en communauté, en étant le plus indépendant possible.",
        },
        {
          id: 'home-4',
          content:
            "Malgré trois plans autisme qui n'ont guère apporté de progrès, il existe depuis le 6 avril 2018 une stratégie autisme. Sept personnes sont chargées d'améliorer le dépistage, la prise en charge et le suivi des personnes atteintes d'un trouble du spectre autistique. Pourtant, il est coutume de dire qu'il existe autant de forme d'autisme que d'individus atteint de cet handicap.",
        },
        {
          id: 'home-5',
          content:
            "C'est dans le but de vulgariser cet handicap, et si possible de venir en aide aux familles qui le vivent aux quotidiens, que nous avons décidé avec ma femme de créer ce Blog. Le but, essayer de centraliser les informations permettant de le détecter, de trouver les spécialistes capable de venir en aide, aider dans les démarches pour permettre à tous de pouvoir prétendre aux aides d'accompagnement pour payer les divers professionnels nécessaires pour un bon suvi.",
        },
        {
          id: 'home-6',
          content:
            "Impossible de tout faire dès le début, nous sommes nous-mêmes en plein dans l'apprentissage de ces différents chantiers pour l'accompagnement de notre fils Soann. Au fur et à mesure de notre apprentissage, ce Blog sera mis à jour pour vous faciliter la tâche, vous éviter les déboires ou difficultés que nous avons nous-même rencontrés, et vous faire gagner un temps précieux.",
        },
        {
          id: 'p-lastChild',
          content:
            'Nous vous souhaitons la Bienvenue pour suivre les aventures de Soann.',
        },
      ],
    }
  },
}
</script>

<style scoped>
#home-1 {
  margin-top: 100vh;
}
#p-lastChild {
  text-align: center;
}
</style>
