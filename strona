<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <script
      src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.js"
      integrity="sha512-n/4gHW3atM3QqRcbCn6ewmpxcLAHGaDjpEBu4xZd47N0W2oQ+6q7oc3PXstrJYXcbNU1OHdQ1T7pAP+gi5Yu8g=="
      crossorigin="anonymous"
      referrerpolicy="no-referrer"
    ></script>
    <script>
      $(function () {
        console.log("run3");

        $("#nav-info").click(function () {
          $(".navinfopop").toggleClass("hide");
        });
        $(".navinfopop .close").click(function () {
          $(".navinfopop").toggleClass("hide");
        });
      });

      function ypb(x, z) {
        //console.log("ypb");
        var y = $("#hiddenCurrentNoy").val();
        y = parseInt(y);
        var percentageComplete = x / 100;
        var strokeDashOffsetValue = 100 - percentageComplete * 100;
        var progressBar = $(".js-progress-bar");
        progressBar.css("stroke-dashoffset", strokeDashOffsetValue);
        const obj = document.getElementById("currentNo");
        animateValue(obj, y, x / z, 1000);
        $('input[name="hiddenCurrentNoy"]').val(x / z);
      }

      function ypb2(x, z) {
        //console.log("ypb2");
        var y = $("#hiddenCurrentNoy2").val();
        y = parseInt(y);
        var percentageComplete = x / 100;
        var strokeDashOffsetValue = 100 - percentageComplete * 100;
        var progressBar = $(".js-progress-bar2");
        progressBar.css("stroke-dashoffset", strokeDashOffsetValue);
        const obj = document.getElementById("currentNo2");
        animateValue(obj, y, x / z, 1000);
        $('input[name="hiddenCurrentNoy2"]').val(x / z);
      }

      function rpb(x, z) {
        //console.log("rpb");
        var y = $("#hiddenCurrentNor").val();
        y = parseInt(y);
        var percentageComplete = x / 100;
        var strokeDashOffsetValue = 100 - percentageComplete * 100;
        var progressBar = $(".js-progress-bar3");
        progressBar.css("stroke-dashoffset", strokeDashOffsetValue);
        const obj = document.getElementById("currentNo");
        animateValue(obj, y, x / z, 1000);
        $('input[name="hiddenCurrentNor"]').val(x / z);
      }

      function rpb2(x, z) {
        var y = $("#hiddenCurrentNor").val();
        y = parseInt(y);
        var percentageComplete = x / 100;
        var strokeDashOffsetValue = 100 - percentageComplete * 100;
        var progressBar = $(".js-progress-bar4");
        progressBar.css("stroke-dashoffset", strokeDashOffsetValue);
        const obj = document.getElementById("currentNo2");

        animateValue(obj, y, x / z, 1000);
        $('input[name="hiddenCurrentNor2"]').val(x / z);
      }

      function labelChange(x) {
        $("." + x).toggleClass("yellow");
        var i = 0;
        var t = "";

        var aBB = false;
        var aACEI = false;
        var aARB = false;
        var aARNI = false;
        var aMRA = false;
        var aSGLT21 = false;

        aBB = $("#switchBB").is(":checked");
        aACEI = $("#switchACEI").is(":checked");
        aARB = $("#switchARB").is(":checked");
        aARNI = $("#switchARNI").is(":checked");
        aMRA = $("#switchMRA").is(":checked");
        aSGLT21 = $("#switchSGLT21").is(":checked");

        if (!aARB) {
          $("#switchACEI").attr("disabled", false);
          $("#wACEI label").removeClass("dis");
          $("#wACEI span").removeClass("dis");
          $("#switchMRA").attr("disabled", false);
          $("#wMRA label").removeClass("dis");
          $("#wMRA span").removeClass("dis");
          $("#switchSGLT21").attr("disabled", false);
          $("#wSGLT21 label").removeClass("dis");
          $("#wSGLT21 span").removeClass("dis");
          $("#switchARNI").attr("disabled", false);
          $("#wARNI label").removeClass("dis");
          $("#wARNI span").removeClass("dis");
        }

        if (!aACEI) {
          $("#switchARB").attr("disabled", false);
          $("#wARB label").removeClass("dis");
          $("#wARB span").removeClass("dis");
          $("#switchSGLT21").attr("disabled", false);
          $("#wSGLT21 label").removeClass("dis");
          $("#wSGLT21 span").removeClass("dis");
          $("#switchARNI").attr("disabled", false);
          $("#wARNI label").removeClass("dis");
          $("#wARNI span").removeClass("dis");
        }
        if (!aARNI) {
          $("#switchARB").attr("disabled", false);
          $("#wARB label").removeClass("dis");
          $("#wARB span").removeClass("dis");
          $("#switchACEI").attr("disabled", false);
          $("#wACEI label").removeClass("dis");
          $("#wACEI span").removeClass("dis");
        }
        if (!aSGLT21) {
          $("#switchARB").attr("disabled", false);
          $("#wARB label").removeClass("dis");
          $("#wARB span").removeClass("dis");
          $("#switchACEI").attr("disabled", false);
          $("#wACEI label").removeClass("dis");
          $("#wACEI span").removeClass("dis");
        }

        if (aBB) {
          $("#switchMRA").attr("disabled", true);
          $("#wMRA label").addClass("dis");
          $("#wMRA span").addClass("dis");
          $("#switchSGLT21").attr("disabled", true);
          $("#wSGLT21 label").addClass("dis");
          $("#wSGLT21 span").addClass("dis");
        }

        if (aACEI) {
          $("#switchARB").attr("disabled", true);
          $("#wARB label").addClass("dis");
          $("#wARB span").addClass("dis");
          $("#switchSGLT21").attr("disabled", true);
          $("#wSGLT21 label").addClass("dis");
          $("#wSGLT21 span").addClass("dis");
          $("#switchARNI").attr("disabled", true);
          $("#wARNI label").addClass("dis");
          $("#wARNI span").addClass("dis");
        }

        if (aACEI && !aBB) {
          $("#switchMRA").attr("disabled", true);
          $("#wMRA label").addClass("dis");
          $("#wMRA span").addClass("dis");
        }
        if ((aACEI && aBB) || (aARNI && aBB)) {
          $("#switchMRA").attr("disabled", false);
          $("#wMRA label").removeClass("dis");
          $("#wMRA span").removeClass("dis");
        }
        if (aMRA && aBB && aARNI) {
          $("#switchSGLT21").attr("disabled", false);
          $("#wSGLT21 label").removeClass("dis");
          $("#wSGLT21 span").removeClass("dis");
        }
        if (aARB) {
          $("#switchACEI").attr("disabled", true);
          $("#wACEI label").addClass("dis");
          $("#wACEI span").addClass("dis");
          $("#switchMRA").attr("disabled", true);
          $("#wMRA label").addClass("dis");
          $("#wMRA span").addClass("dis");
          $("#switchSGLT21").attr("disabled", true);
          $("#wSGLT21 label").addClass("dis");
          $("#wSGLT21 span").addClass("dis");
          $("#switchARNI").attr("disabled", true);
          $("#wARNI label").addClass("dis");
          $("#wARNI span").addClass("dis");
        }
        if (aARNI) {
          $("#switchARB").attr("disabled", true);
          $("#wARB label").addClass("dis");
          $("#wARB span").addClass("dis");
          $("#switchACEI").attr("disabled", true);
          $("#wACEI label").addClass("dis");
          $("#wACEI span").addClass("dis");
        }

        if (aSGLT21) {
          $("#switchACEI").attr("disabled", true);
          $("#wACEI label").addClass("dis");
          $("#wACEI span").addClass("dis");
          $("#switchARB").attr("disabled", true);
          $("#wARB label").addClass("dis");
          $("#wARB span").addClass("dis");
        }

        if (!aARNI && !aBB && !aMRA && !aSGLT21 && !aACEI && !aARB) {
          $("#switchMRA").attr("disabled", true);
          $("#wMRA label").addClass("dis");
          $("#wMRA span").addClass("dis");
          $("#switchSGLT21").attr("disabled", true);
          $("#wSGLT21 label").addClass("dis");
          $("#wSGLT21 span").addClass("dis");
          $("#switchARNI").attr("disabled", true);
          $("#wARNI label").addClass("dis");
          $("#wARNI span").addClass("dis");
        }

        if (aARNI && aBB && aMRA && aSGLT21) {
          i = 61;
          t =
            '<hr class="">BB+ARNI+MRA+SGLT2I<br><span class="fs40">(HR 0.39, 95% CI: 0.31-0.49)</span>';
        } else if (aARNI && aBB && aMRA) {
          i = 56;
          t =
            '<hr class="">BB+ARNI+MRA<br><span class="fs40">(HR 0.44, 95% CI: 0.37-0.54)</span>';
        } else if (aACEI && aBB && aMRA) {
          i = 48;
          t =
            '<hr class="">ACEI+BB+MRA<br><span class="fs40">(HR 0.52, 95% CI: 0.44-0.61)</span>';
        } else if (aARNI && aBB) {
          i = 42;
          t =
            '<hr class="">BB+ARNI<br><span class="fs40">(HR 0.58, 95% CI: 0.50-0.68)</span>';
        } else if (aACEI && aBB) {
          i = 31;
          t =
            '<hr class="">ACEI+BB<br><span class="fs40">(HR 0.69, 95% CI: 0.61-0.77)</span>';
        } else if (aARB && aBB) {
          i = 26;
          t =
            '<hr class="">ARB+BB<br><span class="fs40">(HR 0.74, 95% CI: 0.66-0.82)</span>';
        } else if (aBB) {
          i = 22;
          t =
            '<hr class="">BB<br><span class="fs40">(HR 0.78, 95% CI: 0.72-0.84)</span>';
        } else if (aACEI) {
          i = 11;
          t =
            '<hr class="">ACEI<br><span class="fs40">(HR 0.89, 95% CI: 0.82-0.96)</span>';
        } else if (aARB) {
          i = 5;
          t =
            '<hr class="">ARB<br><span class="fs40">(HR 0.95, 95% CI: 0.88-1.02)</span>';
        }

        ypb(i, 1);

        $("#bcinfo").html(t);
      }

      function ccChange(x) {
        var t = '<hr class="yellow">ACEI';
        var s = '<hr class="yellow">ARNI';

        if ($("#switch1").is(":checked")) {
        } else {
          $(".cctogbb").addClass("hide");
        }

        switch (x) {
          case 1:
            $(".switch1").toggleClass("yellow");
            if ($("#switch1").is(":checked")) {
              $("#switch1").prop("checked", false);
            } else {
              $("#switch1").prop("checked", true);
            }
            $(".switch2").removeClass("yellow");
            $(".switch2").prop("checked", false);
            $(".cctogbb").toggleClass("hide");
            $(".cctogmra").addClass("hide");
            t =
              '<hr class="yellow">ACEI+BB<br><span class="fs40">(HR 0.69, 95% CI: 0.61-0.77)</span>';
            s =
              '<hr class="yellow">ARNI+BB<br><span class="fs40">(HR 0.58, 95% CI: 0.50-0.68)</span>';
            ypb(31, 1);
            ypb2(42, 1);
            break;
          case 2:
            $(".switch2").toggleClass("yellow");
            if ($("#switch2").is(":checked")) {
              $(".switch2").prop("checked", false);
            } else {
              $(".switch2").prop("checked", true);
            }
            $(".switch1").removeClass("yellow");
            $("#switch1").prop("checked", false);
            $(".cctogbb").addClass("hide");
            $(".cctogmra").toggleClass("hide");
            t =
              '<hr class="yellow">ACEI+BB+MRA<br><span class="fs40">(HR 0.52, 95% CI: 0.44-0.61)</span>';
            s =
              '<hr class="yellow">ARNI+BB+MRA<br><span class="fs40">(HR 0.44, 95% CI: 0.37-0.54)</span>';
            ypb(48, 1);
            ypb2(56, 1);
            break;
        }

        if ($("#switch2").is(":checked") || $("#switch1").is(":checked")) {
        } else {
          var t = '<hr class="yellow">ACEI';
          var s = '<hr class="yellow">ARNI';

          ypb(0, 1);
          ypb2(0, 1);
          $(".cctogbb").addClass("hide");
          $(".cctogmra").addClass("hide");
        }

        $("#ccinf1").html(t);
        $("#ccinf2").html(s);
      }

      function yearsChange(x) {
        var t = "";
        var s = "";

        switch (x) {
          case 1:
            $(".yellow2").toggleClass("hide");
            break;
          case 2:
            $(".yellow3").toggleClass("hide");
            $(".y3").toggleClass("yel");

            break;
        }
        if ($("#ccMRA").is(":checked") && $("#ccBB").is(":checked")) {
          $(".nogap").addClass("hide");
          $(".achidden").removeClass("hide");
          $("#c1y").removeClass("hide");
          $("#c1g").removeClass("hide");
          $("#c2y").removeClass("hide");
          $("#c2g").removeClass("hide");

          $("#acinf1").addClass("hide");
          $("#acinf2").addClass("hide");
          $(".yesgap").removeClass("hide");
        } else {
          $(".nogap").removeClass("hide");
          $(".achidden").addClass("hide");
          $("#c1y").addClass("hide");
          $("#c1g").addClass("hide");
          $("#c2y").addClass("hide");
          $("#c2g").addClass("hide");
          $("#acinf1").removeClass("hide");
          $("#acinf2").removeClass("hide");
          $(".yesgap").addClass("hide");
        }

        switch (x) {
          case 1:
            if (!$("#ccBB").is(":checked")) {
              console.log("here");
              ypb(0.1, 1);
              ypb2(0.1, 1);
              $("#circ1").css({ transform: "rotate(0deg)" });
              $("#circ1 .circ").css({ transform: "rotate(0deg)" });
              $("#circ2").css({ transform: "rotate(0deg)" });
              $("#circ2 .circ").css({ transform: "rotate(0deg)" });
            } else {
              ypb(55, 11);
              ypb2(80, 10);
              $("#circ1").css({ transform: "rotate(210deg)" });
              $("#circ1 .circ").css({ transform: "rotate(-210deg)" });
              $("#circ2").css({ transform: "rotate(305deg)" });
              $("#circ2 .circ").css({ transform: "rotate(-305deg)" });
              t = "(95% CI: 1.4-8.4)";
              s = "(95% CI: 4.7-11.2)";
            }

            if ($("#ccMRA").is(":checked")) {
              rpb(40, 11);
              rpb2(55, 11);
            }
            break;
          case 2:
            if (!$("#ccMRA").is(":checked")) {
              console.log("here1");
              rpb(0.1, 1);
              rpb2(0.1, 1);
              $("#circ3").css({ transform: "rotate(0deg)" });
              $("#circ3 .circ").css({ transform: "rotate(0deg)" });
              $("#circ4").css({ transform: "rotate(0deg)" });
              $("#circ4 .circ").css({ transform: "rotate(0deg)" });
            } else {
              rpb(40, 11);
              rpb2(55, 11);
              $("#circ3").css({ transform: "rotate(152deg)" });
              $("#circ3 .circ").css({ transform: "rotate(-152deg)" });
              $("#circ4").css({ transform: "rotate(210deg)" });
              $("#circ4 .circ").css({ transform: "rotate(-210deg)" });
              t = "(95% CI: 0.7-5.8)";
              s = "(95% CI: 2.5-7.5)";
            }

            if ($("#ccBB").is(":checked")) {
              ypb(55, 11);
              ypb2(80, 10);
            }
            break;
        }

        $("#acinf1").html(t);
        $("#acinf2").html(s);
      }

      function spin() {
        console.log("test2");
        $(".parent-circ").css({ transform: "rotate(120deg)" });
        $(".circ").css({ transform: "rotate(-120deg)" });
      }

      function animateValue(obj, start, end, duration) {
        let startTimestamp = null;
        const step = (timestamp) => {
          if (!startTimestamp) startTimestamp = timestamp;
          const progress = Math.min((timestamp - startTimestamp) / duration, 1);
          obj.innerHTML = Math.floor(progress * (end - start) + start);
          if (progress < 1) {
            window.requestAnimationFrame(step);
          }
        };
        window.requestAnimationFrame(step);
      }

      function setTime() {
        ++totalSeconds;
        secondsLabel.innerHTML = pad(totalSeconds % 60);
        minutesLabel.innerHTML = pad(parseInt(totalSeconds / 60));
      }

      function pad(val) {
        var valString = val + "";
        if (valString.length < 2) {
          return "0" + valString;
        } else {
          return valString;
        }
      }
    </script>
    <style>
      * {
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
      }

      @font-face {
        font-family: NewsGothicECB;
        src: url("./NewsGothicBT-BoldExtraCondensed.otf") format("opentype");
      }
      @font-face {
        font-family: NewsGothicECM;
        src: url("./NewsGothicBT-ExtraCondensed.otf") format("opentype");
      }
      @font-face {
        font-family: NewsGothicRC;
        src: url("./News-Gothic-BT-Roman-Condensed-Font.ttf") format("truetype");
      }

      html,
      body {
        margin: 0;
        font-size: 8px;
      }

      .push {
        height: 10.65vw;
      }

      .home .footer p {
        max-width: 100%;
      }

      .NewsGothicECB {
        font-family: NewsGothicECB, sans-serif;
      }
      .NewsGothicECM {
        font-family: NewsGothicECM, sans-serif;
      }

      .txtcenter {
        text-align: center;
      }
      .center {
        margin: 0 auto;
      }
      .txtleft {
        text-align: left;
      }
      .relative {
        position: relative;
      }
      .fs250 {
        font-size: 15.6rem;
      }
      .fs150 {
        font-size: 12rem;
      }
      .fs90 {
        font-size: 5.6rem;
      }
      .fs70 {
        font-size: 4rem;
      }
      .fs60 {
        font-size: 3.75rem;
      }
      .fs55 {
        font-size: 3.4375rem;
      }
      .fs50 {
        font-size: 2.5rem;
      }
      .fs45 {
        font-size: 2.25rem;
      }
      .fs40 {
        font-size: 2rem;
      }
      .fs25 {
        font-size: 1.6rem;
      }
      .footer .fs25 {
        font-size: 1.5rem;
      }

      .yellow {
        color: #ffcd03 !important;
      }
      .yellow2 {
        color: #fadc00;
      }
      .grey {
        color: #808080;
      }
      .black {
        color: #000;
      }
      .gold {
        color: #e1aa1e;
      }

      .btngold {
        background: #e1aa1e;
      }

      .underline {
        border-bottom: 1px solid #ffcd03;
        margin-bottom: 15px;
      }
      hr.yellow {
        border-top: 1px solid #ffcd03;
        margin: 5px 0;
      }

      .container {
        background: #374b5a;
        width: 90.3vw;
        height: 50vw;
        margin: 0 auto;
        color: #fff;
        padding: 5.1vw;
        box-sizing: border-box;
        display: flex;
        column-gap: 3.66vw;
        position: relative;
      }

      .pbtm {
        position: absolute;
        bottom: 0;
      }

      #nav-home {
        background: url("../images/nav-home.png") 50% no-repeat;
        background-size: 100%;
        display: block;
        width: 60px;
        height: 50px;
        margin-top: 10px;
      }
      #nav-back {
        background: url("../images/nav-back.png") 50% no-repeat;
        background-size: 100%;
        display: block;
        width: 60px;
        height: 50px;
        margin-top: 5px;
      }
      #nav-forward {
        background: url("../images/nav-forward.png") 50% no-repeat;
        background-size: 100%;
        display: block;
        width: 60px;
        height: 50px;
        margin-top: 5px;
      }
      #nav-info {
        background: url("../images/nav-info.png") 50% no-repeat;
        background-size: 40%;
        display: block;
        width: 60px;
        height: 50px;
        margin-top: 5px;
      }

      .navinfopop {
        position: absolute;
        top: 0;
        left: 0;
        width: 100vw;
        background-color: rgba(46, 44, 44, 0.76);
        height: calc(100% - 9.26vw);
      }
      .infocon {
        position: relative;
        top: calc(50% - 15vh);
        width: 50%;
        margin: 0 auto;
        height: 33vh;
        background-color: #374b5a;
        border: 1px solid #fff;
        color: #fff;
        padding: 50px 30px;
        box-sizing: border-box;
        font-size: 15px;
      }
      .infocon .close {
        color: white;
        font-size: 20px;
        right: 15px;
      }

      .ac .container {
        padding: 3vw 5.1vw;
      }

      .bc .container {
        padding: 3vw 5.1vw;
      }

      .cc .container {
        padding: 3vw 5.1vw;
      }

      .pri .container {
        background: #fff;
        color: #374b5a;
        display: block;
      }
      .inf .container {
        background: #fff;
        color: #374b5a;
        padding: 3.5vw 5.5vw;
      }

      .close {
        position: absolute;
        right: 25px;
        top: 10px;
        font-size: 60px;
      }

      .pt149 {
        padding: 5vw 0;
      }
      .mt30 {
        margin-top: 30px;
      }
      .mt50 {
        margin-top: 50px;
      }
      .mtb25 {
        margin: 25px 0;
      }
      .w125 {
        width: 125% !important;
      }
      .w100 {
        width: 100%;
      }
      .w50 {
        width: 60%;
      }
      .w40 {
        width: 45%;
      }
      .hide {
        display: none !important;
      }
      .center {
        margin: 0 auto;
      }

      span.outline {
        text-decoration: none;
        border: 1px solid #fff;
        border-radius: 25px;
        padding: 5px 20px;
        color: #fff;
      }

      .bgOpa {
        background-color: rgba(46, 44, 44, 0.76);
      }

      .home .container,
      .home2 .container {
        background: transparent;
      }
      .home2 .container {
        padding: 0 5.1vw 5.1vw;
      }
      .cc .container,
      .ac .container,
      .lb .container,
      .qu .container {
        display: block;
      }

      .home .content {
        width: 49.4vw;
        position: absolute;
        right: 0;
        padding-right: 50px;
      }
      .home2 .content {
        width: 50vw;
      }
      .home2 .content p {
        margin: 0 0 1vw;
      }
      .home2 .content a {
        margin: 0 0 3.5vw;
      }

      .flex {
        display: flex;
        gap: 25px 20px;
        flex-wrap: wrap;
      }
      #board {
        margin-top: 50px;
      }
      #board .col1 {
        width: calc(20% - 10px);
      }
      #board .col2 {
        width: calc(80% - 10px);
      }

      .flex-form {
        display: flex;
        gap: 25px 20px;
        flex-wrap: wrap;
      }
      .flex-form .col1 {
        width: calc(20% - 10px);
      }
      .flex-form .col2 {
        width: calc(80% - 10px);
      }

      .btnwrap {
        display: flex;
        position: absolute;
        right: 20.8vw;
        top: 30%;
      }
      .btn2 {
        width: 3.1vw;
        height: 3.1vw;
        margin: 0 10px;
      }
      .goldbtn {
        background: #ffcd03;
        border-radius: 96px;
        color: #374b5a;
      }

      .box {
        background: #2d3e4c;
        padding: 10px;
      }
      .ac .box {
        border-radius: 15px;
        width: 70%;
        padding: 15px;
      }

      .grid.two {
        display: grid;
        grid-template-columns: 50% 50%;
        margin-bottom: 5px;
      }
      .grid.two.tweak {
        display: grid;
        grid-template-columns: 50px calc(100% - 50px);
        margin-bottom: 5px;
      }
      .grid.two.nogap {
        display: grid;
        grid-template-columns: 30% 70%;
        margin-bottom: 5px;
      }
      .grid.two.legend {
        width: 35%;
      }
      .grid.two.legend label:after {
        display: none;
      }
      .grid.two.tweak span {
        line-height: 25px;
      }
      .grid.three {
        display: grid;
        grid-template-columns: calc(36% - 100px) 32% 32%;
        margin-bottom: 22px;
        grid-column-gap: 50px;
      }
      .grid.three.tweak {
        display: grid;
        grid-template-columns: calc(33% - 20px) calc(33% - 20px) calc(
            33% - 20px
          );
        grid-column-gap: 50px;
      }
      .grid.four {
        display: grid;
        grid-template-columns: 25% 25% 25% 25%;
        margin-bottom: 22px;
      }
      .grid span {
        transition: 0.2s ease color;
      }

      .coll {
        width: 39.7vw;
      }
      .colr {
        width: 35.69vw;
      }

      .p20 {
        padding: 20px;
      }
      .br15 {
        border-radius: 15px;
      }

      .inf ul {
        padding-left: 16px;
      }

      .nova {
        position: absolute;
        bottom: 15px;
        left: 30px;
        width: 8vw;
      }

      .goldline {
        background: #ffcd03;
        color: #374b5a;
        border-radius: 20px;
        padding: 0 10px;
        text-decoration: none;
      }

      .ic1 {
        background: url("../images/ic1.png") 0 0 no-repeat;
        background-size: 60px;
        padding-left: 80px;
      }
      .ic2 {
        background: url("../images/ic2.png") 0 0 no-repeat;
        background-size: 60px;
        padding-left: 80px;
      }

      #ccinf1,
      #ccinf2 {
        margin-top: -15px;
      }

      #c1y {
        position: absolute;
      }
      #c1y:after {
        content: "\25B2";
        display: block;
        color: #fadc00;
        width: 20px;
        height: 20px;
        position: absolute;
        right: 0;
        top: -16px;
      }
      #c1g {
        position: absolute;
        right: -49px;
        bottom: 14px;
      }
      #c1g:after {
        content: "\25B2";
        display: block;
        color: #e1aa1e;
        width: 20px;
        height: 20px;
        position: absolute;
        left: 0;
        top: -17px;
      }
      #c2y {
        position: absolute;
        top: 1.2vh;
        left: -6vh;
      }
      #c2y:after {
        content: "\25bc";
        display: block;
        color: #fadc00;
        width: 20px;
        height: 20px;
        position: absolute;
        right: 0;
        bottom: -14px;
      }
      #c2g {
        position: absolute;
        left: 71px;
        bottom: -28px;
      }
      #c2g:after {
        content: "\25B2";
        display: block;
        color: #e1aa1e;
        width: 20px;
        height: 20px;
        position: absolute;
        left: 0;
        top: -19px;
      }

      .circleprogAssistant hr {
        margin: 8px auto;
        border: 2px solid #fff;
      }
      hr {
        border-top: 0px !important;
      }

      /* Toogle Switches */
      input[type="checkbox"] {
        height: 0;
        width: 0;
        visibility: hidden;
      }
      input[type="checkbox"].show {
        height: auto;
        width: auto;
        visibility: visible;
      }

      .ac label,
      .bc label,
      .cc label {
        cursor: pointer;
        text-indent: -9999px;
        width: 3vw;
        height: 2vw;
        background: #c9c4c4;
        display: block;
        border-radius: 3.66vw;
        position: relative;
        transition: 0.2s ease background;
      }

      label.gold {
        background: #fadc00;
      }
      label.orange {
        background: #e1aa1e;
      }

      span {
        transition: 0.2s ease color;
      }

      label.dis {
        background: #808080;
      }
      span.dis {
        color: #4d4c4c;
      }

      .ac label:after,
      .bc label:after,
      .cc label:after {
        content: "";
        position: absolute;
        top: 1px;
        right: 1.1vw;
        width: 1.8vw;
        height: 1.8vw;
        background: #fff;
        border-radius: 90px;
        transition: 0.3s;
      }
      label.dis:after {
        background: #9b9b9b;
      }

      .bc label.active:after,
      .bc label.notav:after {
        display: none;
      }
      .bc label.active,
      .cc label.active {
        background: #ffcd03;
      }
      .bc label.notav,
      .cc label.notav {
        background: #808080;
      }

      input:checked + label {
        background: #ffcd03;
      }

      input:checked + label:after {
        right: 2px;
      }

      label:active:after {
        width: 1.8vw;
      }

      /* Circle Animations */
      .circleprogAssistant {
        width: 35.69vw;
        text-align: center;
        padding: 15px;
        background-color: #374b5a;
        position: relative;
      }
      .cc .circleprogAssistant,
      .ac .circleprogAssistant {
        width: 25.6vw;
        padding: 0;
      }
      #circleContent {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 58%;
      }
      .ac #circleContent {
      }

      .circleprog {
        height: 35.69vw;
        width: 35.69vw;
        transform: rotate(-90deg);
      }
      .cc .circleprog,
      .ac .circleprog {
        height: 25.6vw;
        width: 25.6vw;
      }

      .progress-bar__background {
        fill: none;
        stroke: #97a4ae;
        stroke-width: 4px;
      }

      .progress-bar__progress {
        fill: none;
        stroke: #ffcd03;
        stroke-dasharray: 100 100;
        stroke-dashoffset: 100;
        stroke-linecap: round;
        stroke-width: 4px;
        -webkit-transition: stroke-dashoffset 1s ease-in-out;
        transition: stroke-dashoffset 1s ease-in-out;
        stroke-dashoffset: 99.9px;
      }
      .progress-bar__progress.y2 {
        stroke: #fadc00;
      }
      .progress-bar2__progress {
        fill: none;
        stroke: #f15b56;
        stroke-dasharray: 100 100;
        stroke-dashoffset: 100;
        stroke-linecap: round;
        stroke-width: 4px;
        -webkit-transition: stroke-dashoffset 1s ease-in-out;
        transition: stroke-dashoffset 1s ease-in-out;
        stroke-dashoffset: 99.9px;
      }

      .progress-bar2__progress.y3 {
        stroke: #e1aa1e;
      }

      .progress-bar2__progress.yel {
        opacity: 0;
      }

      .circ {
        display: block;
        width: 2.9vw;
        height: 2.9vw;
        background: #090;
        position: absolute;
        border-radius: 2.9vw;
        transition: transform 1s ease-in-out;
        top: 1px; /* -child size/2 */
        left: 11.6vw; /* parent size/2 - child size/2 */
      }

      .circ.yellow {
        background: #ffe285;
      }
      .circ.yellow2 {
        background: #fced80;
      }
      .circ.yellow3 {
        background: #f0d48f;
      }
      .circ.red {
        background: #f8adab;
      }

      .circ .txt1 {
        font-size: 2em;
        color: #374b5a;
        display: block;
      }
      .circ .txt2 {
        font-size: 1.25em;
        color: #374b5a;
        display: block;
        margin-top: -15px;
      }

      .parent-circ {
        width: 25.6vw;
        height: 25.6vw;
        position: absolute;
        top: 0;
        border-radius: 50%;
        transform: rotate(0deg);
        transition: transform 1s ease-in-out;
      }

      .form-control-670 {
        --form-control-color: #374b5a;
        display: grid;
        grid-template-columns: 1em auto;
        gap: 0.5em;
        margin-bottom: 25px;
        line-height: 3.125rem;
      }

      .form-control-670 input {
        -webkit-appearance: none;
        appearance: none;
        background-color: #fff;
        margin: 0;
        font: inherit;
        color: #fff;
        width: 1.15em;
        height: 1.15em;
        border: 0.15em solid #fff;
        border-radius: 50%;
        transform: translateY(-0.075em);
        display: grid;
        place-content: center;
      }

      input[type="radio"] {
        /* ...existing styles */
        display: grid;
        place-content: center;
      }

      input[type="radio"]::before {
        content: "";
        width: 0.85em;
        height: 0.85em;
        border-radius: 50%;
        transform: scale(0);
        transition: 120ms transform ease-in-out;
        box-shadow: inset 1em 1em var(--form-control-color);
      }

      input[type="radio"]:checked::before {
        transform: scale(1);
      }

      .qu .col2 input[type="text"] {
        border-radius: 96px;
        height: 50px;
        width: 75%;
      }
      .qu .ind {
        padding-left: 20%;
        margin-top: 40px;
      }
      .qu input[type="text"] {
        border: 1px solid #ffcd03;
        background: transparent;
        color: #fff;
        padding: 10px 20px;
      }
      .qu input:focus {
        outline: none;
      }

      .qu ::placeholder {
        color: #9ba5ad;
        opacity: 1;
      }
      .qu :-ms-input-placeholder {
        color: #9ba5ad;
      }
      .qu ::-ms-input-placeholder {
        color: #9ba5ad;
      }

      .toggle {
        --width: 300px;
        --height: calc(var(--width) / 6);

        position: relative;
        display: block;
        width: var(--width);
        height: var(--height);
        box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.3);
        border-radius: var(--height);
        cursor: pointer;
        margin-bottom: 25px;
      }

      .toggle.w450 {
        --width: 450px;
        --height: calc(var(--width) / 9);

        position: relative;
        display: block;
        width: var(--width);
        height: var(--height);
        box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.3);
        border-radius: var(--height);
        cursor: pointer;
        margin-bottom: 25px;
      }

      .toggle input {
        display: none;
      }

      .toggle .slider {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        border-radius: var(--height);
        background-color: transparent;
        transition: all 0.4s ease-in-out;
        border: 1px solid #fff;
        color: #fff;
      }

      .toggle .slider::before {
        content: "\2713";
        position: absolute;
        top: 4px;
        left: 4px;
        width: calc(var(--height) - 8px);
        height: calc(var(--height) - 8px);
        border-radius: calc(var(--height) / 2);
        background-color: #ffcd03;
        transition: all 0.4s ease-in-out;
        color: #374b5a;
        font-size: 4rem;
        font-family: NewsGothicECB, sans-serif;
        text-align: center;
        line-height: 42px;
      }

      .toggle .slider.a::before {
        content: "A";
      }
      .toggle .slider.b::before {
        content: "B";
      }
      .toggle .slider.c::before {
        content: "C";
      }
      .toggle .slider.d::before {
        content: "D";
      }
      .toggle .slider.correct::before {
        content: "";
      }

      .toggle input:checked + .slider,
      .slider.correct {
        background-color: #ffcd03;
        border-color: #ffcd03;
      }
      .toggle input:checked + .slider::before,
      .slider.correct::before {
        content: "";
        color: #ffcd03;
        background: url("../images/tick.png") #fff 50% 50% no-repeat;
        background-size: 24px;
      }
      .toggle input:checked + .slider.incorrect {
        background-color: #808080;
        border-color: #808080;
      }
      .toggle input:checked + .slider.incorrect::before {
        content: "";
        color: #808080;
        background: url("../images/cross.png") #fff 50% 50% no-repeat;
        background-size: 24px;
      }

      .toggle input:checked + .slider::before,
      .slider.correct:before {
        transform: translateX(calc(var(--width) - var(--height)));
      }

      .toggle .labels {
        position: absolute;
        top: 8px;
        left: 0;
        width: 100%;
        height: 100%;
        font-size: 12px;
        font-family: sans-serif;
        transition: all 0.4s ease-in-out;
      }

      .toggle .labels::after {
        content: attr(data-off);
        position: absolute;
        color: #fff;
        opacity: 1;
        transition: all 0.4s ease-in-out;
        right: 0;
        left: 0;
        margin: 0 auto;
        text-align: center;
        line-height: 35px;
        font-size: 2.4rem;
      }

      .toggle .labels::before {
        content: attr(data-on);
        position: absolute;
        color: #ffffff;
        opacity: 0;
        transition: all 0.4s ease-in-out;
        right: 0;
        left: 0;
        margin: 0 auto;
        text-align: center;
        line-height: 35px;
        font-size: 2.4rem;
      }

      .toggle input:checked ~ .labels::after {
        opacity: 0;
      }

      .toggle input:checked ~ .labels::before {
        opacity: 1;
      }

      .lb .leadrow {
        border: 1px solid #ffcd03;
        padding: 10px 30px;
        border-radius: 50px;
        width: 100%;
        font-size: 4rem;
        text-transform: uppercase;
      }

      .w125 {
        width: 125% !important;
        margin-top: 2vh;
      }
      .mtb2vh {
        margin: 2vh 0;
      }

      @media screen and (aspect-ratio: 16/9) {
        .fs250 {
          font-size: 14vh;
        }
        .fs150 {
          font-size: 10vh;
        }
        .fs90 {
          font-size: 5vh;
        }
        .fs70 {
          font-size: 4vh;
        }
        .fs60 {
          font-size: 3.4vh;
        }
        .fs55 {
          font-size: 3vh;
        }
        .fs50 {
          font-size: 2.8vh;
        }
        .fs45 {
          font-size: 2.5vh;
        }
        .fs40 {
          font-size: 2vh;
        }
        .fs25 {
          font-size: 1.1vh;
        }
        .footer .fs25 {
          font-size: 1.1vh;
        }
        .inf .fs50 {
          font-size: 3vh;
        }
        .inf .fs25 {
          font-size: 2vh;
        }
        .inf .footer .fs25 {
          font-size: 1.1vh;
        }
        .footer .novartis {
          top: 2.7vh;
        }

        .home .container,
        .home2 .container {
          height: 47vw;
        }

        .home .pt149 {
          padding: 0;
        }

        .qy .content {
          width: 47vw;
        }

        .ac .container,
        .pri .container {
          height: 75vh;
        }
        .ac .footer,
        .pri .footer {
          height: 17vh;
        }
        .bc .container {
          height: 75vh;
        }
        .bc .footer {
          height: 16vh;
        }
        .cc .container {
          height: 75vh;
        }
        .cc .footer {
          height: 17vh;
        }
        .qu .container,
        .lb .container {
          height: 73vh;
          width: 80vw;
          padding: 3vw;
        }
        .qu .footer {
          height: 14.2vh;
          z-index: 100;
        }
        .lb .footer {
          height: 14vh;
        }
        .lb .container {
          padding: 3vw 9vw 3vw 4vw;
        }
        .flex-form .col2 {
          width: calc(70% - 10px);
        }

        .lb .leadrow {
          font-size: 4vh;
        }

        .ac label,
        .bc label,
        .cc label {
          height: 3vh;
        }
        .ac input[type="checkbox"],
        .bc input[type="checkbox"],
        .cc input[type="checkbox"] {
          margin: 0;
        }
        .ac label:after,
        .bc label:after,
        .cc label:after {
          right: 2.4vh;
          width: 2.8vh;
          height: 2.8vh;
          top: 0;
        }

        .qu .col2 input[type="text"] {
          font-size: 2vh;
          height: 5vh;
        }

        .nova {
          position: absolute;
          bottom: 1.5vh;
          left: 2.5vw;
          width: 6vw;
        }
        .home2 .content a {
          margin: 0 0 3vw;
        }
        .btn {
          font-size: 3vh;
          line-height: 4vw;
        }
        .btnwrap {
          right: 18.8vw;
        }
        .mtb25 {
          margin: 3vh 0;
        }

        .grid.two.tweak {
          display: grid;
          grid-template-columns: 3.5vw calc(100% - 3.5vw);
        }
        .grid.three {
          margin-bottom: 2vh;
        }

        .circleprog {
          height: 55vh;
          width: 55vh;
        }
        .cc .circleprog,
        .ac .circleprog,
        .parent-circ {
          height: 40vh;
          width: 40vh;
        }
        .cc .circleprogAssistant,
        .ac .circleprogAssistant {
          width: 40vh;
        }
        .circ {
          height: 4.4vh;
          width: 4.4vh;
          left: 18vh;
        }
        .circ .txt1 {
          font-size: 1.25vh;
        }
        .circ .txt2 {
          font-size: 1.25vh;
        }

        #c1y:after {
          width: 2vh;
          height: 2vh;
          right: 0;
          top: -2vh;
        }
        #c1g {
          right: 1vh;
          bottom: -3vh;
        }
        #c1g:after {
          width: 2vh;
          height: 2vh;
          left: 0;
          top: -2vh;
        }
        #c2y {
          top: 1vh;
          left: -6vh;
        }
        #c2y:after {
          width: 2vh;
          height: 2vh;
          right: 0;
          bottom: -1.8vh;
        }
        #c2g {
          left: 9vh;
          bottom: -3vh;
        }
        #c2g:after {
          width: 2vh;
          height: 2vh;
          left: 0;
          top: -2vh;
        }

        .toggle {
          --width: 18vw;
        }
        .toggle.w450 {
          --width: 32vw;
        }
        .toggle .slider::before {
          font-size: 4vh;
          line-height: 4.5vh;
        }
        .toggle .labels::after,
        .toggle .labels::before {
          line-height: 4vh;
          font-size: 3vh;
        }
        .toggle.w450 .labels::after,
        .toggle.w450 .labels::before {
          line-height: 5vh;
        }

        .mt50 {
          margin-top: 8vh;
        }
        .flex-form {
          gap: 3vh 3vh;
        }

        span.outline {
          padding: 5px 2vw;
        }
        .grid.three.tweak {
          grid-column-gap: 3vw;
        }
      }

      @media (width: 960px) {
        html {
          font-size: 6px;
        }
        .infocon {
          font-size: 15px;
          height: auto;
        }
        .cc .fs50 {
          font-size: 2.2rem;
        }
        .footer .novartis {
          top: -10px;
        }
        .container {
          margin: 0 75px 0 auto;
        }
        .footer {
          background-size: 182px;
          padding: 1vw 2.56vw;
        }
        .footer .fs25 {
          font-size: 2rem;
        }

        #c1g {
          position: absolute;
          right: 9px;
          bottom: -21px;
        }
        #c2y:after {
          bottom: -20px;
        }
        #c2g {
          left: 54px;
          bottom: -26px;
        }
        #c2y {
          left: -38px;
        }
        .home .content {
          padding-right: 0px;
          top: 10px;
        }

        html sup {
          font-size: 0.5em;
        }
        .home .content {
          width: 47.4vw;
        }
        span.dis {
          color: #808080;
        }
        .bc .coll {
          width: 43vw;
        }
        .bc .coll .fs25,
        .cc .grid.three .fs25 {
          font-size: 2rem;
        }
        .bc .grid.three.tweak {
          grid-column-gap: 37px;
          grid-template-columns: calc(32% - 20px) calc(35% - 20px) calc(
              33% - 20px
            );
        }
        .bc .inf .container {
          margin: 0 auto;
        }

        .bc .inf .container .fs25 {
          font-size: 1.9rem;
        }

        .cc .pushd {
          margin-top: 50px;
        }
        .cc .grid.three {
          grid-template-columns: calc(36% - 57px) 32% 32%;
          grid-column-gap: 30px;
        }
      }
    </style>
  </head>
  <body>
    <div class="wrapper ac pt149">
      <div class="container">
        <div>
          <span class="fs70 NewsGothicECB"
            >Szacuje się, że pacjenci z HFrEF leczeni ENTRESTO<sup>®</sup> żyją dłużej w porównaniu z pacjentami leczonymi ACEI+BB <sup>1,*</sup></span
          >
          <p class="fs40 NewsGothicECM">

            Analiza obejmująca 7 376 pacjentów wykazała, że pacjenci leczeni ACEI+BB w porównaniu z pacjentami leczonymi terapią ARNI+BB+MRA+SGLT2
             żyją dłużej o 4.9 lat lub 7.9 lat w porównaniu z placebo.<sup>1</sup>
          </p>
        </div>

        <div class="grid three">
          <div>
            <p class="fs40 NewsGothicECB">
             Prognozowane wydłużenie życia pacjenta stosującego terapię ARNI+BB+MRA+SGLT2I
            </p>
            <div class="box">
              <span class="NewsGothicECB fs55 switchBB">WIEK</span>
              <hr class="mtb25" />
              <div id="wBB" class="grid two">
                <span class="NewsGothicECB fs55 switchBB">50 LAT</span>
                <div>
                  <input
                    type="checkbox"
                    id="ccBB"
                    onclick="yearsChange(1)"
                  /><label for="ccBB">50 LAT</label>
                </div>
              </div>
              <div id="wMRA" class="grid two">
                <span class="NewsGothicECB fs55 switcMRA">70 LAT</span>
                <div>
                  <input
                    type="checkbox"
                    id="ccMRA"
                    onclick="yearsChange(2)"
                  /><label for="ccMRA">70 LAT</label>
                </div>
              </div>
            </div>
          </div>

          <div>
            <input
              type="hidden"
              id="hiddenCurrentNoy"
              name="hiddenCurrentNoy"
              value="0"
            />
            <input
              type="hidden"
              id="hiddenCurrentNoy2"
              name="hiddenCurrentNoy2"
              value="0"
            />
            <input
              type="hidden"
              id="hiddenCurrentNor"
              name="hiddenCurrentNor"
              value="0"
            />
            <input
              type="hidden"
              id="hiddenCurrentNor2"
              name="hiddenCurrentNor2"
              value="0"
            />

            <div id="circleprogAssistant" class="circleprogAssistant">
              <svg
                id="circleprog"
                class="circleprog"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="-1 -1 34 34"
              >
                <circle
                  cx="16"
                  cy="16"
                  r="15"
                  class="progress-bar__background"
                />
                <circle
                  id="topc"
                  cx="16"
                  cy="16"
                  r="15"
                  class="progress-bar__progress y2 js-progress-bar"
                />
                <circle
                  cx="16"
                  cy="16"
                  r="15"
                  class="progress-bar2__progress y3 js-progress-bar3 yel"
                />
              </svg>
              <div class="parent-circ" id="circ1">
                <div class="circ yellow2 hide">
                  <span class="NewsGothicECB txt1">5</span><br /><span
                    class="NewsGothicECB txt2"
                    >years</span
                  >
                </div>
              </div>
              <div class="parent-circ" id="circ3">
                <div class="circ yellow3 hide">
                  <span class="NewsGothicECB txt1">3</span><br /><span
                    class="NewsGothicECB txt2"
                    >years</span
                  >
                </div>
              </div>
              <div id="circleContent" class="NewsGothicECB fs70">
                <div class="grid two nogap">
                  <span id="currentNo" class="fs90">-</span>
                  <div class="txtleft">
                    LAT<br />
                    <span class="fs25 NewsGothicECB"
                      >PROGNOZOWANE WYDŁUŻENIE ŻYCIA PACJENTA</span
                    >
                  </div>
                </div>
                <div class="yesgap hide fs25 NewsGothicECM">
                  <span class="fs25 NewsGothicECB"
                    >PROGNOZOWANE WYDŁUŻENIE ŻYCIA PACJENTA</span
                  >
                </div>

                <hr />
                <span class="fs40">W PORÓWNANIU Z ARNI+BB+MRA+SGLT2I</span>
                <div id="acinf1" class="fs40"></div>
              </div>

              <div id="c1y" class="hide yellow2 fs40 NewsGothicECB">
                (95% CI: 1.4-8.4)
              </div>

              <div id="c1g" class="hide gold fs40 NewsGothicECB">
                (95% CI: 0.7-5.8)
              </div>
            </div>
          </div>

          <div>
            <div id="circleprogAssistant2" class="circleprogAssistant">
              <svg
                id="circleprog2"
                class="circleprog"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="-1 -1 34 34"
              >
                <circle
                  cx="16"
                  cy="16"
                  r="15"
                  class="progress-bar__background"
                />
                <circle
                  cx="16"
                  cy="16"
                  r="15"
                  class="progress-bar__progress y2 js-progress-bar2"
                />
                <circle
                  cx="16"
                  cy="16"
                  r="15"
                  class="progress-bar2__progress y3 js-progress-bar4 yel"
                />
              </svg>
              <div class="parent-circ" id="circ2">
                <div class="circ yellow2 hide">
                  <span class="NewsGothicECB txt1">8</span><br /><span
                    class="NewsGothicECB txt2"
                    >years</span
                  >
                </div>
              </div>
              <div class="parent-circ" id="circ4">
                <div class="circ yellow3 hide">
                  <span class="NewsGothicECB txt1">5</span><br /><span
                    class="NewsGothicECB txt2"
                    >years</span
                  >
                </div>
              </div>
              <div id="circleContent" class="NewsGothicECB fs70">
                <div class="grid two nogap">
                  <span id="currentNo2" class="fs90">-</span>
                  <div class="txtleft">
                    LAT<br />
                    <span class="fs25 NewsGothicECB"
                      >PROGNOZOWANE WYDŁUŻENIE ŻYCIA PACJENTA</span
                    >
                  </div>
                </div>
                <div class="yesgap hide fs25 NewsGothicECM">
                  <span class="fs25 NewsGothicECB"
                    >PROGNOZOWANE WYDŁUŻENIE ŻYCIA PACJENTA</span
                  >
                </div>
                <hr />
                <span class="fs40">W PORÓWNANIU DO PLACEBO</span>
                <div id="acinf2" class="fs40"></div>
              </div>

              <div id="c2y" class="hide yellow2 fs40 NewsGothicECB">
                (95% CI: 4.7-11.2)
              </div>

              <div id="c2g" class="hide gold fs40 NewsGothicECB">
                (95% CI: 2.5-7.5)
              </div>
            </div>
          </div>
        </div>

        <div class="grid two legend">
          <div class="grid two tweak">
            <div>
              <label class="active gold">50 LAT</label>
            </div>
            <span class="NewsGothicECM fs40">50 LAT</span>
          </div>

          <div class="grid two tweak">
            <div>
              <label class="active orange">70 LAT</label>
            </div>
            <span class="NewsGothicECM fs40">70 LAT</span>
          </div>
        </div>
      </div>
    </div>
  </div>
  <p class="fs5 NewsGothicECM">
    <STRONG> PL2308106320 08/2023 </STRONG> <br>
    <strong>INFORMACJA:</strong>  Oszacowanie oparto na danych z badania BIOSTAT-CHF (BIOlogy Study to TAilored
    Treatment in Chronic Heart Failure) i badania ASIAN-HF (Asian Sudden Cardiac Death in Heart Failure).
    Sudden Cardiac Death in Heart Failure. Na początku badania 5 691
    (77%) pacjentów przyjmowało ACEI/ARB, 6 018 (82%) pacjentów przyjmowało BB, a 4 093 (55%) pacjentów przyjmowało
    (55%) przyjmowało MRA.
    <br />
    <STRONG>Skróty:</STRONG> ACEI, inhibitor konwertazy angiotensyny; ARB,
    ARB, bloker receptora angiotensyny; ARNI, inhibitor neprylizyny receptora angiotensyny; BB, beta-bloker
    inhibitor; BB, beta-bloker; CI, przedział ufności; GDMT,
    ukierunkowana terapia medyczna; HR, współczynnik ryzyka; MRA,
    antagonista receptora mineralokortykoidowego; SGLT2I, inhibitor kotransportera sodowo-glukozowego 2
    inhibitor kotransportera sodowo-glukozowego 2.
    <br />
    <STRONG>REFERENCJE:</STRONG>
     <br> References: 1. Tromp J et al. JACC: Heart Fail. 2022; 10(2): 73-84. <br> Charakterystyka Produktu Leczniczego Entresto</p>
    
  </div>
  
    </p>
</div>

       
       
      </div>
    </div>
  </body>
</html>
