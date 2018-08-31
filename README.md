# Soundjs

> Soundjs 是处理HTML5的音频audio的JavaScript的库

## 起步

```js
  <body onload="loadSound();">

      // 按钮
      <button onclick="playSound();" class="playSound">开始播放Music</button>

      // 引入js库 soundjs
      <script src="./soundjs.js"></script>

      // js脚本
      <script>

          // music 的id 全局 ## 以后在任意位置可以根据id执行音乐
          var soundID = "timian";

          // 注册audio
          function loadSound() {
              createjs.Sound.registerSound("asserts/timian.mp3", soundID);
          }

          // 播放audio
          function playSound() {
              createjs.Sound.play(soundID);
          }
      </script>
  </body>

```
