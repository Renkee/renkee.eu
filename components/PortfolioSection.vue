<template>
  <div class="portfolio-section">
    <div class="section-container">
      <h1>portfolio</h1>
      <div class="portfolio-grid">
        <div class="porftolio-grid-area tft-area">
          <div class="porfolio-grid-img">
            <img src="/test.jpg" />
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
              <a href="https://github.com/Renkee/tft-item-helper">GitHub</a>
              <a href="https://tft.renkee.eu">Visit</a>
            </div>
          </div>
        </div>
        <div class="porftolio-grid-area movie-area">
          <div class="porfolio-grid-img">
            <img src="/test.jpg" />
          </div>
          <div class="porfolio-grid-text">
            <h4>Vue / Laravel</h4>
            <h2>Movie List</h2>
            <p>
              A web application that makes it simple to keep track of the movies
              you've watched and rate them. I did most of the frontend work.
            </p>
            <div class="portfolio-grid-buttons">
              <a href="https://github.com/hkovesdi/movie-list">GitHub</a>
              <a href="https://movielist.renkee.eu">Visit</a>
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

@media screen and (min-width: 700px) {
  .porftolio-grid-area {
    flex-direction: row;
    justify-content: space-between;
  }
  .porfolio-grid-text {
    width: 47.5%;
    margin-bottom: 4rem;
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
