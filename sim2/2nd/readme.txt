./sim text_parent text_child data pc ifile > output
のようにして実行
GPRは%r30, %r31だけ16進数表示にしてある


そのままenterで直前と同様の内容で実行
s [num] : 1 (指定されてればnum) ステップ実行
c : 実質終了までずっと実行
j num : 最初から数えてnum回命令が実行されるまで続ける
pj : ジャンプ時にどこからどこへ行くかの表示のON/OFFの切り替え
p : レジスタの状態等を再表示する
m [num]: メモリの内容を表示する。指定されてなければ前回と同じアドレスを参照する。
u : 前回表示したメモリのアドレスより一ブロック分前のメモリの内容を表示する
d : 前回表示したメモリのアドレスより一ブロック分後のメモリの内容を表示する
md : メモリの内容を次回から符号付き整数で表すようにする
mh : メモリの内容を次回から16進数で表すようにする
mf : メモリの内容を次回から小数表示で表すようにする
mc num : 次回からnum番目のコアのメモリの内容を表示するようにする
b : ブレークポイントの表示
b num : ブレークポイントにnumを追加
bc : ブレークポイントの全削除
ps : 現在の統計情報を表示する
pc num : PCの値をnumにする (parallelモードでは使用不可)
