# Comparing `tmp/flytekitplugins-envd-1.8.1.tar.gz` & `tmp/flytekitplugins-envd-1.9.0a0.tar.gz`

```diff
@@ -0,0 +1,199 @@
+00000000: 1f8b 0808 ca83 b964 02ff 666c 7974 656b  .......d..flytek
+00000010: 6974 706c 7567 696e 732d 656e 7664 2d31  itplugins-envd-1
+00000020: 2e39 2e30 6130 2e74 6172 00ed 1d5d 73db  .9.0a0.tar...]s.
+00000030: b831 cffc 1528 f310 694e a23e ac8f 5833  .1...(..iN.>..X3
+00000040: ba39 f7e2 dc79 2e4e 3c71 ae9d 8eeb 6120  .9...y.N<q....a 
+00000050: 1294 5093 040b 82b1 341e fff7 2e40 88a2  ..P.....4....@..
+00000060: 68d9 969c 4469 6bec 8345 82bb 0b60 01ec  h...Dik..E...`..
+00000070: 2eb1 e0da 6939 ad5f cef0 fc77 827d c25f  ....i9._...w.}._
+00000080: 7c17 68e7 70df 6fbb 7dd0 5b5d cbf2 4ebb  |.h.p.o.}.[]..N.
+00000090: dbe9 be40 f317 7b80 2c15 9843 f52f 9e27  ...@..{.,..C./.'
+000000a0: 745f a348 d088 8c3b 83d7 87af 8787 bdc3  t_.H...;........
+000000b0: d74e e770 3018 f45f 5b2f 0cfc df43 102e  .N.p0.._[/...C..
+000000c0: 04b9 a222 09b3 298d d326 89bf f8cd 8e73  ..."..)..&.....s
+000000d0: e8b4 71bb f50d d7ff b0df 97bf 9d61 bfa3  ..q..........a..
+000000e0: ee3b c383 b535 dfe9 f5fa 8303 2886 85df  .;...5......(...
+000000f0: eef4 fb07 fd17 a8bf cff5 cfb3 387e 4801  ............8~H.
+00000100: facc bbfa 5e0a f207 8263 f4bf d1ff 46ff  ....^....c....F.
+00000110: 1bfd bf49 ff9f fdf1 5bf3 e4fd db0f df60  ...I....[......`
+00000120: fd0f 7abd fbf4 7fa7 3fac eaff c140 eaff  ..z.....?....@..
+00000130: f63e d7ff 33d5 ffa7 4460 1f0b dcfc 1be1  .>..3...D`......
+00000140: 2965 f108 759d 8ef5 1e47 6484 36cd 0dab  )e..u....Gd.6...
+00000150: c0d3 93c4 3acf a208 f3c5 087d 9ad1 1425  ....:......}...%
+00000160: d8bb c253 8248 8c27 2149 5196 023e 120c  ...S.H.'!IQ..>..
+00000170: 119c d270 8126 190d 7d84 d11b 254e 4423  ...p.&..}...%ND#
+00000180: 891c 308e 044e af52 0417 d78c 5f05 21bb  ..0..N.R...._.!.
+00000190: 4e1d eb28 1333 c675 4318 9fea 8226 8930  N..(.3.uC....&.0
+000001a0: 0d47 08fb 118d 7f51 0f1d f9f4 1df5 489c  .G.....Q......H.
+000001b0: 42c3 31b4 6246 bad6 af21 4e53 1a50 023c  B.1.bF...!NS.P.<
+000001c0: 4e62 4162 9ff8 e828 f329 893d 8246 2374  NbAb...(.).=.F#t
+000001d0: eea9 cbd6 4792 12cc bdd9 e314 6fc8 1712  ....G.......o...
+000001e0: b204 3ab5 86ab ab96 181f ce4f d051 9270  ..:........O.Q.p
+000001f0: f605 48e1 fe48 3506 9db3 405c 634e 96a8  ..H..H5...@\cN..
+00000200: 6be4 679c 4d39 8ea0 3b53 f40e c7d3 4c4a  k.g.M9..;S....LJ
+00000210: 0568 cf16 d0df 585e 1d38 af77 a638 dc99  .h....X^.8.w.8..
+00000220: a2d3 de9d a4b3 46f2 8925 d42b 442b a0d4  ......F..%.+D+..
+00000230: 6b1d c730 7d08 e1c0 6617 5c25 3cae 8a29  k..0}...f.\%<..)
+00000240: 0ed5 7084 219d ca91 b887 cd52 c47a 9022  ..p.!......R.z."
+00000250: 60ba 3da6 2c7f 4727 1c73 4ad2 2792 9584  `.=.,.G'.sJ.'...
+00000260: 73ca fc0c 1680 f591 fc3b a39c a4cd bc7c  s........;.....|
+00000270: 847e 1ecb b134 fe5f c9ff eb0e eefa 7f07  .~...4._........
+00000280: c6ff db8b ffd7 adf8 7fc3 9ed3 369e 9ff1  ............6...
+00000290: ffa4 fff7 f1f8 e8cd e9b1 13f9 dfd7 ffeb  ................
+000002a0: 81b3 b7f4 ff06 03e9 ff0d dbdd 03e3 ffed  ................
+000002b0: 035e a2b7 7a06 a063 187a 74a6 e681 655d  .^..z..c.zt...e]
+000002c0: c889 7059 9b09 91a4 a356 6b4a c52c 9b38  ..pY.....VkJ.,.8
+000002d0: 1e8b 5ae0 14a5 0c7c 25c6 fd96 44aa 2370  ..Z....|%...D.#p
+000002e0: fb30 8247 118e fd66 08e6 1bfc 3d16 2231  .0.G...f....=."1
+000002f0: c302 cd48 98a4 68c1 32e4 7182 053c 025f  ...H..h.2.q..<._
+00000300: c863 b1c0 80c7 9b13 9c82 97e4 97cc 29b0  .c............).
+00000310: a49c c5ea 5afa 8547 27ad d377 8e65 1daf  ....Z..G'..w.e..
+00000320: ca53 e545 0a74 0d8d 92f8 3e92 de16 f573  .S.E.t....>....s
+00000330: e601 0bc1 7b94 fe43 0015 6660 7a11 cb44  ....{..C..f`z..D
+00000340: 9305 4d78 da9c b0f9 c86a a23f 6276 1d12  ..Mx.....j.?bv..
+00000350: 1fdc 194e c045 4534 966d 042f 94e0 081e  ...N.EE4.m./....
+00000360: ff55 f2ff 0364 1263 41bf 9086 765b b344  .U...d.cA...v[.D
+00000370: 7ab2 8339 0a70 2a08 07c4 f308 8721 f8b1  z..9.p*......!..
+00000380: d073 1412 1c2f 5dda d4b2 fe2e 5bf7 79d3  .s.../].....[.y.
+00000390: fafa dc40 0961 4948 964e b116 0d46 fe1d  ...@.aIH.N...F..
+000003a0: af18 3a54 38c4 aac3 d017 74cd a990 1d2c  ..:T8.....t....,
+000003b0: 0802 1a12 90d1 2706 1d81 f91c 868a 30af  ......'.......0.
+000003c0: b381 606a 5724 a307 6b64 599f 3f7f 8631  ..`jW$..kdY.?..1
+000003d0: 9859 094d 0ada 8d7e 3f20 c220 cc71 04ed  .Y.M...~? . .q..
+000003e0: 9637 8972 67ac 9728 e02c 2a48 a0e9 09e3  .7.rg..(.,*H....
+000003f0: 4279 f3d5 678e ea96 9b26 c45b a29d c892  By..g....&.[....
+00000400: 7328 b05e 02f6 2f92 aab6 c21a 178f 6bfa  s(.^../.......k.
+00000410: b522 1d5f d809 341c a776 03d9 7116 250b  ."._..4..v..q.%.
+00000420: fbb2 01fe be70 4b18 3059 6529 2753 9a0a  .....pK.0Ye)'S..
+00000430: be18 dbcb f707 bb5e 876a 7c12 20d1 a9d5  .......^.j|. ...
+00000440: 51f3 6704 cf47 5024 8113 982c 31b2 61c6  Q.g..GP$...,1.a.
+00000450: 86cc 56fd 7d06 fadf ecff 99fd bfbb fb7f  ..V.}...........
+00000460: ddc1 a03f 305e e073 f7ff 2a0f 5b5f b1fe  ...?0^.s..*.[_..
+00000470: 778a ff74 dbc3 61d7 c47f 8cfe 37fa ffc7  w..t..a.....7...
+00000480: e87f 13ff 31fa 7f83 fe97 0f5b 4f5b ffbb  ....1......[O[..
+00000490: e9ff ceb0 3b30 faff d9e8 7fb3 fffb e3f4  ....;0..........
+000004a0: bfd9 ff35 fa7f 27fd efba 34a6 c275 9d64  ...5..'...4..u.d
+000004b0: f16d f67f db07 c3e1 fafe 6fb7 d7ee 77cd  .m........o...w.
+000004c0: feef 3ec0 b66d cb71 9097 714e 6211 a9a0  ..>..m.q..qNb...
+000004d0: e5e8 4ee8 df51 5b80 561e e157 4545 803f  ..N..Q[.V..WEE.?
+000004e0: 2538 82df 14d1 5890 29c7 82b2 184d 88b8  %8....X.)....M..
+000004f0: 2624 cef7 96d5 e6a8 64e0 58b2 2a9c 0996  &$......d.X.*...
+00000500: ea33 0323 0b21 3412 244a 422c c808 9a91  .3.#.!4.$JB,....
+00000510: 0a16 393c 15f9 03e6 094e a07c 4a60 6c00  ..9<.....N.|J`l.
+00000520: c36f 59f2 81dc a92e f606 e55e 2d98 2e4b  .oY........^-..K
+00000530: f6c4 521b 8e7a a371 923f 58ee 356e 247a  ..R..z.q.?X.5n$z
+00000540: f6eb dfd8 7f63 ff8d fd37 f67f 7bfb bfa6  .....c...7..{...
+00000550: 5cb7 7202 1eb1 fffd 835e d5fe f73b 6d73  \.r......^...;ms
+00000560: fe6f 2fa0 8d63 82c5 2ca4 134b dfa6 b34c  .o/..c..,..K...L
+00000570: d0b0 b8cb 2609 671e 1879 6b59 e485 d4bb  ....&.g..ykY....
+00000580: d2e6 b688 ef79 2c0e e834 d33e 80c6 7c43  .....y,..4.>..|C
+00000590: 029c 85e2 248f 8a56 0938 59e2 c998 3099  ....$..V.8Y...0.
+000005a0: 0b37 c231 6072 ebbe d0e1 8628 a2fb d63d  .7.1`r.....(...=
+000005b0: 39fd cd3d 79d3 c803 8aca b8e7 07c9 1aab  9..=y...........
+000005c0: 1063 e972 69fd 2dcb 93c7 bc36 ba06 b56a  .c.ri.-....6...j
+000005d0: 415d 392b 48ba 19f2 57f9 4239 3955 c71c  A]9+H...W.B99U..
+000005e0: 7d19 1b5e 1e6f 5c0b e466 a98c b9e6 1ed0  }..^.o\..f......
+000005f0: 9285 ba90 9148 45e1 2ac4 5a4a c2a0 8156  .....HE.*.ZJ...V
+00000600: 1d1c ad9a ac6b 97e0 0553 578e 171a ebc0  .....k...SW.....
+00000610: b12b 59bb b9f4 4be1 d3fa 8a22 0ff7 0241  .+Y...K...."...A
+00000620: 60ab 7879 decc 6653 b1b9 d183 ef9c c16f  `.xy..fS.......o
+00000630: 6dc9 bdee 2458 ba84 b748 e281 7b16 301e  m...$X...H..{.0.
+00000640: a19b d240 2c0b 6fed a222 1a94 5aef 2c03  ...@,.o.."..Z.,.
+00000650: b0ab a697 1bf3 936c 0df0 6699 4832 81c4  .......l..f.H2..
+00000660: 2221 6345 dc88 31d8 a39b 3b43 2e8b 6bf5  "!cE..1...;C..k.
+00000670: db46 92a5 b3b1 e019 59d5 aba6 a393 126f  .F......Y......o
+00000680: c66a 81fd 318b 8b08 37ba d157 b7c8 6ea0  .j..1...7..W..n.
+00000690: 603a b627 2150 ae64 9380 5456 13dc 3963  `:.'!P.d..TV..9c
+000006a0: 0989 6b9a c649 9390 8a5a bd81 52e1 433b  ..k..I...Z..R.C;
+000006b0: c765 c493 b363 554e 38af 96af b8cb 18be  .e...cUN8.......
+000006c0: 3a11 011e 3315 30ab 1227 6705 c2c1 7ea8  :...3.0..'g...~.
+000006d0: 66a8 6dd7 d725 0452 4c9c 8485 614d 9dad  f.m..%.RL...aM..
+000006e0: 8899 40ef 594c d691 244c 80c9 5595 5432  ..@.YL..$L..U.T2
+000006f0: 757c e231 1fa4 05b5 719a 009f bf8c a19e  u|.1....q.......
+00000700: bb1c ca82 db48 b826 336b ad85 79c0 5ca2  .....H.&3k..y.\.
+00000710: 4bee ed75 e6ee 5236 20de 449e 1b89 b298  K..u..R6 .D.....
+00000720: 7a30 596b f535 3c8e 694a d0f1 dc23 89d4  z0Yk.5<.iJ...#..
+00000730: 1ab5 3b2d 0cec 00d3 b0bc bae4 5106 ba5c  ..;-........Q..\
+00000740: 1708 0b18 623d 676f f591 10ce 41ec 3779  ....b=go....A.7y
+00000750: fdb7 7663 8d27 f4c2 92eb eec1 a553 5e78  ..vc.'.......S^x
+00000760: c531 0125 719c 927c b142 bfd6 541b 484e  .1.%q..|.B..T.HN
+00000770: dde9 a55c afac 8512 210c a91c 4e44 c294  ...\....!...ND..
+00000780: 6c46 5155 2d0f 3440 4517 9715 6ec5 b3fb  lFQU-.4@E...n...
+00000790: 782d 1114 a7f2 f188 4ddc d69e dfc7 b18c  x-......M.......
+000007a0: a4b8 82e4 80d9 8d7d f68f 4fbf 7f78 7f76  .......}..O..x.v
+000007b0: f4e9 777b 84ec 1667 4cc0 4a2b 74f2 08dd  ..w{...gL.J+t...
+000007c0: b790 adbb 1a03 78ae a611 dc38 59e2 cb39  ......x....8Y..9
+000007d0: b38e a227 6269 e894 66b3 ed97 285d c402  ...'bi..f...(]..
+000007e0: cfc7 5f3a f920 ab09 53ab afc6 2ee7 34b6  .._:. ..S.....4.
+000007f0: 6f56 c286 0922 0f20 8ddf 62e8 713e 39f5  oV...". ..b.q>9.
+00000800: 4118 273f e352 74bb 261b 2e05 78f3 aa81  A.'?.Rt.&...x...
+00000810: 5e39 ff62 34ae 4538 a9c1 ec68 2079 11e2  ^9.b4.E8...h y..
+00000820: 68e2 6334 87f7 e757 f6cd fcd6 06bc 2571  h.c4...W......%q
+00000830: bd5e bfbd 5c67 5f16 e993 7897 1994 f883  .^..\g_...x.....
+00000840: 2b23 5d7a 471f a5aa c1ef f806 fedc d6ad  +#]zG...........
+00000850: c2f4 54e6 53de d12f fa6c 7f31 042f d149  ..T.S../.l.1./.I
+00000860: ec83 11d0 163d 453c 3fcd 0c16 64a1 e45f  .....=E<?...d.._
+00000870: 1eac 6230 a466 7f75 578e 35cd 1ea4 7f6f  ..b0.f.uW.5....o
+00000880: d5b7 76fd 9ff1 abbc 899e 984b 13b7 ee17  ..v........K....
+00000890: 386a 4be1 d7bc f054 97e9 dd0b 57e3 6a15  8jK....T....W.j.
+000008a0: 53b6 9362 eec8 3352 2ef6 9492 9e12 e172  S..b..3R.......r
+000008b0: 50f0 2c72 43e6 e150 e1d5 6c35 5dd4 5e87  P.,rC..P..l5].^.
+000008c0: 3610 0f5a 4627 baf2 2968 7475 938e 3f81  6..ZF'..)htu..?.
+000008d0: 456a 2032 0793 e7b2 2b75 5bdf 24eb 9465  Ej 2....+u[.$..e
+000008e0: dc23 ae5c 272b 41e7 0e17 e849 1007 276b  .#.\'+A....I..'k
+000008f0: 13be 84df 78b8 4130 8f29 4fdd 4a13 be7a  ....x.A0.)O.J..z
+00000900: 2cf3 a164 aa71 b519 4b85 aa74 6c3b 2d58  ,..d.q..K..tl;-X
+00000910: 390a 37bf cf97 7e5d 8f9e d2c4 b931 d5cd  9.7...~].....1..
+00000920: 044b 77fd 935d 4738 45c1 aae7 8123 4fb3  .Kw..]G8E....#O.
+00000930: 915a a952 2d36 7d20 6b49 0e7a bbea dd69  .Z.R-6} kI.z...i
+00000940: 0f03 ccaa 726b a039 1b3d b97a ddbc d0fe  ....rk.9.=.z....
+00000950: 57ef ff98 f8ff 8fdb ff31 f17f b3ff b3e5  W........1......
+00000960: fe8f 7296 1d32 9d36 691c b0d6 4eeb 7fb7  ..r..2.6i...N...
+00000970: f8ff 411f 8a4c fcdf ecff 1bfd bfef fd7f  ..A..L..........
+00000980: d0ff 66ff dfe8 ff2d f4ff d6d9 0176 fefe  ..f....-.....v..
+00000990: bfdb 1b48 fd6f f6ff bf3f 98ef ffcd f7ff  ...H.o...?......
+000009a0: e6fb 7ff3 fdbf f1ff 8cff 67fc 3fe3 ffed  ..........g.?...
+000009b0: e0ff 9d7f f8f3 e3af c7e7 8e98 8baf f2ff  ................
+000009c0: dae0 f755 fcbf fec1 c07c ffbf 1728 523c  ...U.....|...(R<
+000009d0: 5829 1159 e224 0beb b153 bfd6 56c7 82ac  X).Y.$...S..V...
+000009e0: ed5e 1eac ade7 d823 983e 49a4 b716 7b0b  .^.....#.>I...{.
+000009f0: 37a4 f155 ba05 0958 6fbe 7013 4663 b10d  7..U...Xo.p.Fc..
+00000a00: ba8c d0a5 e0cc 9122 e6b6 0591 0eb2 6c83  ......."......l.
+00000a10: 2a58 e286 d2b1 787c 4519 fb6f ecbf b1ff  *X....x|E..o....
+00000a20: 067e a8fd dfa4 719f 64ff e1ae 62ff 87fd  .~....q.d...b...
+00000a30: dec0 d8ff 7d80 59ea cf1b 8cfd 37f6 dfd8  ....}.Y.....7...
+00000a40: 7f63 ff9f 60ff abaf 4f4f 7eff 6ff7 8755  .c..`...OO~.o..U
+00000a50: fbdf 36f1 9ffd c045 f189 851e e44b 4b7d  ..6....E.....KK}
+00000a60: 2130 defc 09a8 5930 c6fe 1bfb 6fec bf01  !0....Y0....o...
+00000a70: 63ff 37ef 873e c5fe 772b fbff 076d 93ff  c.7..>..w+...m..
+00000a80: f7c7 8cbf 59f9 c6fe 1bfb 6fec bf01 63ff  ....Y.....o...c.
+00000a90: 1fb3 ffe5 d0e6 a3eb ff61 fb3f a8bc ff0f  .........a.?....
+00000aa0: da43 b3ff bfd7 f157 6ffd 3f8f dbce 81d3  .C.....Wo.?.....
+00000ab0: ed9a f56f ecbf b1ff c6fe 1b30 f6ff 1b9c  ...o.......0....
+00000ac0: 57da f9fd bf3b e876 4dfe 47f3 fe6f e079  W....;.vM.G..o.y
+00000ad0: d87f f3fd ff8f b3ff e6fb 7f63 ffef b3ff  ...........c....
+00000ae0: f991 702f 987e fdfa 7fd0 fef7 2aef fff0  ..p/.~......*...
+00000af0: b06f deff f702 17e0 ceb9 d29d bbb4 049e  .o..............
+00000b00: e6e7 f7d1 18a9 1b99 7a0b aedb 96d1 04c6  ........z.......
+00000b10: fe9b f7ff 67f2 fedf 35ef ffc6 fe97 edff  ....g...5.......
+00000b20: d6ff e7e1 89f6 bfdb eb77 57f6 bfdd 93f6  .........wW.....
+00000b30: bfdb 37f1 fffd 8cbf 4cb3 acc6 59fe cfde  ..7.....L...Y...
+00000b40: 7499 5259 9558 d6d9 bb3f 7f3b 79ef be3f  t.RY.X...?.;y..?
+00000b50: 3a3d 0647 204f b267 5911 f538 0be9 c4d5  :=.G O.gY..8....
+00000b60: 392b 03bb 3a8b 6e4a 84b7 4091 97bb cb88  9+..:.nJ..@.....
+00000b70: 91cc 7359 d0c8 ffe4 5a0e 3ed8 9796 e52e  ..sY....Z.>.....
+00000b80: f341 baae ac57 cf47 60a4 da95 2789 5559  .A...W.G`...'.UY
+00000b90: 82d7 9a92 277a 5d66 992c f1c8 1f60 953c  ....'z]f.,...`.<
+00000ba0: a2f4 df60 cbc5 aeca 2931 b62b 3925 348e  ...`....)1.+9%4.
+00000bb0: 4f52 8f53 95a1 766c 7ff3 3c17 ba92 bbe7  OR.S..vl..<.....
+00000bc0: 69c6 1755 c9da 978d b5e4 b0e3 8b3b c277  i..U.........;.w
+00000bd0: d685 af09 742a ce62 08c6 9521 c9b1 c23c  ....t*.b...!...<
+00000be0: 3705 8821 cfa0 a15b a673 7416 b4b6 ca61  7..!...[.st....a
+00000bf0: a01f 7a45 a604 684d 91d6 d1de 2adf 4629  ..zE..hM....*.F)
+00000c00: 37af fd48 ba8d 32ea eed9 36ca d45b 25db  7..H..2...6..[%.
+00000c10: d895 e070 5782 4e7b 678a 4e99 e291 e419  ...pW.N{g.N.....
+00000c20: 3ba0 3e90 6763 3397 0d59 30b6 465c 4b97  ;.>.gc3..Y0.F\K.
+00000c30: f134 aabb 4936 341f 3dd5 cbe7 d2c7 3776  .4..I64.=.....7v
+00000c40: f580 b33d 42b0 68d6 16c9 f891 2574 dbb0  ...=B.h.....%t..
+00000c50: 4c0a 5103 060c 1830 60c0 8001 0306 0cfc  L.Q....0`.......
+00000c60: afc3 7f00 4f8d b3b1 00a0 0000            ....O.......
```

