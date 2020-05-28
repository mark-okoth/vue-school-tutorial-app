<template>
  <div class="about">
    <div class="about-container">
      <h2>About</h2>
      <p class="me">👋 Hi, I'm Mark!</p>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque ullam numquam mollitia,
        delectus temporibus provident? Sunt voluptatum veniam voluptatem debitis, quam earum laboriosam at
        distinctio impedit magnam repellendus placeat consequatur ea totam aliquam, praesentium assumenda ipsum eveniet!
        Praesentium est ipsum qui nulla, labore recusandae quas tempore vel alias, odit expedita et excepturi perspiciatis.
        Distinctio corrupti natus aperiam odio, totam repellat reprehenderit molestias, atque dolorum, labore magni ex.
        Tempora similique eius soluta commodi rerum quasi assumenda fuga ad deserunt mollitia dicta modi sed tenetur
        ipsam, libero accusantium suscipit eum corrupti repudiandae iure, officia temporibus, quos non minus? Iure
        quibusdam repudiandae nobis tempora fuga ex. Ex at, est quis consectetur molestiae blanditiis quaerat iure unde
        delectus accusamus minima veniam perferendis expedita tenetur reprehenderit asperiores repellat odit sint
        provident nihil pariatur deleniti odio voluptatum. Dolorem sint nisi minus veniam placeat id similique
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
  height: 10vh;
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