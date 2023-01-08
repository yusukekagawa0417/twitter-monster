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
              Lv.5
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
              Lv.50
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
  </section>
</template>

<script>
export default {
  layout: 'gameboy'
}
</script>

<style>
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
</style>