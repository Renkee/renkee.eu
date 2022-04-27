<template>
  <div class="work-experience-section">
    <div class="section-container">
      <h1>work experience</h1>
      <div>
        <div class="work-name-time">
          <div class="work-name">
            <a href="https://weborigo.com">WebOrigo</a>
          </div>
          <div class="work-time">since 2021</div>
        </div>
        <div class="work-title">Laravel/Vue fullstack developer</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.work-experience-section {
  background-color: #fafafa;
  color: #333;
}
.work-name-time {
  display: inline-flex;
  align-items: baseline;
}
.work-name {
  font-size: 1.8rem;
  font-weight: 600;
  margin-right: 0.5rem;
}
.work-time {
  font-size: 1.2rem;
  font-weight: 300;
}
.work-title {
  font-size: 1.2rem;
  font-weight: 420;
}
</style>
