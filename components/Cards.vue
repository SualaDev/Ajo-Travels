<template lang="">
  <div class="card-container">
    <div class="first-card">
      <div class="location" />
      <div class="text">
        <h2>Explore cities with ease</h2>
        <p class="attraction">
          Find local attractions and hot spots easily without the stress of
          asking the locals.
        </p>
      </div>
    </div>
    <div class="second-card">
      <div class="text">
        <h2>Never get lost</h2>
        <p class="direction">
          Get directions directly from the app and also book rides with local
          car hires directly.
        </p>
      </div>
      <div class="phone" />
    </div>
    <div class="third-card">
      <div class="world" />
      <div class="text">
        <h2>International suggestions</h2>
        <p class="trip">
          Get trip ideas for other countries and cities for you to explore when
          in doubt.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardPage'
}
</script>

<style scoped>
.card-container {
  /* padding: 0 8.25rem 11.6rem 8.25rem; */
  /* border-bottom: 1px solid rgb(192,192,192,0.3); */
  margin: 0 4rem 0 4rem;
}
.first-card {
  display: flex;
  justify-content: center;
  align-items: center;
  column-gap: 10rem;
  padding-bottom: 11.6rem;
}
.location {
  background-image: url(~assets/images/location.svg);
  background-repeat: no-repeat;
  width: 100%;
  height: 450px;
}
.second-card {
  display: flex;
  justify-content: center;
  align-items: center;
  column-gap: 19.75rem;
  padding-bottom: 11.6rem;
}
.phone {
  background-image: url(~assets/images/phone.svg);
  background-repeat: no-repeat;
  width: 100%;
  height: 449.99px;
}
.third-card {
  display: flex;
  justify-content: center;
  align-items: center;
  column-gap: 6rem;
  padding-bottom: 11.6rem;
  border-bottom: 1px solid rgb(192, 192, 192, 0.3);
}
.world {
  background-image: url(~assets/images/world-location.svg);
  background-repeat: no-repeat;
  width: 100%;
  height: 450px;
}
.text {
  display: flex;
  flex-direction: column;
}

.attraction, .direction, .trip{
  width: 50%;
}

/* .attraction {
  width: 383px;
}
.direction {
  width: 296px;
}
.trip {
  width: 296px;
} */
h2 {
  font-size: 35px;
  line-height: 2.75rem;
  margin-bottom: 1.75rem;
  font-family: 'Cereal Medium';
  font-weight: 500;
}
p {
  font-size: 24px;
  line-height: 2.25rem;
  font-family: 'Cereal Book';
  font-weight: 400;
}
@media only screen and (max-width: 1300px){
  .first-card{
    display: flex;
    flex-direction: column;
    row-gap:10rem
  }
  .second-card{
    display: flex;
    flex-direction: column-reverse;
    row-gap:7rem
  }
  .third-card{
    display: flex;
    flex-direction: column;
    row-gap:6rem
  }
}
@media screen and (max-width: 600px){
  .location,.phone,.world{
    background-size: 65%;
    background-repeat: no-repeat;
    background-position: center center;
    width: 100%;
  }
}
</style>
