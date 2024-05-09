<template>
<div class="nav-container">
  <nav class="left-navigation">
    <div class="brand-container">
      <div class="brand-wrap">
        <a class="link-logo">
          <img class="img-logo" src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="logo" />
        </a>
      </div>
    </div>
    <div class="new-container">

    </div>

  </nav>
</div>
</template>

<script setup lang="ts">
</script>

<style scoped>
.nav-container {
  width: 260px;
  height: 100%;
  display: flex;
  background-color: #efefef;
  transition: width var(--transition-duration) var(--transition-timing-function);
  --transition-duration: 300ms;
  --delayed-transition-duration: 400ms;
  --transition-timing-function: cubic-bezier(0, 0, 0, 1);

  .left-navigation {
    width: 260px;
    position: fixed;
    top: 0;
    z-index: 10;
    display: flex;
    flex-direction: column;
    gap: 4px;
    height: 100vh;
    border-right: 1px solid #CCCCCC;
    background:  #ffffff;
    transition: width var(--transition-duration) var(--transition-timing-function), box-shadow var(--transition-duration) var(--transition-timing-function);

    .brand-container {
      .brand-wrap {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 60px;
        background-color: #ffffff;
        transition: background-color var(--transition-duration) var(--transition-timing-function);

        .link-logo {
          display: flex;
          justify-content: center;
          align-items: center;
          height: 100%;
          width: 100%;
          transition: background-color var(--transition-duration) var(--transition-timing-function);

          .img-logo {
            height: 40px;
            width: 40px;
            transition: height var(--transition-duration) var(--transition-timing-function), width var(--transition-duration) var(--transition-timing-function);
          }
        }
      }
    }
  }
}
</style>
