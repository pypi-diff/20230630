# Comparing `tmp/kraken_build-0.27.4.tar.gz` & `tmp/kraken_build-0.27.5.tar.gz`

```diff
@@ -0,0 +1,104 @@
+00000000: 1f8b 0808 0000 0000 02ff 6b72 616b 656e  ..........kraken
+00000010: 5f62 7569 6c64 2d30 2e32 372e 352e 7461  _build-0.27.5.ta
+00000020: 7200 ed5a e16f e2c6 12cf e7fd 2b46 7e5f  r..Z.o......+F~_
+00000030: 5a09 0c18 0e2e a857 d501 e762 95d8 c890  Z......W...b....
+00000040: bb77 8a28 32f6 02db 60af eb5d 5f0e 55ef  .w.(2...`..]_.U.
+00000050: 7f7f b3b6 9340 daab 9af7 eea2 b6d9 9f22  .....@........."
+00000060: 85dd 9dfd cdec b0eb 9d19 6cb6 ccd6 0fd3  ..........l.....
+00000070: f0d3 050d 639a 9f7c 15b4 2b7c ee7f bbdd  ....c..|..+|....
+00000080: ed3e 7c56 fd9d b6d5 e99c c0a7 9367 4021  .>|V.........g@!
+00000090: 6498 a3fa 9397 096b 0089 6409 7dd3 e9bf  d......k..d.}...
+000000a0: 1e58 fd9e d5ef 9bed b635 e8be 2227 1aff  .X.......5.."'..
+000000b0: 7cdc e4e1 0d4d 97ab 82ed e266 dbb4 06e6  |....M.....f....
+000000c0: abd6 c41d 39de ccf9 a2e7 bfdf eb7d eefc  ....9........}..
+000000d0: 7706 bdfe a3f3 6f75 7add 1368 ebf3 ffd5  w.....ouz..h....
+000000e0: 71e9 ce61 c222 9a0a 4ac8 8867 fb9c 6db6  q..a."..J..g..m.
+000000f0: 12be 89be 05ab 6d75 c163 37bb 5040 c005  ......mu.c7.P@..
+00000100: 8a48 ca52 42a6 344f 9810 8ca7 c004 6c69  .H.RB.4O......li
+00000110: 4e57 7bd8 e461 2a69 dc80 754e 29f0 3544  NW{..a*i..uN).5D
+00000120: db30 dfd0 0648 0e61 ba87 8ce6 0227 f095  .0...H.a.....'..
+00000130: 0c59 cad2 0d84 10a1 3622 b7c8 21f8 5ade  .Y......6"..!.Z.
+00000140: 8639 45c9 1842 2178 c442 2483 9847 4542  .9E..B!x.B$..GEB
+00000150: 5319 4aa5 6ccd 7654 c037 724b c198 d533  S.J.l.vT.7rK...3
+00000160: 8c6f 4b0d 310d 7780 b6dd 75c3 2d93 5b5e  .oK.1.w...u.-.[^
+00000170: 48c8 a990 398b d4fc 060a 44bb 2256 caef  H...9.....D."V..
+00000180: 8677 2c61 35bb a22d d72e 1461 2168 8324  .w,a5..-...a!h.$
+00000190: 3c66 eb7d 0312 5aae 242b 563b 26b6 0d88  <f.}..Z.$+V;&...
+000001a0: 9922 5d15 123b 85ea 2cdd d750 d6b7 780e  ."]..;..,..P..x.
+000001b0: 82ee 766a 710c ad45 4720 3151 eb42 d64c  ..vjq..EG 1Q.B.L
+000001c0: 794e d6be 28f5 dc6e 7952 aabe b71c ddb1  yN..(..nyR......
+000001d0: 2ef2 1415 d172 4ecc d13d a59e 9f69 24b1  .....rN..=...i$.
+000001e0: 87ac f96e c76f d532 229e c64c 592f 8684  ...n.o.2"..LY/..
+000001f0: cc91 255c f18f b474 6cf5 35a6 5ca2 71a5  ..%\...tl.5.\.q.
+00000200: 5b4b 4767 0f5f 5d3d 24b6 215a bba2 b573  [KGg._]=$.!Z...s
+00000210: 5027 4b01 bb88 5a48 b1c2 c391 4a86 cecd  P'K...ZH....J...
+00000220: 785e 2aaa 5774 6faf 898a 2f1c 98f9 e7f3  x^*.Wto.../.....
+00000230: f776 e080 3b83 69e0 bf73 c7ce 180c 7b86  .v..;.i..s....{.
+00000240: 6da3 01ef ddf9 857f 3507 9408 6c6f fe01  m.......5...lo..
+00000250: fc73 b0bd 0ff0 a3eb 8d1b e0fc 7b1a 38b3  .s..........{.8.
+00000260: 19f8 0171 bdd1 e46a ec7a 6fe1 0cc5 3d1f  ...q...j.zo...=.
+00000270: f7a6 8b3b 14b9 e63e 283d 3583 ebcc 14c7  ...;...>(=5.....
+00000280: a513 8c2e b069 9fb9 1377 fea1 01e7 eedc  .....i...w......
+00000290: 5354 e77e 0036 995e 0553 7fe6 a0aa 3172  ST.~.6.^.S....1r
+000002a0: 79ae 771e 20b5 73e9 7873 135c 0ffb c079  y.w. .s.xs.\...y
+000002b0: 870d 985d d893 49c9 6f5f a1a5 81b2 0546  ...]..I.o_.....F
+000002c0: fef4 43e0 bebd 9893 3307 cdb0 cf26 4ec5  ..C.....3....&N.
+000002d0: 8b86 8f26 b67b d980 b17d 69bf 754a 691f  ...&.{...}i.uJi.
+000002e0: 6707 a558 6dca fb0b a7ec 423d 36fe 8de6  g..Xm.....B=6...
+000002f0: aeef a1cd 64ee 07f3 fb09 efdd 99d3 003b  ....d..........;
+00000300: 7067 6acd e781 8fa4 ca51 b836 bf9c 3af2  pgj......Q.6..:.
+00000310: 3dcf a9e6 2a27 c291 afd1 6157 33e7 41fb  =...*'....aW3.A.
+00000320: d8b1 27c8 3353 130f 05cd 3fb8 cacd bf44  ..'.3S....?....D
+00000330: fcd7 fb6d fc67 e9f8 ef59 e2bf d7bf 1bff  ...m.g...Y......
+00000340: 9d76 4f75 00f8 52e3 bfc0 b1c7 978e 99c4  .vOu..R.........
+00000350: cf13 ffb5 adbe f538 feeb b55f e9f8 ef39  .......8..._...9
+00000360: f02f a876 40b3 dc01 8400 5cb7 1743 d84a  ./.v@.....\..C.J
+00000370: 9989 61ab 95ed 3366 f27c d3ca 72ae e28f  ..a...3f.|..r...
+00000380: 562d 1df1 9cb6 9470 e74f 080b 19b7 547c  V-.....p.O....T|
+00000390: 8201 08fe 8590 edc2 886e f90e 2f1c c8c2  .........n../...
+000003a0: e826 dc50 5863 bc71 7d40 be40 33ca b8e5  .&.PXc.q}@.@3...
+000003b0: fa81 6481 da4c fd54 faa2 3075 fd47 d77f  ..d..L.T..0u.G..
+000003c0: eafb ff75 c7b2 3aa7 afcc 7eb7 d7eb f4f5  ...u..:...~.....
+000003d0: 417b a9f7 3f3e c7ab 07b8 2979 b2fb faf5  A{..?>....)y....
+000003e0: 1f6b f0f8 feef b551 5cdf ffcf 80eb ea9b  .k.....Q\.......
+000003f0: 177b 2169 b220 39fd a560 3915 f006 ae8d  .{!i. 9..`9.....
+00000400: 8c53 99ef cbeb d858 904a 7085 f735 c56b  .S.....X.Jp..5.k
+00000410: f90d d4c3 a61a 3693 50f0 141b 61c6 0c42  ......6.P...a..B
+00000420: ae25 e73b b31a 5f90 344c a892 3f0c 340c  .%.;.._.4L..?.4.
+00000430: f291 e665 1d02 07aa 6d67 9098 8a28 6799  ...e....mg...(g.
+00000440: acbb 0d12 1672 cbf3 ca98 df14 a2e0 bbfc  .....r..........
+00000450: fe73 5a0e feb0 4942 b643 8392 efd1 deba  .sZ...IB.C......
+00000460: 2ca3 982e ddb9 814b 0be3 ca90 fbf8 d620  ,......K....... 
+00000470: 75f8 51aa f8f5 ae06 f260 6cab 3256 55b5  u.Q......`l.2VU.
+00000480: 78a2 ba45 1e19 f09f 0589 509d 606b 462b  x..E......P.`kF+
+00000490: eb16 e486 ee6f 791e d7ad 230f 9845 be13  .....oy...#..E..
+000004a0: 0b62 9c15 1b98 e7ca 7fb9 a1b8 eec2 a60d  .b..............
+000004b0: 93db 62a5 cc6e 1dba e8b8 c184 28a8 30c8  ..b..n......(.0.
+000004c0: f8a8 2476 c072 286d d694 8c1f 9318 e482  ..$v.r(m........
+000004d0: 2734 53f1 d693 6706 34e3 8249 9eef 9f6c  '4S...g.4..I...l
+000004e0: fba3 1d61 c634 c32d 44d3 8851 f44b b6c7  ...a.4.-D..Q.K..
+000004f0: 2fb9 5cca 4f5d 7370 2f2b 7661 664a 2a24  /.\.O]sp/+vafJ*$
+00000500: 3a7b 4ba3 1b28 dd8f 9d50 360d 7d3d fd83  :{K..(...P6.}=..
+00000510: e23f 5dff f92b d47f 0ee2 bfc1 a90e 005f  .?]..+........._
+00000520: 6cfc 8797 5ceb f0fe 6b2d 972c 6572 b934  l...\...k-.,er.4
+00000530: b3fd d7a8 ffb4 adc1 a3f3 dfef 0e06 3afe  ..............:.
+00000540: 7b0e 2c97 7520 b65c 1e86 62fa 60bc e0f3  {.,.u .\..b.`...
+00000550: 3ffd f16d d3f5 cefd 2f79 ffff c1f9 b730  ?..m..../y.....0
+00000560: df7b 5cff b5ac b63e ffcf 814b 2ac3 3894  .{\....>...K*.8.
+00000570: 61f3 5df5 1818 8265 7688 8729 dbf0 b832  a.]....ev..)...2
+00000580: 7c3f 5e6d 1232 2b92 24cc f743 20f5 eb03  |?^m.2+.$..C ...
+00000590: 43c0 348b d865 ca36 fc9d f706 aa91 2655  C.4..e.6......&U
+000005a0: 39da 103e 9fbb 61a6 51e5 a0cd 6999 190c  9..>..a.Q...i...
+000005b0: e1fb 3798 1834 beeb 996d 32ba cfbb 8677  ..7..4...m2....w
+000005c0: af2d c070 08fe cc05 3bcb 72fe 91c6 aa7d  .-.p....;.r....}
+000005d0: f856 c3e1 9469 ce37 7998 24ea c7f3 4998  .V...i.7y.$...I.
+000005e0: 6e0a 950a a17c a549 7dea 3e55 de1c 3c79  n....|.I}.>U..<y
+000005f0: c6eb 27cf 387d f28c 4efb e953 3a64 5ad5  ..'.8}..N..S:dZ.
+00000600: 7d9a 57c1 6408 07f9 6a03 fe87 64f5 98ed  }.W.d...j...d...
+00000610: 2871 7de0 fb33 c9e7 31d1 5d0a fbff 703c  (q}..3..1.]...p<
+00000620: 24b3 4f5c 1919 3fd4 289a 239e 4a5c 5173  $.O\..?.(.#.J\Qs
+00000630: becf 70f7 4bfa 49b6 f048 dcc4 fc36 25e4  ..p.K.I..H...6%.
+00000640: eff7 c38a bef4 3534 3434 3434 3434 3434  ......5444444444
+00000650: 3434 3434 3434 3434 3434 3434 3434 3434  4444444444444444
+00000660: 3434 3434 3434 3434 3434 fe46 f82f 1054  4444444444.F./.T
+00000670: 65e3 0050 0000                           e..P..
```

