---
title: 테라서비스 농가용 웹사이트
---

테라서비스 농가용 사이트

<img id="main-img" src="/assets/img/portfolio/terraservice1.jpg" width="100%"/>


<div class="table">
  <div class="tr">
    <div class="td sub-img active" onclick="changeImage(1)">
      <img src="/assets/img/portfolio/terraservice1.jpg"/>
    </div>
    <div class="td sub-img" onclick="changeImage(2)">
      <img src="/assets/img/portfolio/terraservice2.jpg"/>
    </div>
    <div class="td sub-img" onclick="changeImage(3)">
      <img src="/assets/img/portfolio/terraservice3.jpg"/>
    </div>
    <div class="td sub-img" onclick="changeImage(4)">
      <img src="/assets/img/portfolio/terraservice4.jpg"/>
    </div>
    <div class="td sub-img" onclick="changeImage(5)">
      <img src="/assets/img/portfolio/terraservice5.jpg"/>
    </div>
  </div>
</div>

<script>
  var imageLink = '/assets/img/portfolio/terraservice';

  function changeImage(number) {
    var choiceNumber = number - 1;
    var item = document.querySelectorAll('.sub-img');
    var i = 0;

    for (i; i < item.length; i++) {
      item[i].className = 'td sub-img';
    }

    item[choiceNumber].className += ' active';
    document.querySelector('#main-img').src = imageLink + number + '.jpg';
  }
</script>

<style>
.td {
  width: 20%;
}

.td:before {
  background: rgba(140, 140, 140, 0.5);
  content: "";
  display: block;
  position: absolute;
  top: 0;
  bottom: 0;
  left: 5px;
  right: 5px;

  -moz-transition: all .3s linear;
  -webkit-transition: all .3s linear;
  -ms-transition: all .3s linear;
  -o-transition: all .3s linear;
  transition: all .3s linear;
}

.td.active:before {
  background: none;
}
</style>
