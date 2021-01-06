<template>
  <div class="portfolio-section">
    <div class="section-container">
      <h1>portfolio</h1>
      <div class="portfolio-grid">
        <div class="porftolio-grid-area tft-area">
          <div class="porfolio-grid-img">
            <video autoplay loop muted playsinline>
              <source src="/portfolio/tft_app/tft.webm" type="video/webm" />
              <source src="/portfolio/tft_app/tft.mp4" type="video/mp4" />
              <picture>
                <source
                  srcset="/portfolio/tft_app/tft.webp"
                  type="image/webp"
                />
                <img
                  src="/portfolio/tft_app/tft.jpg"
                  alt="TFT image"
                  title="Your browser does not support the <video> tag"
                />
              </picture>
            </video>
          </div>
          <div class="porfolio-grid-text">
            <h4>Vue / Laravel</h4>
            <h2>TFT Item Helper</h2>
            <p>
              Helps you choose between
              <a href="https://teamfighttactics.leagueoflegends.com/"
                >Teamfight Tactics</a
              >
              builds based on your selected items.
            </p>
            <div class="portfolio-grid-buttons">
              <a href="https://tft.renkee.eu">
                <div class="live">Visit</div>
              </a>
              <a href="https://github.com/Renkee/tft-item-helper">
                <div class="source">GitHub</div>
              </a>
            </div>
          </div>
        </div>
        <div class="porftolio-grid-area movie-area">
          <div class="porfolio-grid-img">
            <video autoplay loop muted playsinline>
              <source
                src="/portfolio/movie_list/movielist.webm"
                type="video/webm"
              />
              <source
                src="/portfolio/movie_list/movielist.mp4"
                type="video/mp4"
              />
              <picture>
                <source
                  srcset="/portfolio/movie_list/movielist.webp"
                  type="image/webp"
                />
                <img
                  src="/portfolio/movie_list/movielist.jpg"
                  alt="MovieList image"
                  title="Your browser does not support the <video> tag"
                />
              </picture>
            </video>
          </div>
          <div class="porfolio-grid-text">
            <h4>Vue / Laravel</h4>
            <h2>Movie List</h2>
            <p>
              Track and rate the movies you've watched. Made in collaboration
              with
              <a href="https://github.com/hkovesdi">Hunor</a>. This project
              remains unfinished.
            </p>
            <div class="portfolio-grid-buttons">
              <a href="https://movielist.renkee.eu">
                <div class="live">Visit</div>
              </a>
              <a href="https://github.com/hkovesdi/movie-list">
                <div class="source">GitHub</div>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.portfolio-section {
  background-color: #fafafa;
  color: #333;
}

.portfolio-grid {
  display: grid;
  grid-template-columns: minmax(0, 1fr);
  grid-template-rows: repeat(2, minmax(0, 1fr));
  grid-template-areas:
    'tft-area'
    'movie-area'
    'freelo-area';
  align-items: center;
}

.porftolio-grid-area {
  display: flex;
  flex-wrap: nowrap;
  align-items: center;
}

.tft-area {
  grid-area: 'tft-area';
}
.movie-area {
  grid-area: 'movie-area';
}
.freelo-area {
  grid-area: 'freelo-area';
}

.porfolio-grid-img img {
  max-width: 100%;
  object-fit: cover;
}

.portfolio-grid-buttons {
  a {
    font-family: 'Space Mono', monospace;
    text-decoration: none;
    color: #fafafa;
    margin-right: 0.5rem;
    display: inline-block;
  }
  div {
    display: inline-block;
    padding: 0.5rem;
    background-color: #666;
    transition: background-color 0.2s ease-out;
  }
  .source:hover {
    background-color: #252525;
  }
  .live:hover {
    background-color: #34495e;
  }
}

@media screen and (min-width: 700px) {
  .porftolio-grid-area {
    flex-direction: row;
    justify-content: space-between;
  }
  .porfolio-grid-text {
    width: 47.5%;
    margin-bottom: 4rem;
    p {
      line-height: 1.25;
    }
  }

  .porfolio-grid-img {
    width: 47.5%;
    margin-bottom: 4rem;
  }
  .porftolio-grid-area:nth-child(odd) {
    flex-direction: row-reverse;
  }
}

@media screen and (max-width: 699px) {
  .porftolio-grid-area {
    flex-direction: column;
    justify-content: center;
  }
  .porfolio-grid-img {
    width: 100%;
    margin-bottom: 1rem;
  }
  .porfolio-grid-text {
    width: 100%;
    margin-bottom: 4rem;
  }
}
</style>
