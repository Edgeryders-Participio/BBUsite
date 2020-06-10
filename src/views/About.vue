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
        `Babel Between Us is a cartographic visualization of a collaboratively created fiction, 
          exploring the uncharted waters between collaboration, language and ethnography.`,
        `A group of 18 writers collectively improvise a story on an online forum during an extensive amount of time. 
          The resulting fiction is analyzed by a team of ethnographers and presented as an interactive map. 
          This map is then presented back to the group throughout the process. 
          The final map is presented in itself as an entry point for the general public to experience the work.`,
        `The project is currently ongoing, follow us on twitter for recurring update.`,
        `If you have any questions contact us on our forum, at team [at] bbu.world.`
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