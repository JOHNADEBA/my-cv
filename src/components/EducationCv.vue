<template>
  <div class="skills-cont">
    <p class="title head">EDUCATION</p>
    <div class="info-cont body">
      <div class="left">
        <p class="duty">Institut Superieur De Formation Professionelle</p>
        <p class="duty">Bachelor of Science: Computer Science</p>
      </div>
      <div class="right">
        <p class="location">Cotonou, Repubpque Du Benin</p>
        <p class="duty">Sept 2012 – Aug 2016</p>
      </div>
    </div>

    <p class="title head">RELEVANT CERTIFICATION</p>
    <div class="info-cont body">
      <div class="left">
        <p class="duty">National Institute of Information Technology</p>
        <p class="duty">JAVA</p>
      </div>
      <div class="right">
        <p class="location">Lagos</p>
        <p class="duty">Dec 2017 - Nov 2019</p>
      </div>
    </div>

    <div class="last-cont">
      <div>
        <p class="title head">LANGUAGE</p>
        <p class="body duty">English(Native) | Slovenian(Basic)</p>
      </div>
      <div>
        <p class="title head">INTEREST</p>
        <p class="body duty">
          Coding | Surfing the net | Football | Travelling | Project with a Team
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.skills-cont {
  margin: 0rem 1.5rem;
  font-size: 1rem;
}

.title,
.name {
  color: red;
  font-weight: bold;
  margin-bottom: 0;
  margin-left: 1.3rem;
}
.head {
  color: green;
  margin-bottom: 0.2rem;
  margin-top: 0.5rem;
}
.body {
  font-size: 0.9rem;
  padding-left: 1.3rem;
}
.summary {
  list-style: none;
}
.name {
  font-size: 1.3rem;
  margin-left: 0;
}
.info-cont {
  display: flex;
  justify-content: space-between;
}
span,
.location {
  font-weight: 700;
}
.location {
  margin: 0px;
  color: red;
}
.left {
  flex: 3;
}
.right {
  flex: 1;
  margin-left: -7rem;
}
.duty {
  margin: 0.2rem;
  margin-left: 0;
  font-size: 0.9rem;
}
.last-cont {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
</style>
