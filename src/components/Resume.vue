<template>
  <section class="section-resume">
    <TabGroup>
      <TabList class="tab-list">
        <Tab class="tab">簡介</Tab>
        <Tab class="tab">學歷／經歷</Tab>
        <Tab class="tab">主要作品</Tab>
        <Tab class="tab">技術能力</Tab>
        <Tab class="tab">自傳</Tab>
      </TabList>
      <TabPanels>
        <TabPanel class="tab-panel">Content 1</TabPanel>
        <TabPanel class="tab-panel">Content 2</TabPanel>
        <TabPanel class="tab-panel">Content 3</TabPanel>
        <TabPanel class="tab-panel">Content 4</TabPanel>
        <TabPanel class="tab-panel">Content 5</TabPanel>
      </TabPanels>
    </TabGroup>
  </section>
</template>

<!-- <script setup>
import { ref } from "vue"; // or other dependencies

const yourRef = ref(); // your reactive data
</script> -->

<script>
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from "@headlessui/vue";
export default {
  name: "Resume",
  components: {
    TabGroup,
    TabList,
    Tab,
    TabPanels,
    TabPanel,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.section-resume {
  max-width: 150rem;
  margin: 0 auto;
  padding: 2rem;
  border-radius: 0 0 15px 15px;
  background-color: #d0ebff;
}

.tab-list {
  display: flex;
  justify-content: center;
  margin: 2rem;
  gap: 2rem;
}

.tab {
  font-size: 2rem;
  font-weight: 600;
  padding: 1rem;
  background: #a5d8ff;
  border: none;
  border-radius: 12px;
  cursor: pointer;
}

.tab-panel {
  max-width: 130rem;
  margin: 0 auto;
  border: 1px solid black;
}
</style>
