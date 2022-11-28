<template>
  <div id="app">
    <!-- <button @click="downloadWithCSS">Download PDF WITH CSS</button> -->

    <HeaderCv />
    <SummarySkills />
    <ExperienceCv />
    <EducationCv />
  </div>
</template>

<script>
import jsPDF from "jspdf";
import html2canvas from "html2canvas";
import HeaderCv from "./components/HeaderCv.vue";
import SummarySkills from "./components/SummarySkills.vue";
import ExperienceCv from "./components/ExperienceCv.vue";
import EducationCv from "./components/EducationCv.vue";

export default {
  name: "App",
  components: {
    HeaderCv,
    SummarySkills,
    ExperienceCv,
    EducationCv,
  },

  mounted() {
    // this.downloadWithCSS();
  },
  methods: {
    // downloadWithCSS() {
    //   html2pdf(this.$refs.document, {
    //     margin: 1,
    //     filename: "cv.pdf",
    //     image: { type: "jpeg", quality: 0.98 },
    //     html2canvas:{ dpi: 192, letterRendering: true },
    //     jsPDF:{ unit: "in", format:'letter', orientation:'landscape' },
    //   });
    // },
    // downloadWithCSS() {
    //   const doc = new jsPDF();
    //   /** WITH CSS */
    //   var canvasElement = document.createElement("canvas");
    //   html2canvas(this.$refs.content, { canvas: canvasElement }).then(function (
    //     canvas
    //   ) {
    //     const img = canvas.toDataURL("image/jpeg", 0.8);
    //     doc.addImage(img, "JPEG", 20, 20);
    //     doc.save("john.pdf");
    //   });
    // },
    downloadWithCSS() {
      window.html2canvas = html2canvas;
      var doc = new jsPDF("p", "pt", "a4");
      doc.html(document.querySelector("#app"), {
        callback: function (pdf) {
          pdf.save("mycv.pdf")
        }
      });
    },
  },
};
</script>

<style>
#app {
  /* width: 90%; */
  margin: auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  padding-bottom: 1rem;
  border-radius: 0.3rem;
  box-shadow: 0 3px 10px rgb(0 0 0 / 0.2);
  /* text-align: center;
  color: #2c3e50;
  margin-top: 60px; */


  height: 11in;  
  width: 8.5in;
}
</style>
