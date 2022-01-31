<template>
  <div class="home">
    <section class="bgBlue bgMain">
      <button
        class="bgGrey mt-3 mx-3"
        style="border: none; border-radius: 10px; width: 70px; height: 70px"
      >
        <img src="../assets/admin.png" width="50px" height="50px" />
      </button>
      <div class="d-flex flex-column align-items-center mt-5">
        <img
          src="../assets/IMG_0595.jpeg"
          width="200px"
          height="200px"
          style="border-radius: 200px"
        />
        <div class="mt-4 fontBarlow" style="font-size: 50px">Luís Gomes</div>
        <div class="mt-4 fontBarlow" style="font-size: 30px">
          Web development
        </div>
        <div class="mt-1 fontBarlow" style="font-size: 30px">
          Santa Marinha do Zêzere, Baião
        </div>
        <div
          class="mt-4 fontAsap colorMainGrey"
          style="font-size: 26px; text-align: center"
        >
          Sou estudante de programação, e um entusiasta automóvel nato!
        </div>
        <div class="d-flex mt-5">
          <button
            class="bgGrey mt-3 mx-3"
            style="border: none; border-radius: 10px; width: 70px; height: 70px"
          >
          <a href="//www.github.com/luispegasgomes">
            <img src="../assets/git.png" width="50px" height="50px" />
          </a>
            
          </button>
          <button
            class="bgGrey mt-3 mx-3"
            style="border: none; border-radius: 10px; width: 70px; height: 70px"
          >
            <img src="../assets/in.png" width="50px" height="50px" />
          </button>
          <button
            class="bgGrey mt-3 mx-3"
            style="border: none; border-radius: 10px; width: 70px; height: 70px"
          >
            <img src="../assets/fb.png" width="50px" height="50px" />
          </button>
        </div>
      </div>
    </section>
    <div
      class="
        fontBarlow
        d-flex
        flex-column
        align-items-center
        justify-content-center
        mt-4
        mb-5
      "
    >
      <div class="row">
        <div class="col-sm mt-3">
          <button
            v-on:click="selected = 'sobre'"
            :class="{
              'mx-3': true,
              btns: true,
              selectedBtn: selected == 'sobre',
            }"
          >
            <img
              src="../assets/info.png"
              width="50px"
              height="50px"
              class="mx-3"
            />SOBRE MIM
          </button>
        </div>
        <div class="col-sm mt-3">
          <button
            class="mx-3 btns"
            v-on:click="selected = 'escolaridade'"
            :class="{
              'mx-3': true,
              btns: true,
              selectedBtn: selected == 'escolaridade',
            }"
          >
            <img
              src="../assets/escola.png"
              width="50px"
              height="50px"
              class="mx-2"
            />ESCOLARIDADE
          </button>
        </div>
        <div class="col-sm mt-3">
          <button
            class="mx-3 btns"
            v-on:click="selected = 'interesses'"
            :class="{
              'mx-3': true,
              btns: true,
              selectedBtn: selected == 'interesses',
            }"
          >
            <img
              src="../assets/hob.png"
              width="50px"
              height="50px"
              class="mx-3"
            />INTERESSES
          </button>
        </div>
        <div class="col-sm mt-3">
          <button
            class="mx-3 btns"
            v-on:click="selected = 'certificados'"
            :class="{
              'mx-3': true,
              btns: true,
              selectedBtn: selected == 'certificados',
            }"
          >
            <img
              src="../assets/cert.png"
              width="50px"
              height="50px"
              class="mx-3"
            />CERTIFICADOS
          </button>
        </div>
      </div>
    </div>
    <div v-if="selected == 'sobre'" class="mb-5">
      <div class="mt-5 fontAsap text">luispegasgomes@gmail.com</div>
      <div class="mt-5 fontAsap text">
        Estudo Web Development/Programming <br />
        ESMAD | Escola Superior de Media Artes e Design
      </div>
      <div class="mt-5 fontAsap text">
        Resido em Santa Marinha do Zêzere, Porto, Portugal
      </div>
      <div class="mt-5 fontAsap text">15 de setembro de 2002 (19 Anos)</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      selected: "",
    };
  },
  methods: {
    setSelected(text) {
      this.selected = text;
    },
  },
};
</script>
<style>
.text {
  font-size: 28px;
  text-align: center;
}
.bgMain {
  height: 100vh;
}
.btns {
  border: none;
  border-radius: 10px;
  height: 80px;
  width: 300px;
  font-size: 30px;
}
.selectedBtn {
  background: #95adb6;
}
</style>
