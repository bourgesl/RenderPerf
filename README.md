# RenderPerf

Forked from Jetbrains Runtime (OpenJDK derived):
```
https://github.com/JetBrains/JetBrainsRuntime

<JBR_PATH>/test/jdk/performance/client/RenderPerfTest/
```


-----------------------------------------------------------------------
Introduction
-----------------------------------------------------------------------

RenderPerfTest is a set of on-screen rendering microbenchmarks  to
analyze the  performance of Java2D graphical primitives rendering

-----------------------------------------------------------------------
How To Compile
-----------------------------------------------------------------------

```
#> cd RenderPerfTest
```

The benchmark can be compiled by using either ant:
```
#> ant
```
or gnumake (assuming there's 'javac' in the path):
```
#> gnumake
```
The jar files will be generated into RenderPerfTest/dist directory.

-----------------------------------------------------------------------
How To Run RenderPerfTest
-----------------------------------------------------------------------
- Run all tests:
```
#> ant run
```
or
```
#> java -jar dist/RenderPerfTest.jar
```

- Run particular test cases:
```
#> java -jar dist/RenderPerfTest.jar WhiteTextGray ...
```

-----------------------------------------------------------------------
How To Get Help on RenderPerf
-----------------------------------------------------------------------
- Show help on command-line arguments:
```
#> java -jar dist/RenderPerfTest.jar -h

##############################################################
# RenderPerfTest 2023.11
##############################################################
# java ... RenderPerfTest <args>
#
# Supported Arguments <args>:
#
# -h         : display this help
# -v         : set verbose outputs
# -e<mode>   : set execution mode (default: robot) among [robot, buffer, volatile]
#
# -f         : use FPS unit (default)
# -t         : use TIME(ms) unit
#
# -l         : list available graphics configurations
# -g=all|0:0,0:1... : use all or specific graphics configurations
#
# -w<number> : use number of test frames (default: 1)
#
# -n<number> : set number of primitives (default: 1000)
# -r<number> : set number of test repeats (default: 1)
#
# Test arguments: ArgbSurfaceBlitImage ArgbSwBlitImage BgrSurfaceBlitImage BgrSwBlitImage ClipFlatBox ClipFlatBoxAA ClipFlatOval ClipFlatOvalAA FlatBox FlatBoxAA FlatOval FlatOvalAA FlatOval_XOR FlatQuad FlatQuadAA Image ImageAA Image_XOR LargeTextGray LargeTextLCD LargeTextNoAA LinGrad3RotatedOval LinGrad3RotatedOvalAA LinGradRotatedOval LinGradRotatedOvalAA Lines LinesAA Lines_XOR RadGrad3RotatedOval RadGrad3RotatedOvalAA RotatedBox RotatedBoxAA RotatedBox_XOR RotatedOval RotatedOvalAA TextGray TextLCD TextLCD_XOR TextNoAA TextNoAA_XOR TextWiredQuadAABat TextWiredQuadAAMix TextWiredQuadBat TextWiredQuadMix VolImage VolImageAA VolImageFlatBoxAABat VolImageFlatBoxAAMix VolImageFlatBoxBat VolImageFlatBoxMix VolImageTextNoAABat VolImageTextNoAAMix VolImageWiredQuadAABat VolImageWiredQuadAAMix VolImageWiredQuadBat VolImageWiredQuadMix WhiteTextGray WhiteTextLCD 
WhiteTextNoAA WiredBox WiredBoxAA WiredBubbles WiredBubblesAA WiredQuad WiredQuadAA
```
