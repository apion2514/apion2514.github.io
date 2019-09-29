---
title: 테라서비스 농가용 웹사이트
image: /assets/img/portfolio/terraservice1.jpg
description: >
  테라서비스 농가용 사이트
---

테라서비스 농가용 사이트

 {{ imageNumber }}


<div>
  <img src="/assets/img/portfolio/terraservice1.jpg" width="20%" onclick="changePopup(true ,1)"/>
  <img src="/assets/img/portfolio/terraservice2.jpg" width="20%" onclick="changePopup(true ,2)"/>
  <img src="/assets/img/portfolio/terraservice3.jpg" width="20%" onclick="changePopup(true ,3)"/>
  <img src="/assets/img/portfolio/terraservice4.jpg" width="20%" onclick="changePopup(true ,4)"/>
  <img src="/assets/img/portfolio/terraservice5.jpg" width="20%" onclick="changePopup(true ,5)"/>
</div>

<div class="popup-bg hidden" onclick="changePopup(false)">
  <div class="popup">
    <img class="popupImg" src=""/>
  </div>
</div>

<script>
  var imageLink = '/assets/img/portfolio/terraservice';
  var imageNumber = 1;
  var isPopup = false;

  function changePopup(value, number) {
    var item = document.querySelector('popup-bg');

    if (value === true && isPopup === true) {
      changeNumber(number);
    } else if (value === true && isPopup === false) {
      item.className.replaceAll(' hidden', '');

      isPopup = true;
    } else if (value === false) {
      item.className += ' hidden';

      isPopup = false;
    }
  }

  function changeNumber(number) {
    imageNumber = number;

    document.querySelector('.popupImg').src = imageLink + imageNumber + '.jpg';
  }
</script>
