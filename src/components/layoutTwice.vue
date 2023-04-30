<template>
    <div class="btn-group">
    <button class="btn btn-secondary btn-lg dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
        charge
    </button>
    <ul class="dropdown-menu">
        <li class="ps-3" v-for="(item, index) in priceArr" :key="index">
            {{ item }}
        </li>
    </ul>
  

  <!-- Large button groups (default and split) -->
<div class="btn-group ms-2">
    <button class="btn btn-secondary btn-lg dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
        concentration
    </button>
    <ul class="dropdown-menu">
      <li class="ps-3">strong</li>
      <li class="ps-3">middle</li>
      <li class="ps-3">light</li>

    </ul>
  </div>
<div class="peace container mt-3">
    <div class="card">
        <img src="@/assets/jager1.png" class="card-img-top" alt="..."  onclick="javascript:window.location.href='wineP2.html'">
        <div class="card-body">
        <h5 class="card-title"><b>Jager</b></h5>
        <p class="card-text">野格是德国人的骄傲，也是国外酒吧广受欢迎的利口酒。 欢迎程度与派对的狂野度成正比。酒精濃度35%</p>
    </div>
    </div>
    <div class="card">
    <img src="@/assets/whisky1.jpg" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title"><b>Balvenie Whisky</b></h5>
      <p class="card-text">Balvenie 百富酒廠由獨立的家族企業擁有與經營，五個世代以來，其家族一直致力於釀製麥芽威士忌的傳統、技藝和管理。 百富能夠在眾多單一麥芽威士忌產品中更顯突出，要歸...。酒精濃度40%</p>
    </div>
   
    </div>
    <div class="card">
        <img src="@/assets/loku1.jpg" class="card-img-top loku2" alt="...">
        <div class="card-body">
        <h5 class="card-title"><b>Loku Gin</b></h5>
        <p class="card-text">六（ROKU）」是琴酒工藝師純熟精確掌握各種原料，以及專注在製程上的細節所誕生的頂級琴酒。ROKU在日文裡代表著「六」，六（ROKU）使用了6種經典的日本植物：櫻花、櫻花葉、日本柚子皮、煎茶、玉露，日本山椒；這些植物都是順應四季時序，在植物最盛開的時候採收並擷取其中的精華及香氣，經過日本大阪三得利烈酒廠的日本琴酒工藝師浸製、蒸餾、最後調和而成。酒精濃度43%</p>
    </div>
    </div>
</div>
<nav aria-label="Page navigation example ">
    <ul class="pagination mt-2 container">
      <li class="page-item">
        <a class="page-link" href="#" aria-label="Previous">
          <span aria-hidden="true">&laquo;</span>
        </a>
      </li>
      <li class="page-item"><a class="page-link" href="#">1</a></li>
      <li class="page-item"><a class="page-link" href="#">2</a></li>
      <li class="page-item"><a class="page-link" href="#">3</a></li>
      <li class="page-item">
        <a class="page-link" href="#" aria-label="Next">
          <span aria-hidden="true">&raquo;</span>
        </a>
      </li>
    </ul>
</nav>
</div>
</template>
<script>
  export default {
    name: 'layoutTwice',
    data(){
        return{
            priceArr: [
                '0~1000',
                '1000~3000',
                '3000up',
            ]
        }
    }
  }
</script>