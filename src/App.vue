<template>
<div class="layout">
<header-section></header-section>
  <label-panel></label-panel>
  <small-box-panel></small-box-panel>
  <main-panel></main-panel>
  <categrory-panel></categrory-panel>
</div>
</template>

<script>
import HeaderSection from './components/HeaderSection.vue'
import labelPanel from './components/LabelPanel.vue'
import mainPanel from './components/MainPanel.vue'
import categroryPanel from "@/components/CategroryPanel";
import smallBoxPanel from "@/components/smallBoxPanel";
export default {
  name: 'App',
  components: {
    HeaderSection,
    labelPanel,
    mainPanel,
    categroryPanel,
    smallBoxPanel
  },
  }
</script>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0px;
}

body {
  background-color: rgba(159, 173, 193, 0.7);
}

.smallBoxPanel {
  background-color: #f5f5f5;
}

.layout {
box-sizing: border-box;


  display: grid;
  grid-template-rows: 1.7fr 1.7fr 5fr 1fr  ;
  grid-template-columns: 2fr ;
  grid-template-areas:
    "headerSection"
    "labelPanel"
    "smallBoxPanel"
    "mainPanel"
  "categroryPanel"


}

.headerSection {
  grid-area: headerSection;
  background-color: #0078D5;
}

.labelPanel {
  grid-area: labelPanel;
  background-color: rgb(240, 244, 246);
}

.mainPanel {
  grid-area: mainPanel;
  background-color: rgb(25, 148, 148);
}
.categroryPanel {
  background-color: rgba(146, 131, 157, 0.84);
}



</style>
