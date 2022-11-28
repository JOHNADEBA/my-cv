<template>
  <div class="skills-cont">
    <p class="title">SUMMARY OF QUALIFICATIONS</p>
    <ul class="body">
      <li class="summary" v-for="(summary, index) in summaries" :key="index">
        {{ summary }}
      </li>
    </ul>

    <p class="title">SOFT SKILLS</p>
    <ul class="body soft-skill">
      <li class="soft" v-for="(soft, index) in softSkills" :key="index">
        {{ soft }}
      </li>
    </ul>

    <p class="title">TECHNICAL SKILLS</p>
    <ul class="body soft-skill">
      <li
        class="technical"
        v-for="(technical, index) in technicalSkills"
        :key="index"
      >
        {{ technical }}{{ index < technicalSkills.length -1 ? ' |' : '' }}
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      summaries: [
        "JSON and RESTful web services.",
        " Database management (Relational databases and NoSQL databases).",

        "Excellent understanding of Modern day technologies.",

        "Production experience with React, Vue, Angular, PHP and Nodejs.",

        "Experience working remotely, building Applications with distributed international teams.",
      ],
      softSkills: [
        "Communication",
        "Data Analysis",
        "Project Management ",
        "Team player",
      ],
      technicalSkills: [
        "HTML",
        "CSS",
        "SASS",
        "JavaScript",
        "React",
        "Vue",
        "Angular",
        "PHP",
        "CodeIgniter",
        "JAVA",
        "Node js",
        "Express",
        "MongoDB",
        "PostgreSQL",
        "MySQL",
      ],
    };
  },
};
</script>

<style scoped>
.skills-cont {
  margin: 1rem 1.5rem;
  font-size: 1rem;
}
.title {
  color: green;
  font-weight: bold;
  margin-bottom: 0;
  margin-left: 1.3rem;
  margin-top: -.3rem;
}
.body {
  margin-top: .3rem;
}
.summary {
  font-size: .8rem;
  padding: 0.1rem 0;
}
.soft-skill {
  display: flex;
  flex-wrap: wrap;
  padding-left: 1.4rem ;
}
.soft {
  font-size: .8rem;
  list-style: none;
  margin-right: 2rem;
}
.technical {
  font-size: .8rem;
  list-style: none;
  margin-bottom: .2rem;
  margin-right: .3rem;
}
</style>
