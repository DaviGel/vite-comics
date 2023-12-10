<script>
export default {
  name: 'BottomFooterComponent',
  data() {
    return {
      iconPath: [
        '../../img/footer-facebook.png',
        '../../img/footer-periscope.png',
        '../../img/footer-pinterest.png',
        '../../img/footer-twitter.png',
        '../../img/footer-youtube.png',
      ],
    };
  },
};
</script>

<template>
  <div class="bottom-footer">
    <div class="container">
      <div class="left-content t-upper"><button>Sign-up now</button></div>
      <div class="right-content t-upper">
        <strong>Follow us</strong>
        <ul>
          <li v-for="(path, index) in iconPath">
            <button><img :src="path" :alt="index" /></button>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.bottom-footer {
  background-color: #303030;
  .container {
    height: 110px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .left-content {
      button {
        all: unset;
        cursor: pointer;
        color: #fff;
        // text-transform: uppercase;
        padding: 17px;
        border: 2px solid #0282f9;
      }
    }
    .right-content {
      display: flex;
      align-items: center;
      gap: 30px;
      button {
        all: unset;
        cursor: pointer;
      }
      strong {
        color: #0282f9;
        margin-right: 30px;
      }
      ul {
        display: flex;
        li {
          list-style: none;
          img {
            margin-right: 18px;
          }
        }
      }
    }
  }
}
</style>
