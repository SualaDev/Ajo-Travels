<template>
  <div>
    <div class="first-segment">
      <div class="text">
        <div class="line"></div>
        <h2 class="text-header">
          We understand, exploring cities can be hard
        </h2>
        <div class="line"></div>
      </div>
      <div class="images">
        <div class="road-sign">
          <div class="image-1" />
          <p>You run the risk of getting lost.</p>
        </div>
        <div class="share">
          <div class="image-2" />
          <p>Not a lot of options <br> for you to explore.</p>
        </div>
        <div class="report">
          <div class="image-3" />
          <p>Missing out a lot of fun activities and attractions.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DetailsPage'
}
</script>

<style  scoped>
.first-segment{
  padding: 39.6rem 0 9rem 0;
  position: relative;
}
.images{
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 8.4rem 0 8.4rem 0;
  margin: 0 4rem 0 4rem;
  /* border-top: 1px solid rgb(192,192,192,0.3); */
  border-bottom: 1px solid rgb(192,192,192,0.3);
  column-gap: 8.3rem;
}
.images p{
  font-size: 24px;
  line-height: 2.25rem;
  font-weight: 400;
  font-family: 'Cereal Book';
  font-weight: 400;
  width: 216.85px;
}
.image-1{
  background-image: url(~assets/images/road-sign.svg);
  width: 143.59px;
  height: 138.46px;
  margin-bottom: 16.2px;
}
.image-2{
  background-image: url(~assets/images/share.svg);
  width: 215.78px;
  height: 137.73px;
  margin-bottom: 16.93px;
}
.image-3{
  background-image: url(~assets/images/updates.svg);
  width: 165.67px;
  height: 137.73px;
  margin-bottom: 16.93px;
}
.text{
  display: flex;
  justify-content: center;
  align-items: center;
}

.text .line{
  background: rgb(198, 198, 198);
  width: 50%;
  height: 1px;
}

.text .text-header{
  /* width: 15rem; */
  text-align: center;
  font-size: 1.5rem;
}

.yellow{
  position: absolute;
  top: 650px;
  left: 470px;
  background-image: url(~assets/images/yellow.svg);
  width: 451px;
  height: 23px;
}
@media only screen and (max-width: 769px){
.first-segment{
  padding: 9rem 0;
  position: relative;
}
}

@media only screen and (max-width: 1300px){
  .images{
    display: flex;
    flex-direction: column;
    row-gap: 8.3rem
  }
  /* .text{
    position: absolute;
    top: 590px;
    left: 400px;
    text-align: center;
    padding: 0 2rem;
    background-color: #FFF;
  } */
}
/* @media only screen and (max-width: 1200px){
  .text{
    position: absolute;
    top: 590px;
    left: 400px;
    text-align: center;
    padding: 0 2rem;
    background-color: #FFF;
  }
}
@media only screen and (max-width: 1100px){
  .text{
    position: absolute;
    top: 590px;
    left: 240px;
    text-align: center;
    padding: 0 2rem;
    background-color: #FFF;
  }
}
@media screen and (max-width: 850px){
  .text{
    position: absolute;
    top: 590px;
    left: 170px;
    text-align: center;
    padding: 0 2rem;
    background-color: #FFF;
  }
}
@media screen and (max-width: 720px){
  .text{
    position: absolute;
    top: 590px;
    left: 120px;
    text-align: center;
    padding: 0 2rem;
    background-color: #FFF;
  }
}
@media screen and (max-width: 550px){
  .text{
    position: absolute;
    top: 590px;
    left: 60px;
    text-align: center;
    padding: 0 2rem;
    background-color: #FFF;
  }
} */
/* @media screen and (max-width: 500px){
  .text{
    top: 490px;
    left: 20px;
  }
  .text-header{
    font-size: 1.3rem;
    max-width: 290px;
  }
} */
</style>
