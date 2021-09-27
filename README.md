# pipeline_example
雷雲プロジェクトの観測データからガンマ線イベント(gamma-ray glow)を抽出するコード。

setenv/parameter.yaml
がパラメータを設定するファイルで、これを書き換えた上で、
script/pipeline.py
を動かすと、out の下に結果ができる。

parameter.yaml の中では、datadir　がデータファイルへのパスを示しているので、
最初はここだけ書き換える。

いまは、1 MeV (ADC 100 ch) 以上で 16 sec でビンまとめしたライトカーブを描き、
4 sigma 以上のものをバーストの候補としている。
