<template>
  <div class="hello">
    <div class="menu">
      <div class="menu-item">
        <div class="menu-text">Academic</div>
      </div>

      <div class="menu-item">
        <div class="menu-text">Hobbies</div>
      </div>

      <div class="menu-item menu-center">Blog</div>

      <div class="menu-item">
        <div class="menu-text">Github</div>
      </div>

      <div class="menu-item">
        <div class="menu-text">About</div>
      </div>
    </div>

    <div class="name">
      <div class="letter">
        <img src="../assets/img/A.png" class="letter-image" />
      </div>
      <div class="letter">
        <img src="../assets/img/I2.png" class="letter-image" />
      </div>
      <div class="letter">
        <img src="../assets/img/n2.png" class="letter-image" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.name {
  display: flex;
  align-items: center;
  justify-content: center;
  vertical-align: middle;
  width: 100vw;
  height: calc(100vh - 60px);
}
.letter {
  margin: 0.8%;
  filter: drop-shadow(0px 0px 7px rgba(150, 150, 150, 0.7));
}
.letter-image {
  width: 100%;
}

.menu {
  display: flex;
  align-items: center;
  justify-content: space-around;
  margin-top: 10px;
  height: 60px;
}

.menu-item {
  flex: 1;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

.menu-text {
  font-size: 20px;
  color: #818181;
  cursor: pointer;
  padding: 10px;
  width: fit-content;
}

.menu-text:hover {
  color: #a75d5d;
  border-bottom: 2px solid #c278ff;
}

.menu-center {
  font-size: 36px;
  color: green;
}
</style>
