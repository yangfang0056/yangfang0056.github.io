---
permalink: /interest/
title: "兴趣爱好"
author_profile: true
---

<div class="travel-section">

<h2>Travel Journal</h2>

<p>
Exploring different places through photography.
</p>


<div class="travel-carousel">


<img 
id="travel-image"
src="/assets/images/travel/travel-dalian1.png"
>


<button 
class="prev"
onclick="changeTravel(-1)">
←
</button>


<button 
class="next"
onclick="changeTravel(1)">
→
</button>


</div>


<h3 id="travel-title">
Dalian
</h3>


<p>
Coast · City · Memories
</p>


</div>

<script>

const travels = [

{
image:"/assets/images/travel/travel-dalian1.png",
title:"Dalian"
},

{
image:"/assets/images/travel/travel-dalian2.png",
title:"Dalian"
},

{
image:"/assets/images/travel/travel-dalian3.png",
title:"Dalian"
},

{
image:"/assets/images/travel/travel-yunnan1.png",
title:"Yunnan"
},

{
image:"/assets/images/travel/travel-yunnan2.png",
title:"Yunnan"
},

{
image:"/assets/images/travel/travel-yunnan3.png",
title:"Yunnan"
}

];


let index = 0;


function changeTravel(direction){

index += direction;


if(index >= travels.length){
index = 0;
}


if(index < 0){
index = travels.length-1;
}


document.getElementById(
"travel-image"
).src = travels[index].image;


document.getElementById(
"travel-title"
).innerHTML = travels[index].title;


}

</script>

</div>

<!-- ================================
     Photography
     ================================ -->

<style>

.photography-section {
  margin-top: 100px;
  padding-top: 60px;
  border-top: 1px solid #eeeeee;
}

.photography-section h2 {
  font-size: 36px;
  font-weight: 600;
  margin-bottom: 10px;
}

.photography-intro {
  color: #777;
  font-size: 15px;
  margin-bottom: 45px;
}


/* ================================
   大图
   ================================ */

.photography-preview {
  width: 62%;
  max-width: 850px;
  aspect-ratio: 3 / 2;

  margin: 0 auto 55px;

  background: #f4f2ee;

  overflow: hidden;

  display: flex;
  align-items: center;
  justify-content: center;
}

.photography-preview img {
  width: 100%;
  height: 100%;

  object-fit: contain;

  display: block;

  opacity: 1;

  transition: opacity 0.25s ease;
}


/* ================================
   胶片
   ================================ */

.photography-film-wrapper {

  width: 100%;

  overflow-x: auto;
  overflow-y: hidden;

  padding: 25px 0 40px;

}


/* 胶片主体 */

.photography-film {

  width: max-content;

  min-width: 100%;

  display: flex;

  align-items: center;

  padding: 32px 45px;

  box-sizing: border-box;

  background: #292929;

  position: relative;

  box-shadow:
    0 10px 30px rgba(0,0,0,0.08);

}


/* ================================
   胶片齿孔
   ================================ */

.photography-film::before,
.photography-film::after {

  content: "";

  position: absolute;

  left: 0;
  right: 0;

  height: 12px;

  background-image:
    radial-gradient(
      ellipse,
      #f4f2ee 0,
      #f4f2ee 5px,
      transparent 6px
    );

  background-size: 26px 12px;

  background-repeat: repeat-x;

}


/* 上面的齿孔 */

.photography-film::before {

  top: 5px;

}


/* 下面的齿孔 */

.photography-film::after {

  bottom: 5px;

}


/* ================================
   单张照片
   ================================ */

.photography-frame {

  position: relative;

  flex: 0 0 auto;

  width: 155px;
  height: 105px;

  margin: 0 6px;

  padding: 7px;

  background: #111;

  box-sizing: border-box;

  cursor: pointer;

  transition:
    transform 0.25s ease,
    opacity 0.25s ease;

}


/* 缩略图 */

.photography-frame img {

  width: 100%;
  height: 100%;

  object-fit: cover;

  display: block;

}


/* ================================
   鼠标经过
   ================================ */

.photography-frame:hover {

  transform: translateY(-7px);

  z-index: 5;

}


/* 其他照片稍微变淡 */

.photography-film:hover
.photography-frame:not(:hover) {

  opacity: 0.65;

}


/* ================================
   编号
   ================================ */

.photography-number {

  position: absolute;

  bottom: -24px;

  left: 50%;

  transform: translateX(-50%);

  color: #999;

  font-size: 10px;

  letter-spacing: 1px;

  white-space: nowrap;

}


/* ================================
   底部文字
   ================================ */

.photography-caption {

  text-align: center;

  margin-top: 35px;

  color: #888;

  font-size: 13px;

  letter-spacing: 2px;

}


/* ================================
   手机端
   ================================ */

@media (max-width: 768px) {

  .photography-section {

    margin-top: 70px;

    padding-top: 40px;

  }

  .photography-section h2 {

    font-size: 30px;

  }

  .photography-preview {

    width: 90%;

  }

  .photography-frame {

    width: 120px;

    height: 82px;

  }

}

</style>


<section class="photography-section">

  <h2>Photography</h2>

  <p class="photography-intro">
    Moments seen through my lens.
  </p>


  <!-- ================================
       大图显示
       ================================ -->

  <div class="photography-preview">

    <img
      id="photography-large-image"
      src="/assets/images/photography/photo1.jpg"
      alt="Photography"
    >

  </div>


  <!-- ================================
       胶片
       ================================ -->

  <div class="photography-film-wrapper">

    <div class="photography-film">


      <!-- Photo 01 -->

      <div
        class="photography-frame"
        data-photo="/assets/images/photography/photo1.jpg"
      >

        <img
          src="/assets/images/photography/photo1.jpg"
          alt="Photography 01"
        >

        <span class="photography-number">
          01
        </span>

      </div>


      <!-- Photo 02 -->

      <div
        class="photography-frame"
        data-photo="/assets/images/photography/photo2.jpg"
      >

        <img
          src="/assets/images/photography/photo2.jpg"
          alt="Photography 02"
        >

        <span class="photography-number">
          02
        </span>

      </div>


      <!-- Photo 03 -->

      <div
        class="photography-frame"
        data-photo="/assets/images/photography/photo3.jpg"
      >

        <img
          src="/assets/images/photography/photo3.jpg"
          alt="Photography 03"
        >

        <span class="photography-number">
          03
        </span>

      </div>


      <!-- Photo 04 -->

      <div
        class="photography-frame"
        data-photo="/assets/images/photography/photo4.jpg"
      >

        <img
          src="/assets/images/photography/photo4.jpg"
          alt="Photography 04"
        >

        <span class="photography-number">
          04
        </span>

      </div>


      <!-- Photo 05 -->

      <div
        class="photography-frame"
        data-photo="/assets/images/photography/photo5.jpg"
      >

        <img
          src="/assets/images/photography/photo5.jpg"
          alt="Photography 05"
        >

        <span class="photography-number">
          05
        </span>

      </div>


      <!-- Photo 06 -->

      <div
        class="photography-frame"
        data-photo="/assets/images/photography/photo6.jpg"
      >

        <img
          src="/assets/images/photography/photo6.jpg"
          alt="Photography 06"
        >

        <span class="photography-number">
          06
        </span>

      </div>


      <!-- Photo 07 -->

      <div
        class="photography-frame"
        data-photo="/assets/images/photography/photo7.jpg"
      >

        <img
          src="/assets/images/photography/photo7.jpg"
          alt="Photography 07"
        >

        <span class="photography-number">
          07
        </span>

      </div>


      <!-- Photo 08 -->

      <div
        class="photography-frame"
        data-photo="/assets/images/photography/photo8.jpg"
      >

        <img
          src="/assets/images/photography/photo8.jpg"
          alt="Photography 08"
        >

        <span class="photography-number">
          08
        </span>

      </div>


    </div>

  </div>


  <div class="photography-caption">
    Light · Place · Moment
  </div>

</section>


<script>

document
  .querySelectorAll('.photography-frame')
  .forEach(function(frame) {

    frame.addEventListener('mouseenter', function() {

      const image =
        frame.getAttribute('data-photo');

      const largeImage =
        document.getElementById(
          'photography-large-image'
        );

      if (!image || !largeImage) {
        return;
      }

      largeImage.style.opacity = '0';

      setTimeout(function() {

        largeImage.src = image;

        largeImage.style.opacity = '1';

      }, 120);

    });

  });

</script>
