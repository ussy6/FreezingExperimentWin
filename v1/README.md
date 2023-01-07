# Freezing experiment data viewer

## Overview

https://github.com/ussy6/FreezingExperiment

こちらのスクリプトをPythonの環境がないWindowsマシンで動かすための実行環境です．embeddableという軽量なPythonの実行環境を使います．上記リンク先のスクリプトもこちらに入っているので，こちらをダウンロードするだけで使えます．PCの環境を汚す恐れもありません．

## Requirement
- Windows 10（他のOSでは未確認）

以下のライブラリが
- Python 3.8.2
- numpy
- pandas
- matplotlib
- datetime

## Usage

- build.cmdをダブルクリックしてください．「続行するには何かキーを押してください . . .」と出たら完了なので，何かキーを押して閉じてください．この作業は1度行なえばそれ以後は不要ですが，このフォルダ（FreezingExperimentWinあるいは中のv1）を移動した際には行なってください．エラーが出て動かなくなった時もこの作業を試してみてください．

- codeフォルダ内に'input', 'output', 'graph'という名前のフォルダがそれぞれ存在することを確認してください．なければ作成してください．

- ロガーから回収したcsvファイルを全てinputフォルダに入れます．ファイル名は'PoolTEMP_20221222.csv'のようにしてください．

- run.cmdをダブルクリックしてください．ブラウザでjupyter notebook が起動します．

- make_tempfile.ipynbを開きます．上の「Cell」→「Run All」を実行するとoutputフォルダ内にtemp.csvが生成されます．temp.csvはinputフォルダ内のcsvファイルを全て結合し，10分間隔のデータに整形したデータです．このとき，以前に作られたtemp.csvは上書きされる点に注意してください．

- 同様にtemp_viewer.ipynbを開いて実行するとgraphフォルダ内にグラフの画像ファイルが生成されます．PNG形式とSVG形式の2種類が出力されます
 




