<template>
  <div class="about">
    <div class="about-container">
      <h2>About</h2>
      <p class="me">👋 Hi, I'm Mark!</p>
      <p>
      I am a software developer from kenya and Manchester united fan. I currently Live in kenya and due to my love for code
      I decided to create this platform for tailored course
       this course will contain best course from youtube and free online resourses
        repellendus eaque molestiae culpa ducimus, quia saepe dignissimos inventore ipsa doloribus odio dicta cumque,
        repellat voluptatem consectetur non corrupti ullam animi. Libero at eius dolores autem deserunt corporis
        delectus dolorum itaque, facilis harum commodi cum quos quis? Fugiat harum quasi ipsa vel itaque. Maiores
        fugiat nesciunt repudiandae saepe laudantium porro dignissimos tempora enim, iste fuga eos quidem id cum beatae
        architecto. Distinctio deserunt eius beatae dolorum soluta. Soluta repellendus molestiae sit praesentium, corrupti
        ab quaerat reprehenderit nemo libero quis explicabo consequatur optio deleniti, eius iure id velit, delectus ullam
      </p>
      <br />
      <div class="social">
        <a href="https://twitter.com/mark25floor" target="_blank">Twitter</a>
        <a href="https://github.com/mark-okoth" target="_blank">GitHub</a>
        <a href="https://www.linkedin.com/in/mark-okoth-1b514115b/" target="_blank">LinkedIn</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "about",
  data() {
    return {};
  }
};
</script>

<style scoped>
.about {
  height: 100vh;
  overflow-y: scroll;
  font-size: 1.2rem;
  font-weight: lighter;
  background: rgba(27, 2, 85, 0.767);
}

.about-container {
  margin: 20px 8vw;
}
::-webkit-scrollbar {
  width: 20px;
}
::-webkit-scrollbar-track {
  box-shadow: inset 0 0 5px grey;
  border-radius: 10px;
}
::-webkit-scrollbar-thumb {
  background: red;
  background: rgb(92, 92, 218);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: rgb(92, 92, 218);
}
h2 {
  margin-bottom: 20px;
}
.me {
  margin-bottom: 10px;
}
.social {
  display: flex;
}

a {
  text-decoration: none;
  padding: 15px 20px;
  background:rgb(28, 28, 95);
  margin-right: 20px;
  border-radius: 5px;
  transition: all 500ms ease-in-out;
}

a:hover{
  background: white;
  border: ipx solid lightslategrey;
  color: slateblue;
}
</style>
