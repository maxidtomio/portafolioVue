<script setup></script>

<template>

    <button class="card">
  <div class="row clearfix">
    <div class="left big" id="utn">UTN</div>
  </div>
  <div class="row">
    <p><span class="big">M</span>aximiliano <span class="big">Tomio</span></p>
    <p><span class="big">W</span>eb <span class="big">D</span>eveloper</p>
  </div>
  <div class="row">
    <p><span class="med">301 G</span><span class="small">eneral </span><span class="med">A</span><span class="small">lvear </span><span class="med">M</span><span class="small">endoza </span><span class="med">A</span><span class="small">rgentina</span><span class="med">, C. P. 5620 E</span><span class="small">mail </span><span class="med">maxidpoggio@gmail.com T</span><span class="med">el </span><span class="med">261 5152555</span>
    </p>
  </div>
</button>

</template>

<style scoped>



@import url(https://fonts.googleapis.com/css?family=Cormorant+Garamond);

*,
*::before,
*::after {
  box-sizing: border-box;
}

html {
  font-family: "Cormorant Garamond", serif;
  text-transform: uppercase;
  box-sizing: inherit;
  font-size: 10.5px;
  letter-spacing: 1px;
  text-shadow: 0 0 2px rgba(0, 0, 0, .5),
                -1px -1px 1px rgba(179, 179, 179, .5),
                1px 1px 0 rgba(255, 255, 255, 0.55),
                0 1px 3px white;
  overflow: hidden;
  color: #191919;
  background-color: azure;
}

button {
  display: block;
  position: relative;
  background: none;
  color: inherit;
  border: none;
  padding: 0;
  font: inherit;
  text-transform: inherit;
  letter-spacing: inherit;
  text-shadow: inherit;
  cursor: pointer;
  outline: inherit;
  z-index: 10;
}

p{
    color: rgb(8, 142, 126)
}

#utn {
    color:rgb(8, 142, 126) ;
}
.clearfix::after {
    content: "";
    clear: both;
    display: table;
}

.big {
  font-size: 150%;
}

.med {
  font-size: 100%;
  letter-spacing: .5px;
}

.small {
  font-size: 65%;
  letter-spacing: .5px;
}

.no-space {
  letter-spacing: 0px;
}

.card {
  background-color: #d5c8ae;
  background-image: url("https://www.transparenttextures.com/patterns/paper-fibers.png");
  height: 200px;
  width: 350px;
  margin: 20vh auto 0 auto;
  padding: 20px 10px 10px 10px;
  transform: rotateX(60deg) rotateY(0deg) rotateZ(45deg);
  /*transform-origin: 50% 100%;*/
  box-shadow: 0;
  transition: transform .4s ease,
              box-shadow .4s ease;
}

.card:hover {
  cursor: pointer;
  transform: rotateX(60deg) rotateY(0deg) rotateZ(45deg) translateZ(10px);
  box-shadow: 20px 20px 20px rgba(0, 0, 0, .4);
}

.card:focus {
  transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg) translateZ(10px);
  box-shadow: 0px 10px 10px rgba(0, 0, 0, .4);
}

.card:focus::before {
  transform: skewX(0deg) translateX(0px) translateY(0px);
  height: 0px;
}

.card:focus::after {
  transform: skewY(0deg) translateX(0px) translateY(0px);
  width: 0px;
}

.card::before,
.card::after {
  content: "";
  position: absolute;
  display: block;
  background-color: rgb(56, 42, 42);
  transition: transform .4s ease,
              height .4s ease,
              width .4s ease;
}

.card::before {
  width: 100%;
  height: 6px;
  bottom: 0;
  left: 0;
  transform: skewX(45deg) translateX(-3px) translateY(6px);
}

.card::after {
  height: 100%;
  width: 6px;
  top: 0;
  right: 0;
  transform: skewY(45deg) translateX(6px) translateY(-3px);
}

.row {
  display: block;
  text-align: center;
}

.row:nth-child(2) {
  margin: 35px 0 50px 0;
}

.left {
  float: left;
}

.right {
  float: right;
}

p {
  margin: 0;
}
</style>