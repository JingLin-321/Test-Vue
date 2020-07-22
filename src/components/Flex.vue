<template>
  <div class="container">
    <header>
      <h1>HEADER</h1>
    </header>
    <nav>
      <a href>HTML</a> |
      <a href>CSS</a> |
      <a href>JavaScript</a> |
      <a href>jQuery</a>
    </nav>
    <div class="mainItem">
      <div class="mainLeft">
        <section>
          <h1>AAAAA</h1>
          <p>James runs out. He makes a big pile of snow. He puts a big snowball on top. He adds a scarf and a hat. He adds an orange for the nose. He adds coal for the eyes and buttons.In the evening, James opens the door. What does he see?</p>
        </section>
        <article>
          <h1>BBBBB</h1>
          <p>James runs out. He makes a big pile of snow. He puts a big snowball on top. He adds a scarf and a hat. He adds an orange for the nose. He adds coal for the eyes and buttons.In the evening, James opens the door. What does he see?</p>
        </article>
      </div>
      <figure>
        <img src="../assets/1.jpg" width="100%" height="100%" />
        <figcaption>Fig1. - The Pulpit Pock, Norway.</figcaption>
      </figure>
    </div>
    <footer>
      <h1>FOOTER</h1>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  mounted() {},
  methods: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.container {
  width: 100%;
  height: 700px;
}
header,footer{
  height: 20%;
  display: flex;
  align-items: center;
  justify-content: center;
}
nav {
  height: 10%;
   display: flex;
  align-items: center;
  justify-content: center;
}
header,
nav,
.mainLeft,
figure,
footer {
  border: 1px solid black;
}
.mainItem {
  height: 50%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
</style>