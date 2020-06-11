<template>
  <div class="about">
    <img
      src="https://bbu.world/uploads/babelbetweenus/original/1X/d148a656cefb8fec73359e0a16e50fcac57628d3.jpeg"
    />
    <p v-for="(about, index) in abouts" :key="index">{{about}}</p>
    <h2>Image by Sune Skote, Fornvårdar, 1950</h2>
  </div>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      abouts: [
        `Babel Between Us is a cartographic visualization of a collaboratively created world, 
          exploring the uncharted waters between collaboration, fiction and ethnography.`,
        `A group of 18 writers collectively improvise a story on an online forum during an extensive amount of time. 
          The resulting fiction is analyzed by a team of ethnographers and presented as an interactive map. 
          This map is then presented back to the group throughout the process. 
          The final map is presented in itself as an entry point for the general public to experience the work.`,
        `The project is currently ongoing. This site lets you read the texts produced by the writers, the ethnographic part will be added eventually. Follow us on <a href="https://twitter.com/babelbetweenus">twitter</a> for recurring updates.`,
        `If you have any questions contact us on <a href="https://bbu.world/">our forum</a>, or at team [at] bbu.world.`,
        `Babel between us is created by Ola Claësson, Jennifer McGeachie, Filip Nyström, Alja Gudžević, Hugi Ásgeirsson and Jakob Skote, in collaboration with <a href="https://www.blivande.com/">Blivande</a> and <a href="https://edgeryders.eu/">Edgeryders</a>, and with funding from <a href="https://www.konstnarsnamnden.se/Kulturbryggan/">Kulturbryggan</a>.`
      ]
    };
  }
};
</script>

<style scoped>
.about {
  margin: 20px 0px;
}
img {
  width: 95%;
}
p {
  text-align: left;
  margin-bottom: 40px;
  font-size: 18px;
  line-height: 1.6em;
}
h2 {
  text-align: left;
  white-space: pre-wrap;
  color: #8a8a8a;
  font-weight: 400;
  font-style: italic;
  line-height: 1.3em;
  font-size: 12px;
  text-transform: none;
  text-decoration: none;
  letter-spacing: 0.02em;
}
</style>
