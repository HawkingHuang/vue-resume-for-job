<template>
  <section class="section-header">
    <div>
      <!-- <img
        src="../assets/img/P_20230228_112634.jpg"
        alt="profile-picture"
        class="profile-picture"
      /> -->
    </div>
    <div>
      <h2 class="name">{{ name }}</h2>
      <!-- <p class="title">{{ title }}</p> -->
    </div>
    <div>
      <ul class="personal-info">
        <li class="info-list">
          <ion-icon name="man-outline"></ion-icon>
          <p>生日：{{ birthday }}</p>
        </li>
        <li class="info-list">
          <ion-icon name="call-outline"></ion-icon>
          <p>手機：{{ phone }}</p>
        </li>
        <li class="info-list">
          <ion-icon name="mail-outline"></ion-icon>
          <p>email：{{ email }}</p>
        </li>
        <li class="info-list-a">
          <ion-icon name="logo-linkedin"></ion-icon>
          <a :href="linkedin" class="linkedin-link">LinkedIn</a>
        </li>
        <li class="info-list-a">
          <ion-icon name="logo-facebook"></ion-icon>
          <a :href="facebook" class="facebook-link">Facebook</a>
        </li>
        <li class="info-list-a">
          <ion-icon name="logo-github"></ion-icon>
          <a :href="github" class="github-link">GitHub</a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      name: "Hawking Huang",
      title: "Software Engineering Intern",
      birthday: "1994/09/30",
      phone: "0911-873906",
      email: "math0915@gmail.com",
      linkedin: "https://www.linkedin.com/in/hawking-huang-80b270268/",
      facebook: "https://www.facebook.com/profile.php?id=100000471647087",
      github: "https://github.com/HawkingHuang",
    };
  },
};
</script>

<style scoped>
.section-header {
  color: #fff;
  max-width: 150rem;
  margin: 5rem auto 0 auto;
  padding: 2rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  justify-items: center;
  align-items: center;
  border-radius: 15px 15px 0 0;
  background-color: #1c7ed6;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.name {
  font-size: 4.4rem;
}

.title {
  font-size: 2.4rem;
}

.personal-info {
  display: grid;
  grid-template-columns: 1fr;
  gap: 0.8rem;
  list-style-type: none;
  font-size: 1.6rem;
}

.info-list {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  font-weight: 600;
}

.info-list-a {
  display: flex;
  gap: 0.5rem;
  font-weight: 600;
}

.linkedin-link,
.facebook-link,
.github-link {
  text-decoration: none;
  color: #fff;
}

.profile-picture {
  width: 20rem;
  height: 20rem;
  border-radius: 50%;
  box-shadow: 0 2.4rem 4.8rem rgba(0, 0, 0, 0.075);
}
</style>
