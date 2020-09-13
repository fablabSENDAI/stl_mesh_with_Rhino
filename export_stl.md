---
layout: default
title: STLの書き出し
nav_order: 3
---

# STLデータの書き出し

3Dプリントをするには３DデータをSTL形式で書き出す必要がある。

#### １．閉じたポリサーフェイスであることを確認

開いたサーフェイスはただの”面”なのでプリントできない、

書き出したいオブジェクトを選択し、"What "とコマンドを打つ。

表示されるウィンドウで閉じたポリサーフェイスかどうかを確認。

”**SelClosedPolysrf**”と打てば閉じたポリサーフェイスが全て選択される。

<img src="images/01_what.jpg" alt="hi" class="inline"/>


#### ２．選択→Export

プリントしたいオブジェクトを選択して、

"Export"コマンドを打ち込む。

ファイル形式は"STL"にして、任意の場所に保存。

<img src="images/02_export.png" alt="hi" class="inline"/>


次にToleranceを入力するウィンドウが出てくるが、

大体0.05mm程度にしておけば、3DPの精度以上のデータになるので問題なし。

ここをより小さい値にすると、よりきめ細かいSTLデータが書き出される

（その分データサイズも増える）

<img src="images/03_torelance.png" alt="hi" class="inline"/>


ファイルタイプが聞かれるので、Binaryを選んで書き出し完了。

<img src="images/04_Binary.png" alt="hi" class="inline"/>
