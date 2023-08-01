<template>
  <v-container>
    <h2>About</h2>
    <v-container>
      <v-row>
        <v-col cols="2" />
        <v-col align="center" cols="8">
          <p>
            I am {{age}} years old and currently pursuing my Master's degree in Computer Science at Ghent University. I have a passion for programming and enjoy taking on new challenges. My curiosity knows no bounds and motivates me to independently explore emerging technologies and gain the expertise, which I then eagerly put into practice. In addition to my enthusiasm for individual projects, I also love working with groups on large-scale projects. Besides programming, I find joy in activities such as hiking, mountain biking, meeting up with friends and exploring new places.
          </p>
        </v-col>
      </v-row>
    </v-container>
  </v-container>

</template>

<script>
export default {
  name: "AboutSection",
  data() {
    return {
      birthdate: new Date(2002, 8, 29),
    };
  },
  computed: {
    age() {
      const today = new Date();
      const age = today.getFullYear() - this.birthdate.getFullYear();
      const month = today.getMonth() - this.birthdate.getMonth();
      if (month < 0 || (month === 0 && today.getDate() < this.birthdate.getDate())) {
        return age - 1;
      }
      return age;
    },
  },
}
</script>

<style scoped>

</style>