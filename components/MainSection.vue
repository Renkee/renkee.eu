<template>
  <div class="main-section">
    <Logo class="main-logo" />
    <div class="main-title">
      <div class="main-text">René Lajvort</div>
      <div class="main-social">
        <a href="https://github.com/Renkee" class="social-icon icon-github">
          <svg role="img" viewBox="0 0 24 24">
            <title>GitHub</title>
            <path
              d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"
            />
          </svg>
        </a>
        <a href="https://twitter.com/renkee_" class="social-icon icon-twitter">
          <svg role="img" viewBox="0 0 24 24">
            <title>Twitter</title>
            <path
              d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"
            />
          </svg>
        </a>
        <a href="mailto:rene@renkee.eu" class="social-icon icon-mail">
          <svg role="img" viewBox="0 0 24 24">
            <title>Mail</title>
            <path
              d="M24 4.5v15c0 .85-.65 1.5-1.5 1.5H21V7.387l-9 6.463-9-6.463V21H1.5C.649 21 0 20.35 0 19.5v-15c0-.425.162-.8.431-1.068C.7 3.16 1.076 3 1.5 3H2l10 7.25L22 3h.5c.425 0 .8.162 1.069.432.27.268.431.643.431 1.068z"
            />
          </svg>
        </a>
        <a
          href="https://www.linkedin.com/in/ren%C3%A9-lajvort-a28021135/"
          class="social-icon icon-linkedin"
        >
          <svg role="img" viewBox="0 0 448 512">
            <title>LinkedIn</title>
            <path
              d="M100.28 448H7.4V148.9h92.88zM53.79 108.1C24.09 108.1 0 83.5 0 53.8a53.79 53.79 0 0 1 107.58 0c0 29.7-24.1 54.3-53.79 54.3zM447.9 448h-92.68V302.4c0-34.7-.7-79.2-48.29-79.2-48.29 0-55.69 37.7-55.69 76.7V448h-92.78V148.9h89.08v40.8h1.3c12.4-23.5 42.69-48.3 87.88-48.3 94 0 111.28 61.9 111.28 142.3V448z"
            />
          </svg>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.main-section {
  display: flex;
  flex-wrap: nowrap;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #fafafa;
  width: 100%;
  height: 100vh;
}

.main-logo {
  animation: scaleDown 1s 0.85s both ease-in-out;
  will-change: transform;
}

.main-title {
  animation: pushUpAnim 1s 0.85s both ease-in-out, fadeIn 1s 1.3s both;
  will-change: opacity, height;
  padding: 5vmin;
}

.main-text {
  animation: weightGain 1s 1.3s both;
  will-change: transform;
  font-size: 9vmin;
  font-weight: bold;
  font-family: 'Space Grotesk', sans-serif;
}
.main-social {
  height: 10vmin;
  padding: 1vmin;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-evenly;
  align-items: center;
  animation: fadeIn 1s 1.5s both;
  will-change: opacity;

  .social-icon {
    width: 4.5vmin;
    height: 4.5vmin;
    min-width: 24px;
    min-height: 24px;
    transition: fill 0.15s ease-in;
    padding: 1vmin;
  }
}

.icon-github {
  fill: #444;
  &:hover {
    fill: #000;
  }
}

.icon-mail {
  fill: rgb(255, 117, 117);
  &:hover {
    fill: rgb(255, 31, 31);
  }
}

.icon-twitter {
  fill: rgb(125, 188, 228);
  &:hover {
    fill: rgb(29, 161, 242);
  }
}

.icon-linkedin {
  fill: rgb(79, 153, 227);
  margin-bottom: 5px;
  transform: scale(0.9);
  &:hover {
    fill: rgb(10, 102, 194);
  }
}

.icon-youtube {
  fill: rgb(255, 117, 117);
  &:hover {
    fill: rgb(255, 0, 0);
  }
}

@keyframes pushUpAnim {
  from {
    height: 0;
  }

  to {
    height: 25vmin;
  }
}

@keyframes scaleDown {
  from {
    transform: scale(1);
  }
  to {
    transform: scale(0.75);
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes weightGain {
  from {
    font-variation-settings: 'wght' 300;
  }

  to {
    font-variation-settings: 'wght' 700;
  }
}
</style>
