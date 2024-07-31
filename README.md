𝐒𝐀𝐒𝐀𝐊𝐈-𝐌𝐃

<!DOCTYPE html>
<html>
<head>
<title>Codeflash - Web Page Animation</title>
<style>

*{
  padding:0;
  margin:0;
}

 body{
  width:100%;
  height:100vh;
}

 .bgimage{
  background-image: url("https://i.ibb.co/crM4svf/bg.jpg");
  background-size: cover;
}

 .page{
  background-size: cover;
  height:100vh;
  align-items:center;
  justify-content:center;
  display:flex;
  flex-direction:column;
  color:#F1F1F1;
  background-color: rgba(0,0,0, 0.3);
}

 /*
Text animations code
*/

 .page h1,p{
  padding:10px 20px;
}

 .pagetextanimation{
  position: relative;
  letter-spacing: 4px;
  overflow: hidden;
  background: linear-gradient(90deg, #f1f1f1, #f1f1f1, #f1f1f1);
  background-repeat: no-repeat;
  background-size: 80%;
  animation: animate 6s linear infinite;
  -webkit-background-clip: text;
  -webkit-text-fill-color: rgba(255, 255, 255, 0);
}

 @keyframes animate {
  0% {
    background-position: -500%;
  }
  100% {
    background-position: 500%;
  }
}

  /*
Arrow css codes
*/

 .arrow {
  margin: 0 auto;
  text-align: center;
}

   .arrow::after {
  content: "";
  width: 20px;
  height: 20px;
  margin: 70vh auto;
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  border-right: 4px solid #f1f1f1;
  border-bottom: 4px solid #f1f1f1;
  transform: rotate(45deg);
  animation: 1.5s arrow infinite ease;
}

   @keyframes arrow {
  0%,
  100% {
    top: 50px;
  }

     50% {
    top: 80px;
  }
}

</style>
</head>
<body>

 <!-- Background image div -->
<div class="bgimage">
  <!-- Page div -->
  <div class="page" id="pageid" align="center" >
    <!-- Welcome text -->
    <h1><font color="#FF9800" >&lt;</font>Welcome<br>to<br>Codeflash<font color="#FF9800" >/&gt;</font></h1>
    <!-- Slide text -->
    <p><span class="pagetextanimation">Get started with HTML, CSS and JAVASCRIPT today. Never give up unless you are the BEST.</span></p>
    <!-- Arrow -->
    <div class="arrow" onclick="test()"></div>
  </div>
</div>

 </body>
</html>


