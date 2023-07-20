# Comparing `tmp/flytekitplugins-duckdb-1.8.1.tar.gz` & `tmp/flytekitplugins-duckdb-1.9.0a0.tar.gz`

```diff
@@ -0,0 +1,194 @@
+00000000: 1f8b 0808 c983 b964 02ff 666c 7974 656b  .......d..flytek
+00000010: 6974 706c 7567 696e 732d 6475 636b 6462  itplugins-duckdb
+00000020: 2d31 2e39 2e30 6130 2e74 6172 00ed 1d6b  -1.9.0a0.tar...k
+00000030: 6fdb 46d2 9ff9 2b16 ca01 957a 12ad b762  o.F...+....z...b
+00000040: a1cc d597 38bd a049 ecc6 4e81 8361 a86b  ....8..I..N..a.k
+00000050: 7225 ef99 2259 7219 5b57 e4bf dfec 8314  r%.."Yr.[W......
+00000060: 29d1 b6e4 244a 7b99 8121 89cb 99d9 ddd9  )...$J{..!......
+00000070: 7991 fbb0 bd6f efff 7842 6fff c5a8 c7e2  y....o..xBo.....
+00000080: bd2f 026d 0d77 7db7 dbbd fef2 b72c efb4  ./.m.w}......,..
+00000090: bb9d ee1e b9dd db01 a489 a031 54bf f76d  ...........1T..m
+000000a0: 42f7 2999 0b3e 674e 67f8 f4e0 e9e8 a07f  B.)..>gNg.......
+000000b0: 30b2 47dd f670 7030 b2f6 10fe ef61 ea2f  0.G..pp0.....a./
+000000c0: 04bb e622 f2d3 190f 9296 97ba d7de 65ab  ..."..........e.
+000000d0: 631f d86d dade ff6c f63f 1a0c e477 6734  c..m...l.?...wg4
+000000e0: e8a8 ebce a857 b2f9 4ebf 3f18 f6a0 180c  .....W..N.?.....
+000000f0: bfdd 19b6 7b83 3d32 d8a5 fdc7 6910 dce7  ....{.=2....i...
+00000100: 00bd d0bd fe52 0ef2 2b82 8dfe 1ffd 3ffa  .....R..+.....?.
+00000110: 7ff4 ffd5 feff e4e7 9f5a afde be3c fe64  .........Z...<.d
+00000120: fb1f f6fb 77f9 ffce a0b3 eaff e173 b447  ....w........s.G
+00000130: dabb b4ff 6fd4 ffbf 6182 7a54 d0d6 af2c  ....o...a.zT...,
+00000140: 4e78 188c 49d7 ee58 6fe9 9c8d 49b5 6e58  Nx..I..Xo...I.nX
+00000150: 39a6 5112 eb34 9dcf 69bc 1893 1780 f0e2  9.Q..4..i.......
+00000160: 9fe4 44e1 9369 1893 9786 8575 988a ab30  ..D..i.....u...0
+00000170: 363c c378 660a 5a6c 4eb9 3f26 d49b f3e0  6<.xf.ZlN.?&....
+00000180: 4775 d396 775f 7397 0509 b481 46d4 bd62  Gu..w_s.....F..b
+00000190: 5deb b94f 9384 4f39 031e af02 c102 8f79  ]..O..O9.......y
+000001a0: e430 f538 0b5c 46c6 6372 eaaa 9ffb ef58  .0.8.\F.cr.....X
+000001b0: c268 ec5e 3d4c f182 7d60 7e18 416f 4ab8  .h.^=L..}`~.AoJ.
+000001c0: a66a 8971 7cfa 8a1c 4651 1c7e 0052 b83e  .j.q|...FQ.~.R.>
+000001d0: 548d 21a7 e154 dcd0 9865 a825 f293 389c  T.!..T...e.%..8.
+000001e0: c574 0edd 9991 d734 98a5 74a6 789d 2ca0  .t.....4..t.x.,.
+000001f0: bf81 fcd5 b347 5b53 3cdd 9ae2 606b 8a4e  .....G[S<...`k.N
+00000200: bb44 7216 46dc cd25 2ba0 d4dd 3f0a 6060  .Dr.F..%+...?.``
+00000210: 198b 81cd 36b8 4a76 b12a e6d4 57a3 e1fb  ....6.Jv.*..W...
+00000220: 7c26 07e2 0e36 9984 cd18 cd81 e9e6 98b2  |&...6..........
+00000230: fc35 bf8c 69cc 59f2 48b2 8270 de84 5eea  .5..i.Y.H..p..^.
+00000240: 03a3 77ec f794 c72c 69e9 f231 79e6 c050  ..w....,i..1y..P
+00000250: 367f 00c9 75ff b2b1 f24f 91ff 7587 ebf9  6...u....O..u...
+00000260: 5f0f f3bf 9de4 7fdd 95fc 6fd4 b7db 98f9  _.........o.....
+00000270: 61fe a7f3 bf77 4787 2fde 1cd9 73ef 0be6  a....wG./...s...
+00000280: 7fed ee60 98e7 7fc3 a1ca ff7a dd1e e67f  ...`.......z....
+00000290: bb80 2779 8a56 cede 2ceb 5d1a 101a 50b8  ..'y.V..,.]...P.
+000002a0: cb5d 08da 3761 7ced 87d4 4bc8 0d17 5784  .]..7a|...K...W.
+000002b0: 5148 91d2 4406 774d 675b d659 4840 8504  QH..D.wMg[.YH@..
+000002c0: f57d 2220 4dd2 2ad5 2420 5975 3d0d 7d3f  .}" M.*.$ Yu=.}?
+000002d0: bc91 146e 0809 63e0 8d2d ebb7 df7e bba4  ...n..c..-...~..
+000002e0: c995 15f1 28a7 bd23 ed04 54f4 4bf8 fe07  ....(..#..T.K...
+000002f0: e3ff 977f ff03 5e78 7030 406b c3f8 bf72  ......^xp0@k...r
+00000300: 7bff d1f6 bfd5 fb7f b0fe 5117 dfff a3ff  {.........Q.....
+00000310: 47ff ff55 fc3f beff 47ff 5fed fff5 edfd  G..U.?..G._.....
+00000320: eded 7f3b ffdf 1d74 87e8 ffbf 19ff 8fef  ...;...t........
+00000330: ffbe 9eff c7f7 7fe8 ffb7 f6ff 9309 0fb8  ................
+00000340: 984c ec68 b1a1 fddf fbfe 0fee 95de ff75  .L.h...........u
+00000350: fbc3 3ebe ffdb 09d4 6a35 cbb6 899b c631  ..>.....j5.....1
+00000360: 0bc4 5c4d 758d d7a6 7e6d f30e 4ea2 d254  ..\Mu...~m..N..T
+00000370: 8489 99f1 1d5b 8490 b160 f3c8 a782 8d81  .....[...`......
+00000380: 4d22 c2b9 1d27 42df 085d 1133 289f 3190  M"...'B..].3(.1.
+00000390: 2d60 78fb 96bc a1df 18fe 92b2 7861 c906  -`x.........xa..
+000003a0: 58d3 389c 135b d0e4 9af0 7914 c6a2 8482  X.8..[....y.....
+000003b0: 568a f11f e33f c67f 843f 4bfc 979e 7ab3  V....?...?K...z.
+000003c0: d8ff 70fc ef74 dabd ce6a fc6f f7bb 18ff  ..p..t...j.o....
+000003d0: 7701 26dc fe27 0903 1d85 c522 9253 7459  w.&..'.....".StY
+000003e0: 18e6 ae68 92d7 3c81 4fb9 28cc 3b4b 239f  ...h..<.O.(.;K#.
+000003f0: 35c9 7124 7818 50bf 49de 07f0 c3b2 0cbe  5.q$x.P.I.......
+00000400: c913 cc55 4403 8f26 04fe 222f 2f5b d038  ...UD..&.."//[.8
+00000410: 0e6f 5421 3591 3fd3 b2ac 56bd c0e6 959c  .oT!5.?...V.....
+00000420: 0f0c 5c76 06ca 56c6 b3d9 ad5c cf95 a1cb  ..\v..V....\....
+00000430: f544 f194 ba6c 050b bac2 123b 1171 ea8a  .D...l.....;.q..
+00000440: 3466 5ee1 e744 ae79 4b58 5ee3 697e e785  4f^..D.yKX^.i~..
+00000450: be61 5996 2b17 0e11 9582 1ca7 224a 457d  .aY.+......."JE}
+00000460: 2981 86ca 7c88 1ba6 b2ee 31e1 8120 0e69  )...|.....1.. .i
+00000470: 7554 69a8 b0c7 b990 cea1 de0b b8fd 360c  uTi...........6.
+00000480: 58ce b790 e0d4 d7fb 6bf8 4fce 0e4f 7f9e  X.......k.O..O..
+00000490: 9cfd fbe4 08c8 6b5a b835 9542 118f 4d49  ......kZ.5.B..MI
+000004a0: 9686 d755 8984 84f9 d366 7e15 a865 7c50  ...U.....f~..e|P
+000004b0: fbb2 e877 59e1 588f 9a6c 971e 5cd5 c28b  ...wY.X..l..\...
+000004c0: 2516 0fa0 0349 a107 520f 34ba a65c 9357  %....I..R.4..\.W
+000004d0: 93f8 c0e7 e222 ebe7 92d7 f7df 5fdf d078  ....."......_..x
+000004e0: 96e8 12d3 3109 32f3 cb7e 9f5d f184 cc19  ....1.2..~.]....
+000004f0: 8801 4615 fac4 a9cf ffcb 1235 6f5c 9094  ..F........5o\..
+00000500: 6de5 1487 c072 c96b d95b 3946 249c 2a4a  m....r.k.[9F$.*J
+00000510: e9a6 4a28 a6f7 66a6 5b5d 1111 1276 cbdc  ..J(..f.[]...v..
+00000520: 54b0 126a 2682 33e0 a311 231a 036f 18ee  T..j&.3...#..o..
+00000530: 44d2 5cca e96f e691 9b2b ee33 c341 1a8e  D.\..o...+.3.A..
+00000540: c8f0 2bfb 29c7 c79e 687e ce0a de13 e2c6  ..+.)...h~......
+00000550: 0c92 6442 03a8 bd35 67f3 10b0 a4a2 5eca  ..dB...5g.....^.
+00000560: c976 7145 c577 0909 c2a0 25d7 2c82 b4e5  .vqE.w....%.,...
+00000570: a2b8 3263 370c 80ad d613 1b2e 02e6 8a7a  ..2c7..........z
+00000580: 6dac 598d 6b8d a5f8 b48e 2680 fd47 2d66  m.Y.k.....&..G-f
+00000590: 49ea 8bda 78dd 0a3e 2e09 9214 6aad 17c6  I...x..>....j...
+000005a0: a2a9 ea6c d8eb 4a98 0d86 233f 9aa5 6239  ...l..J...#?..b9
+000005b0: 2213 6997 8e6e 70ae df15 68d0 fe29 9f39  ".i..np...h..).9
+000005c0: 656d d243 63ec ddc9 2dbf ae87 cbd1 5fcd  em.Cc...-....._.
+000005d0: ac7b 8ef9 6e94 1994 5552 a965 c1a8 8c36  .{..n...UR.e...6
+000005e0: e851 aa2b 8bd2 630f dae0 2b4f 68d4 48d9  .Q.+..c...+Oh.H.
+000005f0: 43d1 0534 c91c 04c9 c13f 4c32 82cb 30f4  C..4.....?L2..0.
+00000600: 37d0 7988 3edb 297b c6ff 970a d504 bddc  7.y.>.){........
+00000610: 402d b7b4 87bc 9fef 81bb b990 b873 1ac9  @-...........s..
+00000620: 0ae3 d68c 7f60 0101 b1a6 7231 a56a 88a8  .....`....r1.j..
+00000630: b09d 12d3 3571 9d82 4b9e fa74 26a9 79e0  ....5q..K..t&.y.
+00000640: 7157 da83 5a4c 024a aa16 ee82 696b 64b5  qW..ZL.J....ikd.
+00000650: be38 63a0 aa91 ab3d ab04 cda7 6052 8bfa  .8c....=....`R..
+00000660: 2d70 34cd 91a4 eab2 5efb 5bad 496a ffa8  -p4.....^.[.Ij..
+00000670: 351a 65f9 02cd 6ae3 4af7 0b22 217f 7748  5.e...j.J.."!.wH
+00000680: 67ed 2630 0842 91e3 fc40 7c16 d435 a7c6  g.&0.B...@|..5..
+00000690: 3a2b 0931 e520 da5f a99f b223 0891 71bd  :+.1. ._...#..q.
+000006a0: 7692 498d 7821 4b82 ef04 8c0c 28a0 0d86  v.I.x!K.....(...
+000006b0: 5c51 5d0d 1234 168b 5ade 4ddb 0f6f c066  \Q]..4..Z.M..o.f
+000006c0: efa8 ee89 5a98 6386 7a0e 0222 1e4f 6236  ....Z.c.z..".Ob6
+000006d0: a3b1 9729 4c90 ce2f a172 1039 8ca8 5a15  ...)L../.r.9..Z.
+000006e0: 0bc3 024f f831 5312 547e 4a56 59a1 5919  ...O.1S.T~JVY.Y.
+000006f0: 2c38 f3bd 5210 d526 e9e4 0ecb 2e34 a1fe  ,8..R..&.....4..
+00000700: bbf6 2c5a 4ee7 4678 178d dccc 1cf3 bd2e  ..,ZN.Fx........
+00000710: 00e6 276c fc89 4d78 64f5 d555 f34c 513f  ..'l..Mxd..U.LQ?
+00000720: 6fab 3e4d 16f7 e998 54d7 2462 ae5c 2bed  o.>M....T.$b.\+.
+00000730: 1575 6c9d ddb6 8daf 6a74 ee70 334c ed69  .ul.....jt.p3L.i
+00000740: 33df dc20 ad67 eb01 695c 8896 67c7 2f8e  3.. .g..i\..g./.
+00000750: c7e4 28a0 9760 ff5c c817 4ce0 82c0 546e  ..(..`.\..L...Tn
+00000760: 02b9 508d d0a9 ec15 f572 759e a681 abf3  ..P......ru.....
+00000770: 192e 165a 9533 f624 cb07 ddd0 63b6 55f6  ...Z.3.$....c.U.
+00000780: b259 ea96 954a ddbf 660b 6967 aabf 914a  .Y...J..f.ig...J
+00000790: df26 7958 b275 14b2 0127 59b5 be0f d407  .&yX.u...'Y.....
+000007a0: 76ba 8bf6 8c89 3a20 3556 3d0f 4fb8 c905  v.....: 5V=.O...
+000007b0: eb1f 648e bd26 860a 9306 7366 3399 14c4  ..d..&....sf3...
+000007c0: 15dd 5ac3 5e8e 5346 251b d294 cdb3 c348  ..Z.^.SF%......H
+000007d0: 792a fb4c 0ab6 6153 dfaf 3756 15be a291  y*.L..aS..7V....
+000007e0: f5c8 b365 f35e 4a7d 92da 6a18 dcdf 56f3  ...e.^J}..j...V.
+000007f0: 8820 db39 9584 fbfa e940 48d2 6d5a bd41  . .9.....@H.mZ.A
+00000800: 0365 ecae 6c8c 1b46 0b35 3030 82a1 19f3  .e..l..F.500....
+00000810: 35b4 5c15 00f1 e1ba 6008 2aab 528a a9aa  5.\.....`.*.R...
+00000820: a1aa 3d77 5723 9fc8 6cb5 e0b2 5ed1 bd2a  ..=wW#..l...^..*
+00000830: fb5e b3ed 69ed e816 ec59 30cf 64b3 2a2f  .^..i....Y0.d.*/
+00000840: 86e4 8b54 a4ef d062 027a ad13 9c98 b98c  ...T...b.z......
+00000850: cb4d 2f7f 4874 d580 8fc5 ec71 cac1 88f2  .M/.Ht.....q....
+00000860: 34b6 90d4 969f 3326 da2b 004a d155 340a  4.....3&.+.J.U4.
+00000870: 369c 7cae 78bf 12ac a1ca c290 187f debe  6.|.x...........
+00000880: 304a b0f4 cd4a 94e4 2585 4fcb aab6 c042  0J...J..%.O....B
+00000890: ef32 72d0 5915 ce0b b71a e419 e994 c744  .2r.Y..........D
+000008a0: 8e76 08c9 5120 b859 10cb 02d9 cab9 ece3  .v..Q .Y........
+000008b0: 7ac4 94dd d312 cdfc 8ae6 7c3e 6e75 2ed6  z.........|>nu..
+000008c0: 477b 45c0 013c 12d7 2b5d be66 554e 6a2b  G{E..<..+].fUNj+
+000008d0: 1197 eae7 e82f 93e8 3aa6 ef99 072f d66c  ...../..:..../.l
+000008e0: 9bc2 b5cc d759 b9ae ac71 3d72 954b ee54  .....Y...q=r.K.T
+000008f0: b373 1089 5550 a329 13ee 9591 9e11 897e  .s..UP.).......~
+00000900: 9901 5287 a76d b1f6 a4c5 9461 c8c0 40c9  ..R..m.....a..@.
+00000910: e9d1 eba3 e767 2b28 b943 aa94 ed46 32ad  .....g+(.C...F2.
+00000920: 9465 a14b 9f53 a24b b935 6cc3 4739 d27a  .e.K.S.K.5l.G9.z
+00000930: c168 6306 161f acdb 7e3d efab 93ff 6ae0  .hc.....~=....j.
+00000940: 2b60 9cff d9d9 fc0f aeff fb7a f33f b8fe  +`.........z.?..
+00000950: 0fe7 7f36 9eff 9998 578b 6c36 6bf1 601a  ...6....W.l6k.`.
+00000960: ee6f 6cff dbad ffeb f7a0 08d7 ffe1 fc3f  .ol............?
+00000970: faff 5dcf ff83 ffc7 f97f f4ff 1bfa ff8d  ..].............
+00000980: ce87 d9ee fc17 b8df 1df4 461d 9cff df05  ..........F.....
+00000990: e0f9 2f78 fe0b 9eff 82e7 bf60 fe87 f91f  ../x.......`....
+000009a0: e67f 98ff 6d99 ff9d 1ebf 7ff7 fce8 d416  ....m...........
+000009b0: b7e2 d1f9 5f7b 305c cdff 869d 611f f3bf  ...._{0\....a...
+000009c0: 5d40 7ec0 8f95 3091 4676 b4b0 1ede f363  ]@~...0.Fv.....c
+000009d0: ddbf 2cd8 daf4 a9c1 da42 bd1e c4f5 5824  ..,......B....X$
+000009e0: 73bc c05d 4c7c 1e5c 271b 11c9 156a 0964  s..]L|.\'....j.d
+000009f0: 7572 52c5 bd86 a468 33b2 d8a4 021b 218b  urR....h3.....!.
+00000a00: 309a f832 cdb8 df4a 30fe 63fc c7f8 8ff0  0..2...J0.c.....
+00000a10: 978a ff55 4e77 ebf8 0f57 e5f8 df6b f7fa  ...UNw...W...k..
+00000a20: 038c ffbb 0034 f56f 1b30 fe63 fcc7 f88f  .....4.o.0.c....
+00000a30: f1ff 91f1 bffa f969 dbf8 df6d afc6 ff61  .......i...m...a
+00000a40: 17f7 7f7e 8df1 47cb c7f8 8ff1 1fe3 3f02  ...~..G.......?.
+00000a50: c6ff 4de2 7ff1 45e8 bdf6 7f6f fcef afbd  ..M...E....o....
+00000a60: ff1f e2fa 8fdd 8eff 0f5d bb6d b79b cf9c  .........].m....
+00000a70: 8edd b3db 975d cb2c f640 0bc1 f88f f11f  .....].,.@......
+00000a80: e33f 02c6 ffc7 ce6d 6efd fcdf 1d81 03c0  .?.....mn.......
+00000a90: f88f cfff 08df 44fc c7fd 7f5f 2ffe e3fe  ......D...._/...
+00000aa0: 3f8c ff77 c77f bd28 cc9d ce3e d5fe ef7f  ?..w...(...>....
+00000ab0: fe1f aefe ffdf e160 88f1 7f17 700e a9dc  .......`....p...
+00000ac0: 44a6 7217 96a0 b3c9 65ca 7d8f 3844 5d78  D.r.....e.}.8D]x
+00000ad0: f2a0 0a87 b42d f404 18ff f1f9 ff1b 79fe  .....-........y.
+00000ae0: efe2 f33f c6ff 72fc dff8 a4e7 47c5 ff6e  ...?..r.....G..n
+00000af0: 77d0 5bc6 ff76 5fc6 ffc1 00e7 ff77 33fe  w.[..v_......w3.
+00000b00: f298 2435 ca22 0cfd 243b 0f59 9558 d6c9  ..$5."..$;.Y.X..
+00000b10: ebf7 3fbd 7a3b 797b f8a6 7c00 f19c bb71  ..?.z;y{..|....q
+00000b20: e8f3 cb49 a04f 489a d656 f5e8 8f02 e947  ...I.OH..V.....G
+00000b30: a0d0 e593 6cbe 0868 ce73 9a7c d2a1 a967  ....l..h.s.|...g
+00000b40: 21e4 899c a6aa 0bcb 9a4c 3ee8 0da7 9389  !........L>.....
+00000b50: 6c83 d14c 60a9 daa8 8f5d 52a7 cd96 1aa5  l..L`....]R.....
+00000b60: 8f76 3594 4e81 87be 41d5 ee53 a796 6d47  .v5.N...A..S..mG
+00000b70: ad15 8b27 6a53 aa53 5bd9 946a 703c 96b8  ...'jS.S[..jp<..
+00000b80: 3157 0723 3bb5 bb77 bc1a ecf5 0532 cef9  1W.#;..w.....2..
+00000b90: aab0 6ae6 e4e5 25c6 9a3c edb2 3c0d 81f9  ..j...%..<..<...
+00000ba0: 8fb9 b954 9d15 296b 2c5f ef52 85fe e8bd  ...T..)k,_.R....
+00000bb0: b4a6 65e6 d4c2 9cb6 56d8 ce68 50dc 7ceb  ..e.....V..hP.|.
+00000bc0: 24b4 6979 b4ea 46fb 6f6b cd07 0896 db6f  $.iy..F.ok.....o
+00000bd0: 8ba8 dbef be2d 526f b4f9 765b 82a7 db12  .....-Ro..v[....
+00000be0: 1c6c 4bd0 6917 291e d84c bb05 ea3d fb6e  .lK.i.)..L...=.n
+00000bf0: abb9 54ec 8add 18b1 b47d f671 54eb 9b6e  ..T......}.qT..n
+00000c00: 0d1f d077 3c91 0c01 0101 0101 0101 0101  ...w<...........
+00000c10: 0101 0101 e1d1 f03f e0ef 02cc 00a0 0000  .......?........
```
