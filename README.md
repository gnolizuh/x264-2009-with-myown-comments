x264-2009-with-myown-comments
===================================
  为了更好的理解AVC编码, 近日花了段时间研读开源编码器[x264](http://www.videolan.org/developers/x264.html)的源码。<br/>
  我对源码的一些重要位置进行了注释, 都是本人自己的理解, 希望您联系我, 我将修改并改进。<br/>
  
### 调试参数
    # 如果需要调试, 请务必加上--no-asm
    x264 -o test.264 foreman_qcif.yuv 176x144 --no-asm --profile baseline

