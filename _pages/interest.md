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
