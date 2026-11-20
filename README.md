# FrameOS benchmarks

Scores of real FrameOS frames, per board and per FrameOS build: every
release, and the dev builds between them. The charts are at
**<https://frameos.github.io/frameos-benchmarks/>** (`index.html`).

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
| reTerminal E1002 | 2026.11.10 | 968 (935–996) | 868 (864–876) | 702 (668–703) | 1036 (1032–1037) | 1393 (1283–1542) | 967 (923–967) | 100.0 (0 crash, 0 fail) |
| reTerminal E1002 | 2026.11.11 | 933 (908–961) | 865 (862–868) | 660 (642–667) | 1043 (1040–1049) | 1275 (1182–1403) | 941 (941–941) | 100.0 (0 crash, 0 fail) |
| reTerminal E1002 | 2026.11.12 | 966 (927–1017) | 988 (986–993) | 675 (657–682) | 1027 (1024–1034) | 1273 (1111–1527) | 997 (990–1003) | 100.0 (0 crash, 0 fail) |
| reTerminal E1002 | 2026.11.12+3f3bdac79 | 1002 (964–1030) | 975 (971–979) | 709 (660–714) | 1039 (1030–1040) | 1401 (1307–1546) | 996 (958–996) | 100.0 (0 crash, 0 fail) |
| reTerminal E1003 | 2026.11.10 | 1110 (1064–1152) | 986 (983–992) | 2587 (2540–2611) | 930 (929–933) | 639 (553–729) | 1104 (1013–1121) | 100.0 (0 crash, 0 fail) |
| reTerminal E1003 | 2026.11.11 | 1072 (1038–1116) | 979 (976–980) | 2370 (2336–2389) | 935 (934–936) | 609 (545–709) | 1097 (1076–1117) | 100.0 (0 crash, 0 fail) |
| reTerminal E1003 | 2026.11.12 | 1186 (1158–1224) | 1092 (1089–1093) | 2875 (2847–2877) | 927 (920–927) | 679 (631–770) | 1230 (1221–1239) | 90.0 (0 crash, 1 fail) |
| reTerminal E1003 | 2026.11.12+3f3bdac79 | 1166 (1129–1207) | 1079 (1076–1081) | 2571 (2485–2645) | 927 (922–930) | 718 (660–799) | 1210 (1089–1220) | 100.0 (0 crash, 0 fail) |
| reTerminal E1004 | 2026.11.10 | 506 (489–526) | 859 (858–862) | 505 (505–507) | 837 (836–838) | 181 (158–209) | 540 (530–623) | 4.7 (9 crash, 0 fail) |
| reTerminal E1004 | 2026.11.11 | 521 (509–537) | 870 (868–871) | 511 (510–513) | 836 (835–839) | 199 (181–221) | 569 (560–577) | 0.0 (19 crash, 2 fail) |
| reTerminal E1004 | 2026.11.12 | 574 (560–588) | 995 (994–996) | 594 (593–595) | 822 (820–825) | 224 (203–245) | 644 (642–645) | 0.1 (10 crash, 2 fail) |
| reTerminal E1004 | 2026.11.12+3f3bdac79 | 570 (554–587) | 972 (970–976) | 593 (592–596) | 827 (826–828) | 221 (199–246) | 641 (640–665) | 90.0 (0 crash, 1 fail) |
| reTerminal Sticky | 2026.11.10 | 1030 (986–1053) | 991 (988–992) | 1182 (1167–1182) | 1040 (1040–1040) | 924 (787–1009) | 1024 (928–1040) | 100.0 (0 crash, 0 fail) |
| reTerminal Sticky | 2026.11.11 | 986 (965–1006) | 979 (977–981) | 1134 (1104–1146) | 1041 (1034–1041) | 819 (778–875) | 1051 (1003–1097) | — |
| reTerminal Sticky | 2026.11.12 | 1111 (1097–1126) | 1093 (1089–1097) | 1284 (1272–1292) | 1084 (1081–1085) | 1000 (967–1045) | 1082 (1079–1084) | 90.0 (0 crash, 1 fail) |
| reTerminal Sticky | 2026.11.12+3f3bdac79 | 1070 (1055–1085) | 1080 (1077–1085) | 1238 (1216–1239) | 1040 (1040–1043) | 941 (909–987) | 1078 (1015–1078) | 100.0 (0 crash, 0 fail) |

`+<sha>` is a dev build from that commit; `+elf.<sha>` is a build made on
the bench. Builds with only some suites run, so no FrameOS score, are in
`data/` and on the page.

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
