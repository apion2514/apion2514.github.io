---
title: 테라서비스 농가용 웹사이트
---

테라서비스 농가용 사이트

<img id="main-img" src="/assets/img/portfolio/terraservice1.jpg" width="100%"/>


<div class="table">
  <div class="tr">
    <div class="td active">
      <img src="/assets/img/portfolio/terraservice1.jpg" onclick="changeImage(1)"/>
    </div>
    <div class="td">
      <img src="/assets/img/portfolio/terraservice2.jpg" onclick="changeImage(2)"/>
    </div>
    <div class="td">
      <img src="/assets/img/portfolio/terraservice3.jpg" onclick="changeImage(3)"/>
    </div>
    <div class="td">
      <img src="/assets/img/portfolio/terraservice4.jpg" onclick="changeImage(4)"/>
    </div>
    <div class="td">
      <img src="/assets/img/portfolio/terraservice5.jpg" onclick="changeImage(5)"/>
    </div>
  </div>
</div>

<script>
  var imageLink = '/assets/img/portfolio/terraservice';

  function changeImage(number) {

    var choiceNumber = number - 1;
    var item = document.querySelector('.sub-img');
    var i = 0;

    for (i; i < item.length; i++) {
      item[0].className = 'sub-img'
    }

    item[choiceNumber].className += ' active'

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
  left: 0;
  right: 0;

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
