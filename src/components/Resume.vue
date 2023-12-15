<template>
  <section class="section-resume">
    <TabGroup>
      <TabList class="tab-list">
        <Tab class="tab">簡介</Tab>
        <Tab class="tab">學經歷</Tab>
        <Tab class="tab">主要作品</Tab>
        <Tab class="tab">技術能力</Tab>
        <Tab class="tab">自傳</Tab>
      </TabList>
      <TabPanels>
        <TabPanel class="tab-panel">Content 1</TabPanel>
        <TabPanel class="tab-panel">
          <div class="exp-section">
            <h2 class="exp-section-title">學歷</h2>
            <p class="exp-section-text">國立高雄師範大學 英語學系</p>
          </div>
          <div class="exp-section">
            <h2 class="exp-section-title">經歷</h2>
            <p class="exp-section-text">
              興巨資訊股​份有限公司 - Meta 筆譯專員（2019 年 6 月至 2022 年 3
              月）
            </p>
            <p class="exp-section-text-detail">
              - 主要負責處理 Meta（前身為 Facebook）
              的文件翻譯，領域涵蓋使用說明、遊戲、部落格、行銷等。
            </p>
            <p class="exp-section-text">
              自由譯者（2022 年 4 月至 2023 年 8 月）
            </p>
            <p class="exp-section-text-detail">- 全職擔任自由譯者</p>
            <p class="exp-section-text">
              創科資訊股份有限公司 - 實習生（2023 年 9 月至 2023 年 10 月）
            </p>
            <p class="exp-section-text-detail">
              - 實習過程前兩週主要是對 Git、Figma、Nginx、Ubuntu
              等技術有初步的認識，並完成相關作業。過程中也因為得知該公司主要是使用
              Vue 和 Laravel 進行開發，因此在原本就有 JS 基礎的情況下開始學習
              Vue，並於 10
              月左右開始參與該公司「Monospace」共同工作空間的會員系統維護工作。
            </p>
          </div>
        </TabPanel>
        <TabPanel class="tab-panel">
          <h2 class="portfolio">
            <ion-icon name="caret-forward-outline"></ion-icon
            ><ion-icon name="caret-forward-outline"></ion-icon
            ><a href="http://localhost:8085/" class="portfolio-link"
              >點擊檢視作品</a
            ><ion-icon name="caret-back-outline"></ion-icon
            ><ion-icon name="caret-back-outline"></ion-icon>
          </h2>
          <div class="portfolio-intro">
            <div class="portfolio-intro-section">
              <h3 class="portfolio-intro-title">作品簡介</h3>
              <p>
                Traditional Chinese Checker
                是一項繁體中文錯字檢查工具，之所以想開發此工具是因為之前從事翻譯工作時，交稿前都會進行錯字校正，但由於市面上中文語系的相關工具寥寥可數，加上介面和功能相對陽春，因此當初擬定題目時，才有了開發此工具的念頭產生。
              </p>
            </div>
            <div class="portfolio-intro-section">
              <h3 class="portfolio-intro-title">技術與特色</h3>
              <p>
                Vue.js <ion-icon name="logo-vue"></ion-icon> + Firebase
                <ion-icon name="logo-firebase"></ion-icon> （實作 Router 與
                Vuex）
              </p>
              <p>具備 RWD 響應式網頁設計概念</p>
              <p>
                針對主要路由使用 KeepAlive 和 Transition
                元件，使用者轉至其他路由並返回時，輸入的內容將會保留，且過程中會有動畫效果
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
  margin: 2rem;
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

/* Experience */
.exp-section {
  padding: 1rem;
}

.exp-section-title {
  font-size: 2.4rem;
  padding: 0.5rem;
  margin: 0.5rem;
  color: #1c7ed6;
  text-align: left;
}

.exp-section-text {
  font-size: 1.8rem;
  font-weight: bold;
  padding: 0.5rem;
  margin: 0.5rem;
  line-height: 1.8;
  text-align: left;
}

.exp-section-text-detail {
  color: #343a40;
  font-size: 1.6rem;
  font-weight: bold;
  padding: 0.5rem;
  margin: 0.5rem;
  line-height: 1.5;
  text-align: left;
}

/* Portfolio */
.portfolio {
  padding: 2rem;
}

.portfolio-link {
  color: #fff;
  background-color: #1c7ed6;
  padding: 1rem;
  margin: 1rem auto;
  text-decoration: none;
  border: none;
  border-radius: 5px;
}

.portfolio-intro-section {
  margin: 1.5rem auto;
}

.portfolio-intro-title {
  font-size: 2.4rem;
  margin: 0.5rem;
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
