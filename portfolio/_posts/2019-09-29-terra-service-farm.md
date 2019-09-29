---
title: 테라서비스 농가용 웹사이트
image: /assets/img/portfolio/terraservice1.jpg
description: >
  테라서비스 농가용 사이트
---

테라서비스 농가용 사이트

 {{ imageNumber }}


<div>
  <img src="/assets/img/portfolio/terraservice1.jpg" width="20%" onclick="changeNumber(1)"/>
  <img src="/assets/img/portfolio/terraservice2.jpg" width="20%" onclick="changeNumber(2)"/>
  <img src="/assets/img/portfolio/terraservice3.jpg" width="20%" onclick="changeNumber(3)"/>
  <img src="/assets/img/portfolio/terraservice4.jpg" width="20%" onclick="changeNumber(4)"/>
  <img src="/assets/img/portfolio/terraservice5.jpg" width="20%" onclick="changeNumber(5)"/>
</div>

<div class="popup-bg hidden">
  <div class="popup">
    <img class="popupImg" src=""/>
  </div>
</div>

<script>
  var imageLink = '/assets/img/portfolio/terraservice';
  var imageNumber = 1;

  function changeNumber(number) {
    imageNumber = number;

    document.querySelector('.popupImg').src = imageLink + imageNumber + '.jpg';
  }
</script>
