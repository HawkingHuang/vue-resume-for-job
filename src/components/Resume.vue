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
        <TabPanel class="tab-panel">
          <h2>
            <ion-icon name="caret-forward-outline"></ion-icon
            ><ion-icon name="caret-forward-outline"></ion-icon
            ><a href="http://localhost:8085/" class="portfolio">點擊檢視作品</a
            ><ion-icon name="caret-back-outline"></ion-icon
            ><ion-icon name="caret-back-outline"></ion-icon>
          </h2>
          <div class="portfolio-intro">
            <div class="portfolio-intro-section">
              <h3 class="portfolio-intro-title">作品簡介</h3>
              <p>
                Traditional Chinese
                Checker是一項繁體中文錯字檢查工具，之所以想開發此工具是因為之前從事翻譯工作時，交稿前都會進行錯字校正，但由於市面上中文語系的相關工具寥寥可數，加上介面和功能相對陽春，因此當初擬定題目時，才有了開發此工具的念頭產生。
              </p>
            </div>
            <div class="portfolio-intro-section">
              <h3 class="portfolio-intro-title">技術與特色</h3>
              <p>
                Vue.js <ion-icon name="logo-vue"></ion-icon> + Firebase
                <ion-icon name="logo-firebase"></ion-icon> （實作 Router 與
                Vuex）
              </p>
              <p>具備RWD響應式網頁設計概念</p>
              <p>
                針對主要路由使用KeepAlive和Transition元件，使用者在轉至其他路由並返回時，其輸入的內容將會保留，且過程中會有動畫效果
              </p>
              <p>
                註冊與登入頁面實作正規表達式驗證，使用者在輸入不符合格式的帳號密碼時，系統將會給予提示
              </p>
              <p>
                使用者可於登入後前往「<ion-icon
                  name="add-circle-outline"
                ></ion-icon
                >Custom」自訂欲檢查之錯字，該詞彙將會於「<ion-icon
                  name="checkmark-circle-outline"
                ></ion-icon
                >Check」頁面檢查時一併校正。未來若不想再檢查該詞彙，可前往個人頁面的「MyWords」區塊點擊該詞彙，接著點擊垃圾桶按鈕<ion-icon
                  name="trash-outline"
                ></ion-icon
                >進行刪除
              </p>
            </div>
          </div>
        </TabPanel>
        <TabPanel class="tab-panel">Content 4</TabPanel>
        <TabPanel class="tab-panel">Content 5</TabPanel>
      </TabPanels>
    </TabGroup>
  </section>
</template>

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

<style scoped>
.section-resume {
  max-width: 150rem;
  margin: 0 auto;
  padding: 2rem;
  border-radius: 0 0 15px 15px;
  background-color: #fff;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.tab-list {
  display: flex;
  justify-content: center;
  margin: 3rem;
  gap: 2rem;
}

.tab {
  font-size: 2.4rem;
  font-weight: 600;
  padding: 1rem;
  background: #fff;
  border: none;
  border-radius: 12px;
  cursor: pointer;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
}

.tab-panel {
  max-width: 130rem;
  height: 50rem;
  margin: 0 auto;
  background: #fff;
  border: none;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
}

.tab-panel h2 {
  padding: 2rem;
}

.portfolio {
  color: #fff;
  background-color: #1c7ed6;
  padding: 1rem;
  margin: 1rem auto;
  text-decoration: none;
  border: none;
  border-radius: 5px;
}

.portfolio-intro-section {
  margin: 2rem auto;
}

.portfolio-intro-title {
  font-size: 2.4rem;
  margin: 1rem;
  color: #1c7ed6;
}

.portfolio-intro p {
  width: 80%;
  margin: 0.5rem auto;
  font-size: 1.8rem;
  font-weight: bold;
  line-height: 1.8;
}
</style>
