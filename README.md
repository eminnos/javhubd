<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SpicyVibescdn</title>

<style>
html, body {
  margin: 0;
  padding: 0;
  background: #000;
  font-family: Arial, Helvetica, sans-serif;
  user-select: none;
}

.page {
  width: 100%;
  background: #000;
}

/* Banner wrapper */
.banner {
  width: 100%;
  display: flex;
  justify-content: center;
  padding: 12px 0;
  background: #000;
}

.video-box {
  width: 100%;
  display: flex;
  justify-content: center;
  background: #000;
}

video {
  width: 100%;
  max-height: 78vh;
  object-fit: contain;
  background: #000;
  pointer-events: auto;
}

* {
  -webkit-tap-highlight-color: transparent;
}
</style>
</head>

<body oncontextmenu="return false">

<div class="page">

  <!-- VIDEO -->
  <div class="video-box">
    <video id="player"
      controls
      autoplay
      playsinline
      preload="metadata"
      controlslist="nodownload nofullscreen noremoteplayback"
      disablepictureinpicture
      ondragstart="return false"
    >
      <source id="videoSource" src="" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <!-- BANNER BOTTOM 320x50 -->
  <div class="banner">
    <script>
  atOptions = {
    'key' : '833cefaa22305c19bca4730dded58f3c',
    'format' : 'iframe',
    'height' : 50,
    'width' : 320,
    'params' : {}
  };
</script>
<script src="https://lentattire.com/833cefaa22305c19bca4730dded58f3c/invoke.js"></script>
  </div>

</div>

<!-- AUTO LOAD VIDEO DARI PARAMETER ?v= -->
<script>
(function () {
  const params = new URLSearchParams(window.location.search);
  let video = params.get("v");

  if (video) {
    if (!video.startsWith("http")) {
      video = "https://cdn.videy.co/" + video;
    }
    document.getElementById("videoSource").src = video;
  } else {
    document.getElementById("videoSource").src = "https://cdn.videy.co/HAZ79zvC1.mp4";
  }

  document.getElementById("player").load();
})();
</script>

<!-- PROTEKSI BASIC -->
<script>
(function () {
  document.addEventListener("contextmenu", e => e.preventDefault());
  document.addEventListener("dragstart", e => e.preventDefault());

  document.addEventListener("keydown", function (e) {
    if (e.key === "F12") e.preventDefault();
    if (e.ctrlKey && e.shiftKey && ["I","J","C"].includes(e.key.toUpperCase())) e.preventDefault();
    if (e.ctrlKey && ["U","S","P"].includes(e.key.toUpperCase())) e.preventDefault();
  });
})();
</script>

</body>
</html>
