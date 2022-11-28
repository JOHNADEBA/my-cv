<template>
  <header>
    <div class="head-cont">
      <div class="name-cont">
        <p class="name">JOHN ADEBA</p>
        <p class="title">SOFTWARE DEVELOPER</p>
      </div>
      <div>
        <p class="phone">Phone: +38641286702</p>
        <!-- <div class="links-cont">
          <a href="https://devjayprojects.netlify.app/" target="_blank"
          >projects</a
        >
          <a href="https://www.linkedin.com/in/john-adeba-794738117/" target="_blank"
          >LinkedIn</a
        >

          <a href="https://github.com/JOHNADEBA" target="_blank">github</a>
        </div> -->
      </div>

      <div >
        <h4>Address: Ljubljana, Slovenia, 1000</h4>
        <h4>E-mail: adebajohn@gmail.com</h4>
      </div>
    </div>
    <div class="lin-cont">
      <p class="lin">Projects: <a href="https://devjayprojects.netlify.app/"></a> https://devjayprojects.netlify.app/</p>
      <p class="lin"> LinkedIn: <a href=" https://www.linkedin.com/in/john-adeba-794738117/"></a> https://www.linkedin.com/in/john-adeba-794738117/</p>
      <p class="lin">github: <a href="https://github.com/JOHNADEBA"></a> https://github.com/JOHNADEBA</p>
    </div>
  </header>
</template>

<style scoped>
h4 {
  margin: 0.3rem 0;
}
header {
  border-bottom: 0.1rem solid rgba(77, 75, 75, 0.3);
}
.head-cont {
  font-weight: bold;
  margin: 0;
  text-align: center;
  color: green;
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-size: 1rem;
}

.name {
  margin: 0;
  font-size: 2rem;
}
.title {
  margin: 0.5rem 0 0 0;
  font-size: 1rem;
}
.phone {
  margin-top: 0;
}
.lin-cont{
font-weight: bold;
  padding: .3rem 0;
  font-size: 0.7rem; 
   display: flex;
  justify-content: space-around;
  align-items: center;
}
.lin {
  color: rgb(104, 104, 248);
  margin: 0 .3rem;
}
/* .links-cont {
  display: flex;
  justify-content: space-around;
  align-items: center;

 
}
.links-cont a {
  color: rgb(104, 104, 248);
  text-decoration: none;
}
a:nth-child(2) {
  padding: 0 0.5rem;
  color: rgb(250, 73, 73);
}
.links-cont a:hover {
  color: rgb(255, 142, 142);
  opacity: 0.5;
} */
</style>
