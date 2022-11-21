# -location-based-ar-tutorial-

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <title>Julians Cool Location-based AR.js demo</title>
    <script src="https://aframe.io/releases/1.0.4/aframe.min.js"></script>
    <script src="https://unpkg.com/aframe-look-at-component@0.8.0/dist/aframe-look-at-component.min.js"></script>
    <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar-nft.js"></script>
  </head>

  <body style="margin: 0; overflow: hidden;">
    <a-scene
      vr-mode-ui="enabled: false"
      embedded
      arjs="sourceType: webcam; sourceWidth:1280; sourceHeight:960; displayWidth: 1280; displayHeight: 960; debugUIEnabled: false;"
    >
      <!Julian>
      
           <!-----Kitchen----->
      
      <a-sphere
        radius="0.5"
        color="green"
        gps-entity-place="latitude: 48.983683486961944; longitude: 12.056433536176693;"
      ></a-sphere>
      
      <a-text
        value="This content will always face you"
        look-at="[gps-camera]"
        scale="50 50 50"
           gps-entity-place="latitude: 48.983683486961944; longitude: 12.056433536176693;"
      ></a-text>
     
      <!Enter your name here>

      <!Add objects above here!>
      <a-camera gps-camera rotation-reader> </a-camera>
    </a-scene>
  </body>
</html>
