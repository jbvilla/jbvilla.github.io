<template>
<v-container>
  <h2>Socials</h2>
  <v-container>
    <br/>
    <v-row>
      <v-col>
        <v-icon size="60" @click="handleIconClick(linkedin)" >mdi-linkedin</v-icon>
      </v-col>
      <v-col>
        <v-icon size="60" @click="handleIconClick(github)" >mdi-github</v-icon>
      </v-col>
      <!--
      <v-col>
        <v-icon size="60" @click="handleIconClick(facebook)" >mdi-facebook</v-icon>
      </v-col>
      -->
      <v-col>
        <v-icon size="60" @click="handleIconClick(instagram)" >mdi-instagram</v-icon>
      </v-col>

    </v-row>
  </v-container>
</v-container>
</template>

<script>


export default {
  name: "SocialsSection",
  data() {
    return {
      facebook: 'https://www.facebook.com/profile.php?id=100008351674120',
      instagram: 'https://www.instagram.com/jonas_byle/',
      linkedin: 'https://www.linkedin.com/in/jonas-byl%C3%A9-942194285/',
      github: 'https://github.com/jbvilla'
    };
  },
  methods: {
    handleIconClick(icon) {
      window.open(icon, '_blank');
    },
  },
}
</script>


<style scoped>

</style>