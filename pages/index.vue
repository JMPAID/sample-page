<template>
  <div>
    <section class="section" style="background-color: #f2f2f2">
      <div class="container">
        <img class="header-img" src="~/assets/90_day_supply.png" alt="" />

        <!-- <div style="position: sticky">
          <div style="position: absolute; right: -160px; top: 8px">
            <img class="overlay-circle" src="~/assets/ic_circle.png" alt="" />
          </div>
        </div> -->
      </div>

      <div
        class="columns is-centered has-text-centered"
        style="margin-top: 80px"
      >
        <div class="column is-4">
          <img class="img-check" src="~/assets/ic_check.png" alt="" />
          <p>Order prescription</p>
          <p>meds online</p>
        </div>

        <div class="divider"></div>
        <div class="column is-4">
          <img class="img-check" src="~/assets/ic_check.png" alt="" />
          <p>Save up</p>
          <p>to 80%</p>
        </div>
        <div class="divider"></div>
        <div class="column is-4">
          <img class="img-check" src="~/assets/ic_check.png" alt="" />
          <p>Fast & free delivery</p>
          <p>to your door</p>
        </div>
      </div>
    </section>

    <div class="section">
      <div class="container">
        <div class="box">
          <b-field>
            <b-input placeholder="Default" icon="account"> </b-input>
          </b-field>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomePage",
};
</script>

<style scoped>
.header-img {
  margin-left: auto;
  margin-right: auto;
  display: block;
}

.divider {
  border: 1px solid #3b1a45;
  height: 160px;
  margin-top: 10px;
}
.img-check {
  /* width: 36px; */
  height: 36px;
  margin-bottom: 20px;
}

p {
  font-size: 31px;
}
</style>