# FrameOS benchmarks

Scores of real FrameOS frames, per board and per FrameOS build: every
release, and the dev builds between them. The charts are at
**<https://bench.frameos.net/>** (`index.html`).

The bench that makes these numbers lives in the FrameOS repo,
[`tools/frame-bench`](https://github.com/FrameOS/frameos/tree/main/tools/frame-bench).
It puts the same benchmark scenes on every board over USB and times them by
the lines every firmware prints, so a release from before the bench existed is
measured exactly like main. What is measured, the formula, the noise and what
is not measured yet:
[`SCORES.md`](https://github.com/FrameOS/frameos/blob/main/tools/frame-bench/SCORES.md).

## Scores

1000 is the median board on 2026.11.12. A category is the geometric mean of
its metrics, each scored 1000 × reference ÷ value (higher is better). The
FrameOS score is the geometric mean of CPU, Graphics, Image and
Responsiveness; Memory and Stability are shown beside it. Every value is the
median, with the quartiles in brackets.

| board | build | FrameOS score | CPU | Graphics | Image | Responsiveness | Memory | Stability (full) |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| SenseCAP Indicator D1 | 2026.11.10 | 945 (919–969) | 804 (800–806) | 584 (573–590) | 1007 (1000–1009) | 1685 (1553–1840) | 809 (731–814) | 100.0 (0 crash, 0 fail) |
| SenseCAP Indicator D1 | 2026.11.11 | 934 (913–958) | 798 (795–798) | 565 (556–574) | 1014 (1014–1017) | 1667 (1552–1809) | 795 (787–802) | 100.0 (0 crash, 0 fail) |
| SenseCAP Indicator D1 | 2026.11.12 | 1059 (1035–1085) | 891 (887–897) | 799 (777–814) | 1000 (995–1001) | 1765 (1671–1894) | 739 (738–740) | 81.0 (0 crash, 2 fail) |
| SenseCAP Indicator D1 | 2026.11.12+3f3bdac79 | 1022 (995–1051) | 875 (872–879) | 810 (797–816) | 998 (992–1004) | 1540 (1420–1694) | 743 (738–743) | 22.5 (2 crash, 1 fail) |
| SenseCAP Indicator D1 | 2026.11.13 | 1186 (1159–1218) | 864 (859–868) | 781 (777–799) | 1002 (993–1003) | 2930 (2724–3160) | 806 (806–806) | 100.0 (0 crash, 0 fail) |
| SenseCAP Indicator D1 | 2026.11.13-main-ff6a5b9d5+elf.3004a294 | 1183 (1166–1201) | 1090 (1083–1091) | 1050 (1034–1053) | 1010 (1008–1015) | 1697 (1636–1787) | 819 (819–819) | 100.0 (0 crash, 0 fail) |
| SenseCAP Indicator D1 | 2026.11.14 | 1204 (1183–1223) | 1074 (1068–1080) | 1117 (1094–1124) | 1012 (1007–1017) | 1733 (1666–1815) | 776 (776–776) | 100.0 (0 crash, 0 fail) |
| reTerminal E1002 | 2026.11.10 | 968 (935–996) | 868 (864–876) | 702 (668–703) | 1036 (1032–1037) | 1393 (1283–1542) | 967 (923–967) | 100.0 (0 crash, 0 fail) |
| reTerminal E1002 | 2026.11.11 | 933 (908–961) | 865 (862–868) | 660 (642–667) | 1043 (1040–1049) | 1275 (1182–1403) | 941 (941–941) | 100.0 (0 crash, 0 fail) |
| reTerminal E1002 | 2026.11.12 | 966 (927–1017) | 988 (986–993) | 675 (657–682) | 1027 (1024–1034) | 1273 (1111–1527) | 997 (990–1003) | 100.0 (0 crash, 0 fail) |
| reTerminal E1002 | 2026.11.12+3f3bdac79 | 1002 (964–1030) | 975 (971–979) | 709 (660–714) | 1039 (1030–1040) | 1401 (1307–1546) | 996 (958–996) | 100.0 (0 crash, 0 fail) |
| reTerminal E1002 | 2026.11.13 | 996 (977–1021) | 962 (954–969) | 718 (713–720) | 1032 (1028–1034) | 1381 (1303–1506) | 977 (977–977) | 65.6 (0 crash, 4 fail) |
| reTerminal E1002 | 2026.11.13-main-ff6a5b9d5+elf.3004a294 | 1080 (1064–1097) | 1256 (1247–1262) | 1026 (1019–1031) | 1040 (1038–1045) | 1016 (971–1067) | 848 (848–848) | 100.0 (0 crash, 0 fail) |
| reTerminal E1002 | 2026.11.14 | 1237 (1224–1246) | 1232 (1227–1234) | 1211 (1203–1213) | 1268 (1265–1268) | 1238 (1204–1269) | 850 (850–850) | 100.0 (0 crash, 0 fail) |
| reTerminal E1003 | 2026.11.10 | 1110 (1064–1152) | 986 (983–992) | 2587 (2540–2611) | 930 (929–933) | 639 (553–729) | 1104 (1013–1121) | 100.0 (0 crash, 0 fail) |
| reTerminal E1003 | 2026.11.11 | 1072 (1038–1116) | 979 (976–980) | 2370 (2336–2389) | 935 (934–936) | 609 (545–709) | 1097 (1076–1117) | 100.0 (0 crash, 0 fail) |
| reTerminal E1003 | 2026.11.12 | 1186 (1158–1224) | 1092 (1089–1093) | 2875 (2847–2877) | 927 (920–927) | 679 (631–770) | 1230 (1221–1239) | 90.0 (0 crash, 1 fail) |
| reTerminal E1003 | 2026.11.12+3f3bdac79 | 1166 (1129–1207) | 1079 (1076–1081) | 2571 (2485–2645) | 927 (922–930) | 718 (660–799) | 1210 (1089–1220) | 100.0 (0 crash, 0 fail) |
| reTerminal E1003 | 2026.11.13 | 1174 (1137–1215) | 1066 (1060–1066) | 2584 (2482–2678) | 930 (927–930) | 741 (686–821) | 1249 (1249–1249) | 100.0 (0 crash, 0 fail) |
| reTerminal E1003 | 2026.11.13-main-ff6a5b9d5+elf.6a4d0425 | 1600 (1524–1665) | 1267 (1262–1269) | 6495 (5806–6785) | 923 (923–924) | 863 (798–967) | 1197 (1197–1197) | 100.0 (0 crash, 0 fail) |
| reTerminal E1003 | 2026.11.14 | 1661 (1607–1865) | 1256 (1252–1261) | 7135 (6802–10090) | 935 (934–936) | 908 (839–1015) | 1186 (1186–1186) | 100.0 (0 crash, 0 fail) |
| reTerminal E1004 | 2026.11.10 | 506 (489–526) | 859 (858–862) | 505 (505–507) | 837 (836–838) | 181 (158–209) | 540 (530–623) | 4.7 (9 crash, 0 fail) |
| reTerminal E1004 | 2026.11.11 | 521 (509–537) | 870 (868–871) | 511 (510–513) | 836 (835–839) | 199 (181–221) | 569 (560–577) | 0.0 (19 crash, 2 fail) |
| reTerminal E1004 | 2026.11.12 | 574 (560–588) | 995 (994–996) | 594 (593–595) | 822 (820–825) | 224 (203–245) | 644 (642–645) | 0.1 (10 crash, 2 fail) |
| reTerminal E1004 | 2026.11.12+3f3bdac79 | 570 (554–587) | 972 (970–976) | 593 (592–596) | 827 (826–828) | 221 (199–246) | 641 (640–665) | 90.0 (0 crash, 1 fail) |
| reTerminal E1004 | 2026.11.13 | 575 (560–590) | 960 (955–963) | 606 (605–606) | 829 (828–830) | 226 (205–251) | 692 (692–692) | 100.0 (0 crash, 0 fail) |
| reTerminal E1004 | 2026.11.13-main-ff6a5b9d5+elf.6a4d0425 | 645 (625–663) | 1249 (1240–1251) | 721 (718–721) | 833 (832–833) | 231 (206–257) | 629 (629–629) | 100.0 (0 crash, 0 fail) |
| reTerminal E1004 | 2026.11.14 | 703 (679–726) | 1222 (1216–1227) | 758 (757–759) | 1086 (1085–1087) | 243 (213–275) | 611 (611–611) | 100.0 (0 crash, 0 fail) |
| reTerminal Sticky | 2026.11.10 | 1030 (986–1053) | 991 (988–992) | 1182 (1167–1182) | 1040 (1040–1040) | 924 (787–1009) | 1024 (928–1040) | 100.0 (0 crash, 0 fail) |
| reTerminal Sticky | 2026.11.11 | 986 (965–1006) | 979 (977–981) | 1134 (1104–1146) | 1041 (1034–1041) | 819 (778–875) | 1051 (1003–1097) | — |
| reTerminal Sticky | 2026.11.12 | 1111 (1097–1126) | 1093 (1089–1097) | 1284 (1272–1292) | 1084 (1081–1085) | 1000 (967–1045) | 1082 (1079–1084) | 90.0 (0 crash, 1 fail) |
| reTerminal Sticky | 2026.11.12+3f3bdac79 | 1070 (1055–1085) | 1080 (1077–1085) | 1238 (1216–1239) | 1040 (1040–1043) | 941 (909–987) | 1078 (1015–1078) | 100.0 (0 crash, 0 fail) |
| reTerminal Sticky | 2026.11.13 | 1073 (1057–1097) | 1064 (1058–1065) | 1247 (1212–1310) | 1040 (1040–1041) | 961 (936–998) | 1132 (1132–1132) | 100.0 (0 crash, 0 fail) |
| reTerminal Sticky | 2026.11.13-main-ff6a5b9d5+elf.6a4d0425 | 1215 (1200–1233) | 1273 (1264–1275) | 1608 (1561–1641) | 1052 (1049–1052) | 1013 (1002–1051) | 1058 (1058–1058) | 100.0 (0 crash, 0 fail) |
| reTerminal Sticky | 2026.11.14 | 1245 (1224–1284) | 1257 (1254–1264) | 1625 (1576–1733) | 1051 (1049–1052) | 1120 (1082–1180) | 1032 (1032–1032) | 100.0 (0 crash, 0 fail) |

`+<sha>` is a dev build from that commit; `+elf.<sha>` is a build made on
the bench. Builds with only some suites run, so no FrameOS score, are in
`data/` and on the page.

## Findings

What a run showed, per release, beyond the numbers:

- [2026.11.14](findings/2026.11.14.md): the release; no crash and no fail on any board in a full run; FrameOS score +16 to +41 % over 2026.11.13 on the e-paper boards, S3 image 23.5 KB smaller; the internal RAM floor fell further after the candidate (E1002 down to 8 KB).
- [2026.11.14 candidate, main ff6a5b9d5](findings/2026.11.14-rc.md): no crash and no fail on any board in a full run; CPU +19–30 % (JSON 2–2.7× faster); E1003 graphics 2.5×; fixes for the E1004's pack and fit, text borders, gradients, the E1002's canvas and the Sticky's tap latency.
- [2026.11.13](findings/2026.11.13.md): the first release with no crash on any board, the E1004 included; the E1003's UI renders lost their damage repaint; a scene installed right after another push can be dropped on the board.

## The data

- `data/boards.jsonl`, `runs.jsonl`, `metrics.jsonl`, `images.jsonl`:
  JSON Lines, one table per file, append-only. The columns are in
  [`SCHEMA.md`](SCHEMA.md).
- `index.html`: the page, made from `data/` by `bench.py html`.

## Adding a run

Clone this repo beside your frameos checkout (`../frameos-benchmarks`, or set
`$FRAMEOS_BENCHMARKS`). A finished `tools/frame-bench/bench.py run` adds
its rows to `data/`. Then run `bench.py html`, and commit and push here,
saying in the message which build was run and why.

## The page

<https://bench.frameos.net/> is this repo served as it stands by a Cloudflare
Worker with static assets (`wrangler.jsonc`; `.assetsignore` keeps `.git` and
the config out). Cloudflare's Workers Builds deploys every push to `main`
(deploy command `npx wrangler deploy`, no build step), so pushing a run is
publishing it. By hand: `npx wrangler deploy` from a checkout logged in to the
FrameOS Cloudflare account.
