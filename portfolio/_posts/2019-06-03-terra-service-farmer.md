---
title: 테라서비스-농가 홈페이지
image: /assets/img/portfolio/terra-service/terra-service1.jpg
description: >
  테라서비스 농가용 홈페이지 입니다.
tags: [Java, JSP, HTML, CSS, JavaScript]
---
<div class="portfolio portfolio-image">
  <img id="main-img" src="/assets/img/portfolio/terra-service/terra-service1.jpg" width="100%"/>

  <div class="table">
    <div class="tr td-5">
      <div class="td sub-img active" onclick="changeImage(1)">
        <img src="/assets/img/portfolio/terra-service/terra-service1.jpg"/>
      </div>
      <div class="td sub-img" onclick="changeImage(2)">
        <img src="/assets/img/portfolio/terra-service/terra-service2.jpg"/>
      </div>
      <div class="td sub-img" onclick="changeImage(3)">
        <img src="/assets/img/portfolio/terra-service/terra-service3.jpg"/>
      </div>
      <div class="td sub-img" onclick="changeImage(4)">
        <img src="/assets/img/portfolio/terra-service/terra-service4.jpg"/>
      </div>
      <div class="td sub-img" onclick="changeImage(5)">
        <img src="/assets/img/portfolio/terra-service/terra-service5.jpg"/>
      </div>
    </div>
  </div>
</div>

<div class="portfolio portfolio-description">
  <span>테라서비스-농가 홈페이지는 테라서비스에 속해있는 홈페이지로 농가 유저를 위한 홈페이지 입니다.</span>

  <div class="portfolio-description-comment">* [테라서비스]는 농작물 재배 도중 발생되는 각종 문제들에 효과적으로 대응 할 수 있도록 지원하는 서비스입니다.</div>
</div>

<div class="portfolio">
  <div class="portfolio-title">개발 및 유지보수 기간 : </div>
  <div class="portfolio-date">2019.01.09 ~ 2019.06.03</div>
</div>

<div class="portfolio">
  <div class="portfolio-title">홈페이지 경로 : </div>
  <div class="portfolio-link">
    <a href="http://m3f.terra-service.co.kr" title="테라서비스-농가">http://m3f.terra-service.co.kr</a>
  </div>
</div>

<script>
  function changeImage(number) {
    var imageLink = '/assets/img/portfolio/terra-service/terra-service';
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
