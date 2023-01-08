<template>
  <div class="controller">
    <div class="controller__logo">
      Tweet Monster <i class="fa-brands fa-twitter"></i>
    </div>
    <div class="controller__wrapper">
      <div class="controller__cross-key">
        <div class="controller__cross-key--parts">
          <div class="controller__cross-key--part no-function"></div>
          <div class="controller__cross-key--part up-function"></div>
          <div class="controller__cross-key--part no-function"></div>
        </div>
        <div class="controller__cross-key--parts">
          <div class="controller__cross-key--part left-function"></div>
          <div class="controller__cross-key--part center-no-function"></div>
          <div class="controller__cross-key--part right-function"></div>
        </div>
        <div class="controller__cross-key--parts">
          <div class="controller__cross-key--part no-function"></div>
          <div class="controller__cross-key--part down-function"></div>
          <div class="controller__cross-key--part no-function"></div>
        </div>
      </div>
      <div class="controller__buttons">
        <div class="controller__button controller__button--b"></div>
        <div class="controller__button controller__button--a"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Controller'
}
</script>

<style>
.controller__logo {
  padding: 4px 0 0;
  color: #000099;
  font-size: 16px;
  font-weight: bold;
  font-style: italic;
}
.controller__wrapper {
  margin: 36px 8px 0;
  display: flex;
  justify-content: space-between;
}
.controller__cross-key {
  height: 84px;
  width: 84px;
}
.controller__cross-key--parts {
  height: 28px;
  display: flex;
  justify-content: space-between;
}
.controller__cross-key--part {
  height: 28px;
  width: 28px;
  background: gray;
}
.no-function {
  background: lightgray;
}
.controller__buttons {
  padding: 8px 0; 
  display: flex;
  justify-content: space-between;
}
.controller__button {
  height: 48px;
  width: 48px;
  background: #CC3399;
  border-radius: 50%;
}
.controller__button--b {
  margin: 16px 16px 0 0;
}
</style>