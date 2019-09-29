---
title: 테라서비스 농가용 웹사이트
---

테라서비스 농가용 사이트

<img id="mainImg" src="/assets/img/portfolio/terraservice1.jpg" width="100%"/>


<table>
  <tr>
    <td>
      <img src="/assets/img/portfolio/terraservice1.jpg" onclick="changeImage(1)"/>
    </td>
    <td>
      <img src="/assets/img/portfolio/terraservice2.jpg" onclick="changeImage(2)"/>
    </td>
    <td>
      <img src="/assets/img/portfolio/terraservice3.jpg" onclick="changeImage(3)"/>
    </td>
    <td>
      <img src="/assets/img/portfolio/terraservice4.jpg" onclick="changeImage(4)"/>
    </td>
    <td>
      <img src="/assets/img/portfolio/terraservice5.jpg" onclick="changeImage(5)"/>
    </td>
  </tr>
</table>

<script>
  var imageLink = '/assets/img/portfolio/terraservice';
  var imageNumber = 1;

  function changeNumber(number) {
    imageNumber = number;

    document.querySelector('#mainImg').src = imageLink + imageNumber + '.jpg';
  }
</script>
