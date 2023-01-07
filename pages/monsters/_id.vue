<template>
  <section class="container">
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
                ライチュウ
              </div>
              <div class="info__upper--level">
                Lv 10
              </div>
            </div>
            <div class="info__lower">
              <div class="info__hp">
                HP <meter min="0" max="500" value="40"></meter>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="sentence">
        ピカチュウの攻撃
      </div>
  </section>
</template>

<script>
export default {}
</script>

<style>
body {
  background: lightgray;
  padding: 8px;
}
.container{
  background: #FFFAF0;
  padding: 12px;
}
.field__rival {
  height: 160px;
  display: flex;
  justify-content: space-between;
}
.field__myself {
  height: 120px;
  display: flex;
  justify-content: space-between;
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
  width: 120px;
}
.sentence {
  height: 160px;
  padding: 8px;
  margin: 12px 0 0;
  border: 1px solid;
  border-radius: 4px;
}
</style>