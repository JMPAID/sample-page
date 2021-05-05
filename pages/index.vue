<template>
  <div>
    <section
      class="section"
      style="background-color: #f2f2f2; padding-bottom: 160px"
    >
      <div class="container">
        <img class="header-img" src="~/assets/90_day_supplyx.png" alt="" />

        <div style="position: sticky">
          <div class="right-circle">
            <img
              class="overlay-circle"
              src="~/assets/ic_circle.png"
              alt=""
              width="200"
            />
          </div>
        </div>

        <div style="position: sticky">
          <div class="left-circle">
            <img
              class="overlay-circle"
              src="~/assets/ic_circle.png"
              alt=""
              width="200"
            />
          </div>
        </div>

        <div
          class="columns is-centered has-text-centered"
          style="margin-top: 80px"
        >
          <div class="column is-4">
            <img class="img-check" src="~/assets/ic_check.png" alt="" />
            <p class="check-description">Order prescription</p>
            <p class="check-description">meds online</p>
          </div>

          <div class="divider is-hidden-touch"></div>
          <div class="column is-4">
            <img class="img-check" src="~/assets/ic_check.png" alt="" />
            <p class="check-description">Save up</p>
            <p class="check-description">to 80%</p>
          </div>
          <div class="divider is-hidden-touch"></div>
          <div class="column is-4">
            <img class="img-check" src="~/assets/ic_check.png" alt="" />
            <p class="check-description">Fast & free delivery</p>
            <p class="check-description">to your door</p>
          </div>
        </div>
      </div>
    </section>

    <div class="section">
      <div
        class="container is-overlay"
        style="margin-top: -140px; padding-bottom: 30px"
      >
        <div class="box" style="padding: 60px 60px; margin-bottom: 120px">
          <b-field label="Start search here" class="has-text-grey">
            <b-select
              placeholder="Search Your Medication"
              icon="magnify"
              expanded
            >
              <option value="1">Option 1</option>
              <option value="2">Option 2</option>
            </b-select>
          </b-field>
        </div>

        <img src="~/assets/how_it_worksx.png" alt="" />
      </div>
    </div>

    <div
      class="section"
      style="background-color: #ff5724; padding: 160px 40px"
      id="aboutUs"
    >
      <div class="container">
        <div class="columns is-vcentered is-variable is-7">
          <div class="column is-6">
            <img src="~/assets/ic_vid.png" alt="" />
          </div>

          <div class="column is-6">
            <h1 class="title has-text-white">About Us</h1>
            <p class="has-text-white" style="line-height: 2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorum
              voluptatem aut beatae pariatur, voluptatum velit assumenda quos,
              temporibus rem voluptates minima ullam doloremque eius modi
              asperiores nisi illo soluta dignissimos. Lorem ipsum dolor sit
              amet consectetur adipisicing elit.
            </p>
          </div>
        </div>
      </div>
    </div>

    <div class="section" style="padding-bottom: 320px; padding-top: 160px">
      <h1 class="title has-text-centered">Frequently Searched Rx</h1>

      <b-carousel-list
        v-model="values"
        :data="items"
        :items-to-show="3"
        style="box-shadow: none; margin-top: 60px"
        icon-size="is-large"
        :repeat="true"
      >
        <template #item="list">
          <div class="">
            <div
              class="card-image"
              style="
                background-color: #f2f2f2;
                margin-left: 40px;
                margin-right: 40px;
                padding-top: 60px;
                padding-bottom: 50px;
              "
            >
              <figure class="image">
                <img
                  :src="list.image"
                  style="
                    height: 220px;
                    width: 120px;
                    display: block;
                    margin-left: auto;
                    margin-right: auto;
                  "
                />
              </figure>
            </div>
            <div class="card-content">
              <div class="content">
                <div class="buttons is-centered">
                  <button
                    class="button"
                    style="background-color: #3b1a45; color: white"
                  >
                    {{ list.name }}
                  </button>
                </div>
              </div>
            </div>
          </div>
        </template>
      </b-carousel-list>
    </div>

    <div
      class="section"
      style="background-color: #3b1a45; padding-bottom: 130px"
    >
      <div class="container is-overlay" style="margin-top: -235px">
        <div class="columns is-vcentered is-centered">
          <div class="column is-4">
            <img src="~/assets/iphone.tif.png" alt="" width="260" />
          </div>
          <div class="column is-6">
            <div class="box" style="background-color: #f2f2f2; padding: 30px">
              <h1 class="title">Savings Calculator</h1>
              <p
                style="line-height: 1.8; margin-bottom: 20px; margin-top: -15px"
              >
                Use our Savings Calculator to compare your current presciption
                pricing to us
              </p>

              <div class="field">
                <input
                  type="text"
                  class="input"
                  placeholder="Viagra"
                  style="border: 1px solid #ff5724"
                />
              </div>

              <div class="field">
                <div class="select is-fullwidth">
                  <select style="border: 1px solid #ff5724">
                    <option value="1" selected disabled>
                      Viagra 25MG (Prescription)
                    </option>
                  </select>
                </div>
              </div>

              <div>
                <b-button
                  style="
                    background-color: #ff5724;
                    color: white;
                    width: 110px;
                    height: 45px;
                    margin-right: 16px;
                  "
                  >Add</b-button
                >
                <b-button
                  style="
                    background-color: #3b1a45;
                    color: white;
                    width: 110px;
                    height: 45px;
                  "
                  >Clear</b-button
                >
              </div>
            </div>
          </div>
        </div>

        <div
          class="columns has-text-white has-text-centered is-centered is-variable is-8"
          style="margin-top: 20px"
        >
          <div class="column is-3 has-text-left">
            <h4 class="has-text-white is-size-6 has-text-weight-bold">
              Prescription/Dosage
            </h4>
            <p>Viagra</p>
            <p>Viagra 25MG(Prescription)</p>
          </div>
          <div class="column is-2">
            <h4>Qty</h4>
            <b-field>
              <b-numberinput step="1" exponential> </b-numberinput>
            </b-field>
          </div>
          <div class="column is-2">
            <h4>Usual Copay?</h4>
            <b-field>
              <b-input placeholder="$100"></b-input>
            </b-field>
          </div>
          <div class="column is-2">
            <h4>VeloxRxPrice</h4>
            <b-field>
              <b-input placeholder="$89.92"></b-input>
            </b-field>
          </div>
          <div class="column is-2">
            <h4>Savings</h4>
            <div class="field">
              <input
                type="text"
                class="input savings"
                placeholder="$10.18"
                style="background-color: #ff5724; border: none; color: white"
              />
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="section" style="padding-top: 140px">
      <div class="container">
        <div class="columns is-vcentered">
          <div class="column is-6">
            <h1 class="title">VeloxRx For Your</h1>
            <h1 class="title" style="margin-top: -14px">Furry Friends</h1>
            <p style="line-height: 2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Repellendus, dolorum. Aperiam aliquid ipsam iusto ipsum culpa
              impedit qui aliquam vitae corporis corrupti! Tempore voluptates
              architecto sapiente doloremque voluptas ut maxime?
            </p>
          </div>
          <div class="column is-6">
            <img src="~/assets/ic_cat_dog.png" alt="" />
          </div>
        </div>
      </div>
    </div>

    <hr />

    <div class="section" style="padding-bottom: 160px">
      <div class="container">
        <div class="columns is-variable is-6">
          <div class="column is-5">
            <div>
              <img
                src="~/assets/footer_logo.png"
                alt=""
                width="250"
                style="margin-bottom: 40px"
              />
            </div>

            <div>
              <img
                src="~/assets/ic_pharmacy.png"
                alt=""
                width="100"
                style="margin-bottom: 15px"
              />
            </div>
            <p style="font-size: 14px; margin-bottom: 10px">
              VeloxRx (veloxrx.com) is a licensed pharmary
            </p>
            <p style="font-size: 14px">accredited through NABP, Dot.Pharmary</p>
          </div>
          <div class="column is-4" style="margin-top: 50px">
            <h1 class="title is-size-4">For Doctors</h1>
            <p style="font-size: 14px; margin-bottom: 14px">
              Velox Pharmacy Solutions
            </p>
            <p style="font-size: 14px; margin-bottom: 14px">
              24275 Katy Fwy Ste. 400,
            </p>
            <p style="font-size: 14px">Katy, TX, 77494</p>
          </div>
          <div class="column is-3" style="margin-top: 50px">
            <h1 class="title is-size-4">Contact Us</h1>
            <div
              class="is-inline-flex"
              style="font-size: 14px; margin-bottom: 14px"
            >
              <img
                src="~/assets/ic_mail.png"
                alt=""
                style="margin-right: 10px"
              />
              <p>pharmary@veloxrx.com</p>
            </div>

            <div
              class="is-inline-flex"
              style="font-size: 14px; margin-bottom: 14px"
            >
              <img
                src="~/assets/ic_headset.png"
                alt=""
                style="margin-right: 10px"
              />
              <p>(346) 387-7160</p>
            </div>

            <div>
              <div
                class="is-inline-flex"
                style="font-size: 14px; margin-bottom: 14px"
              >
                <img
                  src="~/assets/ic_pager.png"
                  alt=""
                  style="margin-right: 10px"
                />
                <p>(346) 707-3640</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomePage",
  data() {
    return {
      values: 1,
      items: [
        {
          name: "Lisonopril",
          image: require("@/assets/cupx.png"),
        },
        {
          name: "Atorvastatin",
          image: require("@/assets/cupx.png"),
        },
        {
          name: "Metmorfin",
          image: require("@/assets/cupx.png"),
        },
        {
          name: "Viagra",
          image: require("@/assets/cupx.png"),
        },
        {
          name: "Atorvastatin",
          image: require("@/assets/cupx.png"),
        },
      ],
    };
  },
};
</script>

<style scoped>
.header-img {
  margin-left: auto;
  margin-right: auto;
  display: block;
}

.divider {
  border-right: 1px solid #3b1a45;
  height: 160px;
  margin-top: 10px;
}
.img-check {
  /* width: 36px; */
  height: 28px;
  margin-bottom: 20px;
}

p.check-description {
  font-size: 24px;
  font-family: "Source Sans Pro", sans-serif;
}

h1 {
  color: #3b1a45;
  font-size: 42px;
}

h4 {
  margin-bottom: 50px;
}

.carousel-item {
  width: 60px !important;
  height: 40px !important;
}

input.savings::placeholder {
  color: white;
}

hr {
  border-top: 1px solid #3b1a45;
  margin: 40px 80px;
}

.right-circle {
  position: absolute;
  right: -220px;
  top: -260px;
}

.left-circle {
  position: absolute;
  left: -250px;
  top: -60px;
}

@media only screen and (min-width: 769px) and (max-width: 1023px) {
  .right-circle {
    position: absolute;
    right: -150px;
  }

  .left-circle {
    position: absolute;
    left: -170px;
    top: -30px;
  }
}

@media only screen and (min-width: 1216px) and (max-width: 1407px) {
  .right-circle {
    position: absolute;
    right: -225px;
    top: -290px;
  }

  .left-circle {
    position: absolute;
    left: -210px;
    top: -30px;
  }
}

@media only screen and (min-width: 1408px) {
  .right-circle {
    position: absolute;
    right: -140px;
    top: -290px;
  }

  .left-circle {
    position: absolute;
    left: -150px;
    top: 0px;
  }
}
</style>