<template>
  <div class="skills-cont">
    <p class="title head">RELEVANT EXPERIENCE</p>
    <ul class="body">
      <li
        class="summary"
        v-for="(experience, index) in experiences"
        :key="index"
      >
        <div class="info-cont">
          <div class="left">
            
        <p class="name">{{ experience.name }} <span style="color: rgb(122, 122, 235);">( {{ experience.tools }})</span> </p>
            <P class="position">{{ experience.position }}</P>
            <div v-show="experience.duties.length > 0">
              <ul
                class="duty"
                v-for="(duty, index) in experience.duties"
                :key="index"
              >
               <li>{{ duty }}</li> </ul
              >
            </div>
            <!-- <P class="tools"> <span>Tools:</span> {{ experience.tools }}</P> -->
          </div>

          <div class="right">
            <P class="location">{{ experience.location }}</P>
            <P  class="tools">{{ experience.date }}</P>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      experiences: [
        {
          name: "ENDAVA - HYBRID",
          position: "Software Developer(Engineer)",
          tools: "Angular",
          location: "Slovenia",
          date: "Feb 2022 - Present",
          duties: [],
        },
        {
          name: "ELMIBIT - REMOTE",
          position: "FullStack Developer",
          tools: "Vue, CodeIgniter, PostgreSQL, Visual Studio, Linux",
          location: "Slovenia",
          date: "April 2021 - Jan 2022",
          duties: ["Developed business modules, presentations for senior management.",
            "Engaged in software development utilizing wide range of technological tools."],
        },
        {
          name: "DIPTOUR LIMITED",
          position: "Business Development/Lead, Travel Sales Consultant",
          tools: "HTML, CSS, React, Express and SQL",
          location: "Victoria Island, Lagos",
          date: "June 2016 – Dec 2019",
          duties: [
            "Created and designed contents for all social media handles and website every week",
          ],
        },
        {
          name: "HOUSE 53/54",
          position: "IT Assistant",
          tools: "HTML, CSS,Bootstrap, JavaScript, MsOffice, PHP and SQL.",
          location: "Victoria Island, Lagos",
          date: "Feb 2010 – Jan 2012",
          duties: [
            "Developed business cases, presentations for senior management.",
            "Engaged in software development utilizing wide range of technological tools.",
            "Provided clear and timely technical data required for design and specification of product.",
          ],
        },
        {
          name: "YOUTH EMPOWERMENT COMPUTERS",
          position: "Instructor",
          tools: "HTML, CSS, JavaScript, MsOffice",
          location: "Ikom, Cross River",
          date: "July 2008 – April 2009",
          duties: [
            "Taught courses on Desktop Publishing and Web Development.",
            "Removed malware and other threats from laptops and desktop systems.",
            "Designed computer literacy program for schools with specific programs, goals and assessments",
          ],
        },
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

.title,
.name {
  /* color: rgb(122, 122, 235); */
  color: red;
  font-weight: bold;
  margin-bottom: 0;
  margin-left: 1.3rem;
}
.head {
  color: green;
  margin-bottom: 0;
}
.body {
  
  margin-top: 0;
  font-size: 1rem;
  padding-left: 1.3rem;
}
.summary {
  /* padding: 0.3rem 0; */
  list-style: none;
}
.name {
  margin-left: 0;
}
.info-cont {
  font-size: 1rem;
  display: flex;
  justify-content: space-between;
}
span,
.location {
  font-weight: 700;
}

.left {
  flex: 3;
  font-size: .9rem;
}
.position {
    font-weight: 700;
  margin: 0.5rem 0 .3rem 0;
}
.duty {
  margin: 0.2rem;
  margin-left: 0;
  font-size: .8rem;
}
.right {
  font-size: .9rem;
  flex: 1;
  margin-right: 1rem;
}
.location {
     margin-bottom: 0px;
  color: red;
}
.tools {
  margin: 0.5rem 0 0.1rem 0;
}
</style>
