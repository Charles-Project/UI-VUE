<template>
  <div class="container pt-3 mb-4">
    <div class="row">
      <!-- card component -->
      <div class="col-sm-4 mb-3" v-for="(color, i) in bgColors">
        <cardCom
          :bgcolor="color"
          :icon="icons[i]"
          :iconBg="iconBgs[i]"
          :cardtextH="cardH"
          :cardtextP="cardP"
        />
      </div>
    </div>
  </div>
</template>
<script>
import cardCom from "./cardCom";
export default {
  components: {
    cardCom
  },
  data: function() {
    return {
      bgColors: ["card-bg", "card-bg1", "card-bg2"],
      icons: ["fa-user", "fa-envelope", "fa-user"],
      iconBgs: ["icon-bg", "icon-bg1", "icon-bg2"],
      iconColors: ["text-primary", "text-danger", "text-success"],
      cardH: "12000",
      cardP: "Visitors"
    };
  }
};
</script>
<style>
/*  --------------------- styles for cards --------------------------------*/
.card-body {
  padding-top: 2.5rem !important;
  padding-bottom: 2.5rem !important;
}

/* -- card background 1-- */
.card-bg {
  background: #f2f3fc;
}

.icon-bg {
  background: #e8ebf9;
}

.icon-bg .far {
  color: #405fe4;
}

/* ---- */

/* -- card background 2-- */
.card-bg1 {
  background: #fff8f9;
}

.icon-bg1 {
  background: #f7d7db;
}

.icon-bg1 .far {
  color: #dc4457;
}

/* ---- */

/* -- card background 3-- */
.card-bg2 {
  background: #f8fdff;
}

.icon-bg2 {
  background: #ccf3f7;
}

.icon-bg2 .far {
  color: #234ce0;
}

/* ---- */

.card-icon {
  width: 85px;
  height: 85px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.card-icon .far {
  font-size: 2.2rem;
}

.card-text {
  display: flex;
  flex-direction: column;
  line-height: 20px;
}

.card-text h3 {
  font-size: 2.7rem;
  margin-bottom: 5px;
  font-weight: 500;
  opacity: 0.8;
}

.card-text p {
  text-transform: uppercase;
  font-size: 1.1rem;
  font-weight: 400;
}

/*  --------------------- styles for cards --------------------------------*/

@media (max-width: 991px) {
  .card-text h3 {
    font-size: 1.7rem;
    font-weight: 400;
  }

  .card-text {
    padding-top: 1rem;
  }

  .card-text p {
    text-transform: uppercase;
    font-size: 0.8rem;
  }

  .card-icon {
    width: 60px;
    height: 60px;
  }

  .card-icon .far {
    font-size: 1.8rem;
  }
}

/* media queries */
@media (max-width: 768px) {
  .card-text {
    padding-top: 0.9rem;
    margin-left: 5px;
  }

  .card-text h3 {
    font-size: 1rem;
  }

  .card-text p {
    font-size: 0.6rem;
  }

  .card-icon {
    width: 45px;
    height: 45px;
  }

  .card-icon .far {
    font-size: 1.4rem;
  }
}

/* media queries */
@media (max-width: 577px) {
  .card-text h3 {
    font-size: 2.7rem;
  }

  .card-text p {
    font-size: 1.1rem;
  }

  .card-icon {
    width: 90px;
    height: 90px;
  }

  .card-icon .far {
    font-size: 2.3rem;
  }
}
</style>


