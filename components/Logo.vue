<template>
  <div id="logo-container">
    <div class="colored-rectangle rect-6"></div>
    <div class="colored-rectangle rect-5"></div>
    <div class="colored-rectangle rect-4"></div>
    <div class="colored-rectangle rect-3"></div>
    <div class="colored-rectangle rect-2"></div>
    <div id="main-rect">
      <div class="colored-rectangle rect-1"></div>
      <div id="text-container">
        <div id="text">rnk</div>
        <div id="underline"></div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@font-face {
  font-family: 'Harabara Mais Demo';
  src: url('/logo_font.otf') format('opentype');
}

#logo-container {
  user-select: none;
  position: relative;
  width: 50vmin;
  height: 50vmin;
  display: inline-block;

  .colored-rectangle {
    position: absolute;
    width: 100%;
    height: 100%;
    opacity: 0;
    will-change: opacity;
  }

  #main-rect {
    position: absolute;
    width: 100%;
    height: 100%;
    opacity: 1;
  }
}

#text-container {
  position: absolute;
  inset: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  #text {
    color: #ecf0f1;
    font-family: 'Harabara Mais Demo', sans-serif;
    line-height: 50vmin * 0.4;
    font-size: 50vmin * 0.64;
    text-shadow: 0px 0px 1px rgba(0, 0, 0, 0.55);
    animation: logoTextFade 1s 0.7s both;
    will-change: opacity;
  }
  #underline {
    background-color: #ecf0f1;
    height: 50vmin * 0.048;
    width: 50vmin * 0.848;
    margin-left: 50vmin * 0.026;
    border-bottom-left-radius: 50vmin * 0.848 * 0.0117924528;
    border-bottom-right-radius: 50vmin * 0.848 * 0.0117924528;
    box-shadow: 0px 0px 1px 0px rgba(0, 0, 0, 0.55);
    animation: logoTextFade 1s 0.7s both, logoUnderlineAnim 1.8s 0.7s both;
    will-change: opacity, clip-path;
  }
}

.rect-1 {
  background-color: #34495e;
  animation: logoRectFade 1s 0.5s both;
}
.rect-2 {
  background-color: #c0392b;
  transform: rotate(15deg);
  animation: logoRectFade 1s 0.4s both;
}
.rect-3 {
  background-color: #9b59b6;
  transform: rotate(30deg);
  animation: logoRectFade 1s 0.3s both;
}
.rect-4 {
  background-color: #2980b9;
  transform: rotate(45deg);
  animation: logoRectFade 1s 0.2s both;
}
.rect-5 {
  background-color: #f1c40f;
  transform: rotate(60deg);
  animation: logoRectFade 1s 0.1s both;
}
.rect-6 {
  background-color: #f39c12;
  transform: rotate(75deg);
  animation: logoRectFade 1s 0s both;
}

@keyframes logoRectFade {
  from {
    opacity: 0;
  }
  to {
    opacity: 0.87;
  }
}

@keyframes logoTextFade {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes logoUnderlineAnim {
  from {
    clip-path: inset(0 100% 0 0);
  }
  to {
    clip-path: inset(0);
  }
}
</style>
