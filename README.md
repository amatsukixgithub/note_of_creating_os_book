# note_of_creating_os_book
【作って理解するOS x86系コンピュータを動かす理論と実装】のメモ

https://gihyo.jp/book/2019/978-4-297-10847-2

# 0章 コンピュータが数を数える仕組みとC言語への応用
## 数の表現方法
基数：何進数であるか表す数値

|基数|C言語での表記|
|-|-|
|2|不可|
|8|0123|
|10|123|
|16|0x123|

キャリー：加算の際に最上位ビットで発生した桁上がりのこと。
オーバーフロー：キャリーが発生している場合のこと。

## 演算を行うための負数の表現方法
初期のコンピュータでは「1の補数」を用いて負数を表現していたが、キャリービットを有効な値として使用するためオーバーフローが発生しているか分からなかった。現在はオーバーフローの発生が分かるように「2の補数」が採用されている。

1の補数：最上位ビットを負数かどうかのフラグとし、ビットをすべて反転して得られる。（001の場合は110）
2の補数：1の補数に+1した値（001の場合は111）

|2進数|1の補数|2の補数|
|-|-|-|
|000|0|0|
|001|1|1|
|010|2|2|
|011|3|3|
|100|-3|-4|
|101|-2|-3|
|110|-1|-2|
|111|-0|-1|

## コンパイル
システム記述言語（C,Java,...）をコンパイラによってCPU命令に翻訳すること。
CPU命令はアセンブラによりCPU固有の機械語に変換される。
システム記述言語 -> コンパイラ -> CPU命令(x86) -> アセンブラ -> 機械語(x86)

# 1章
# 2章
# 3章
# 4章
# 5章
# 6章
# 7章
# 8章
# 9章

