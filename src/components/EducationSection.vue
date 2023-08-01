<template>
  <v-container>
    <h2>Education</h2>
    <v-container>
      <v-row>
        <v-col>
          <h3>{{ highSchool.degree }}</h3>
          <p>{{ highSchool.school }}</p>
          <p>{{ highSchool.duration }}</p>
        </v-col>
      </v-row>
    </v-container>
    <v-container>
      <v-row>
        <v-col v-for="(educationItem, index) in educationHistory" :key="index" cols="6">
          <h3>{{ educationItem.degree }}</h3>
          <p>{{ educationItem.school }}</p>
          <p>{{ educationItem.duration }}</p>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {
  name: "EducationSection",
  data() {
    return {
      educationHistory: [
        {
          degree: 'Bachelor of Science in Computer Science',
          school: 'Ghent University',
          duration: 'Sep 2020 - Jul 2023',
        },
        {
          degree: 'Master of Science in Computer Science',
          school: 'Ghent University',
          duration: 'Sep 2023 - current',
        },
      ],
      highSchool: {
        degree: 'Industrial science (8h mathematics)',
        school: 'Don Bosco Halle (High School)',
        duration: 'Sep 2014 - Jul 2020',
      },
    };
  },
}
</script>

<style scoped>

</style>