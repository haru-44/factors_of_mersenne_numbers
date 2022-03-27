# Factors of Mersenne numbers

## 概要

Mersenne数について、既知の素因数をリスト化している。
[mersenne.ca](https://www.mersenne.ca/)を基に作成しているため、最新の情報はそちらを参照すること。

## 仕様

Mersenne数は、M_q = 2^q - 1 という形の自然数である。
qが素数の場合のみ記載する。

* headerなしのcsv(Comma-Separated Values)
* 1列目はq
* 2列目はM_qの状態
  * `U` : M_qは素数か合成数か不明
  * `P` : M_qは素数
  * `L` : M_qは一度Lucas–Lehmerテストを実施し、合成数だと思われる
  * `C` : M_qの素因数が見つかっているが、Lucas–Lehmerテストのダブルチェックが完了している
  * `F` : M_qは完全に素因数分解されている
* 3列目以降は具体的な素因数
  * Mersenne数の素因数は2qk+1の形をしているため、kのみを記載

### 例

* `3,P` : M_3は素数
* `11,F,1` : M_11 = (2 * 11 * 1 + 1) * R と分解でき、Rは素数
* `5000081,C,2563,3507120` : M_5000081 = (2 * 5000081 * 2563 + 1) * (2 * 5000081 * 3507120 + 1) * R と分解でき、Rは合成数

## License

[MIT license](https://en.wikipedia.org/wiki/MIT_License).
