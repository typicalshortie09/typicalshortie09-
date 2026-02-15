<!DOCTYPE html>
<html lang="en">
<head>
  <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-6098277355901807"
     crossorigin="anonymous">
     </script>
  <meta name="google-adsense-account" content="ca-pub-6098277355901807">
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Deals & Hot Offers</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f0f2f5;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .ad-container {
      background: #fff;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.1);
      text-align: center;
      width: 360px;
      animation: fadeIn 1.5s ease-in-out;
    }

    h1 {
      font-size: 24px;
      color: #333;
      margin-bottom: 10px;
    }

    p {
      color: #666;
      font-size: 16px;
      margin-bottom: 20px;
    }

    a.cta-button {
      display: inline-block;
      background: #ff5722;
      color: #fff;
      padding: 12px 25px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
      transition: transform 0.3s, background 0.3s;
      margin-bottom: 20px;
    }

    a.cta-button:hover {
      background: #e64a19;
      transform: scale(1.1);
    }

    /* Rotating banners */
    .ad-banner {
      width: 100%;
      height: 100px;
      margin: 15px 0;
      border-radius: 10px;
      background: #f9f9f9;
      border: 2px dashed #ccc;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 14px;
      color: #888;
      overflow: hidden;
      position: relative;
    }

    .banner-slide {
      position: absolute;
      width: 100%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      transition: opacity 1s;
    }

    @keyframes fadeIn {
      0% {opacity: 0; transform: translateY(-20px);}
      100% {opacity: 1; transform: translateY(0);}
    }
  </style>
</head>
<body>

  <div class="ad-container">
    <h1>Hot Deals This Week!</h1>
    <p>Grab amazing offers on products you love. Click below to shop now!</p>

    <!-- Example Affiliate Link Button -->
    <a href="https://www.amazon.com/dp/B08N5WRWNW?tag=exampleaffiliate-20" class="cta-button" target="_blank">
      Shop Now
    </a>

    <!-- Rotating Banner 1 -->
    <div class="ad-banner" id="banner1">
      <div class="banner-slide" style="opacity:1;">
        <a href="https://www.amazon.com/dp/B07FZ8S74R?tag=exampleaffiliate-20" target="_blank">
          <img src="https://via.placeholder.com/300x80?text=Affiliate+Product+1" alt="Affiliate Product 1">
        </a>
      </div>
      <div class="banner-slide" style="opacity:0;">
        <!-- Placeholder for AdSense code -->
        <div id="adsense1">Google AdSense Ad Here</div>
      </div>
      <div class="banner-slide" style="opacity:0;">
        <a href="https://www.amazon.com/dp/B08KH53D3S?tag=exampleaffiliate-20" target="_blank">
          <img src="https://via.placeholder.com/300x80?text=Affiliate+Product+2" alt="Affiliate Product 2">
        </a>
      </div>
    </div>

    <!-- Rotating Banner 2 -->
    <div class="ad-banner" id="banner2">
      <div class="banner-slide" style="opacity:1;">
        <!-- Placeholder for AdSense code -->
        <div id="adsense2">Google AdSense Ad Here</div>
      </div>
      <div class="banner-slide" style="opacity:0;">
        <a href="https://www.amazon.com/dp/B08K2S1NSQ?tag=exampleaffiliate-20" target="_blank">
          <img src="https://via.placeholder.com/300x80?text=Affiliate+Product+3" alt="Affiliate Product 3">
        </a>
      </div>
      <div class="banner-slide" style="opacity:0;">
        <a href="https://www.amazon.com/dp/B07Y2ZHG4M?tag=exampleaffiliate-20" target="_blank">
          <img src="https://via.placeholder.com/300x80?text=Affiliate+Product+4" alt="Affiliate Product 4">
        </a>
      </div>
    </div>

  </div>

  <script>
    // Function to rotate banners
    function rotateBanner(bannerId) {
      const banner = document.getElementById(bannerId);
      const slides = banner.getElementsByClassName('banner-slide');
      let index = 0;

      setInterval(() => {
        slides[index].style.opacity = 0;
        index = (index + 1) % slides.length;
        slides[index].style.opacity = 1;
      }, 3000);
    }

    rotateBanner('banner1');
    rotateBanner('banner2');
  </script>
  <meta name="google-adsense-account" content="ca-pub-6098277355901807">

</body>
</html>
