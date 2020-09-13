---
layout: default
title: STLの分析
nav_order: 4
---

# STLデータの分析

スキャンしたり、ダウンロードしたSTLファイルにはそのままプリントできないものもある。

どこに問題があるのかモデルを分析して見つける。

まずは、**[STLファイル](stl/guinomi_broken.stl)**をRhinoで開く。


## Whatコマンド

STLファイルはMeshオブジェクトとして読み込まれる。

通常のRhinoコマンドが使えない場合もある。

ただし、前述した"What"コマンドでオブジェクトの情報を読み取ることができる。

”Closed polygon mesh”の文字があれば3Dプリント可能な**閉じた**メッシュ

<img src="images/05_what.png" alt="hi" class="inline"/>


## DupBorderコマンド

もしも、メッシュが閉じていなけばドコが開いているか見つけ出す必要がある。

"DupBorder"コマンドを打ち込むとメッシュの開いたエッジがコピーされ選択される。

<img src="images/06_dupborder.png" alt="hi" class="inline"/>


## ShowEdgeコマンド

また、"ShowEdges"コマンドでも開いたメッシュのエッジを見つけることができる。

”ShowEdges”コマンドを打ち込み、Naked Edgesを選択することで開いた部分がハイライトされる。

"DupBorder"コマンドのようにエッジがコピーされない。

<img src="images/07_showedges.png" alt="hi" class="inline"/>
