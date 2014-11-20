x264-2009-with-myown-comments
===================================
  为了更好的理解AVC编码, 近日花了段时间研读开源编码器[x264](http://www.videolan.org/developers/x264.html)的源码。<br/>
  我对源码的一些重要位置进行了注释, 都是本人自己的理解, 如有错误请联系我, 我将修正并改进, 希望能够共同进步。<br/>
  
### 调试参数
    # 如果需要调试, 请务必加上--no-asm
    x264 -o test.264 foreman_qcif.yuv 176x144 --no-asm --profile baseline

### 侧重点
    1. 帧类型决策方式
    2. intra-prediction
    3. inter-prediction
    4. rate-control
    5. 过了一遍transform, quant
