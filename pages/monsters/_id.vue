<template>
  <section class="container">
    <div class="frame">
      <div class="screen">
        <div class="field">
          <div class="field__rival">
            <div class="info">
              <div class="info__upper">
                <div class="info__upper--name">
                  ピカチュウ
                </div>
                <div class="info__upper--level">
                  Lv 5
                </div>
              </div>
              <div class="info__lower">
                <div class="info__hp">
                  HP <meter min="0" max="100" value="40"></meter>
                </div>
              </div>
            </div>
            <div class="icon">
              <img class="icon" src="~/assets/pika.png">
            </div>
          </div>
          <div class="field__myself">
            <div class="icon">
              <img class="icon" src="~/assets/pika.png">
            </div>
            <div class="info">
              <div class="info__upper">
                <div class="info__upper--name">
                  あなた
                </div>
                <div class="info__upper--level">
                  Lv 50
                </div>
              </div>
              <div class="info__lower">
                <div class="info__hp">
                  HP <meter min="0" max="500" value="400"></meter>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="sentence">
          ピカチュウの攻撃
        </div>
      </div>
    </div>
    <div class="controller">
      <div class="controller__logo">
        Twitter Monster
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
  </section>
</template>

<script>
export default {}
</script>

<style>
.frame{
  background: gray;
  padding: 16px 20px 20px;
  border-radius: 4px;
}
.screen{
  background: #FFFAF0;
  padding: 16px;
  border-radius: 4px;
}
.field__rival {
  height: 124px;
  display: flex;
  justify-content: space-between;
}
.field__myself {
  height: 100px;
  display: flex;
  justify-content: space-between;
}
.field__myself > .info {
  margin: 36px 0 0;
}
.info__upper {
  display: flex;
  justify-content: space-between;
}
.info__upper--level {
  margin: 0 0 0 4px;
}
meter {
  width: 120px;
}
.icon {
  width: 100px;
}
.sentence {
  height: 80px;
  padding: 8px;
  margin: 12px 0 0;
  border: 1px solid;
  border-radius: 4px;
}
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
  background: gray;
}
.controller__cross-key--parts {
  height: 28px;
  display: flex;
  justify-content: space-between;
}
.controller__cross-key--part {
  height: 28px;
  width: 28px;
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