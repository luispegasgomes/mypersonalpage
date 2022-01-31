<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Mali:wght@400;500;600;700");
@import url("https://fonts.googleapis.com/css2?family=Barlow:wght@100;200;300;400;500;600;700;800;900");
@import url("https://fonts.googleapis.com/css2?family=Nunito:wght@200;300;400;500;600;700;800;900");
:root {
  --white: #ffffff;
  --black: #000000;
  --grey: #DBC7BE;
  --darkBlue: #102B3F;
  --blue: #95ADB6;
  --mainGrey: #E9E3E6;
}
body,
body * {
  margin: 0;
  padding: 0;
}
html,
body {
  overflow-x: hidden;
}
body,
#app {
  min-width: 100vw;
  min-height: 100vh;
}
.fontAsap {
  font-family: "Asap", sans-serif;
}
.fontBarlow {
  font-family: "Barlow", sans-serif;
}
.fontNunito {
  font-family: "Nunito", sans-serif;
}
.weightLight {
  font-weight: 300;
}
.weightRegular {
  font-weight: 300;
}
.weightBold {
  font-weight: 700;
}
.colorWhite {
  color: var(--white);
}
.colorBlack {
  color: var(--black);
}
.colorGrey {
  color: var(--grey);
}
.colorDarkBlue {
  color: var(--darkBlue);
}
.colorBlue {
  color: var(--blue);
}
.colorMainGrey {
  color: var(--mainGrey);
}
.bgWhite {
  background: var(--white);
}
.bgBlack {
  background: var(--black);
}
.bgGrey {
  background: var(--grey);
}
.bgDarkBlue {
  background: var(--darkBlue);
}
.bgBlue {
  background: var(--blue);
}
.bgMainGrey {
  background: var(--mainGrey);
}
</style>