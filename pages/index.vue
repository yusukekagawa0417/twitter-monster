<template>
  <section class="container">
    <div class="title">
      ツイートモンスター
      <div class="title__english">
        Tweet Monster
      </div>
      <i class="fa-brands fa-twitter title__icon"></i>
    </div>
    <div class="config">
      <form v-on:submit.prevent="start">
        <label class="config__explaination">対戦相手を入力してください</label>
        <input class="config__form" v-model="rival" placeholder="@elonmusk">
        <button class="config__start-button">バトル開始</button>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  data() {
      return {
        rival: '',
      }
  },
  methods: {
    start() {
      this.$router.push('/monsters/' + this.rival);
    }
  },
  layout: 'gameboy',
}
</script>

<style>
.title {
  font-size: 28px;
  font-weight: bold;
  text-align: center;
  margin: 20px 0 0;
}
.title__english {
  font-size: 16px;
  margin: 16px 0 0;
}
.title__icon {
  font-size: 64px;
  margin: 28px 0 0;
}
.config {
  margin: 28px 0 0;
  text-align: center;
}
.config__explaination {
  display: inline-block;
  margin: 0 0 8px;
}
.config__form {
  height: 28px;
  padding: 0 8px;
  border-radius: 4px;
  border: none;
  box-shadow: 0 0 0 1px #ccc inset;
}
.config__start-button {
  height: 28px;
  padding: 0 8px;
  border: none;
  border-radius: 4px;
  background: #333;
  color: #fff;
  font-weight: bold;
  cursor: pointer;
  border: 2px solid transparent;
}
</style>