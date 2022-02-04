# 2021gsc_KuniharuHigano

# 2021年度 日向野邦春ゼミ論用レポジトリ
2021年度　卒業論文/ゼミ論文 ２０２１年１月２５日

青山学院大学 地球社会共生学部 地球社会共生学科

日向野邦春/KUNIHARU HIGANO

学生番号　1A118128

指導教員　古橋 大地 教授

© Furuhashi Laboratory/Kuniharu　Higano, CC BY 4.0

# Introduce
GPS　Drawingを使ってサカナクションの「新宝島」の歌詞を表現する。きっかけは私がサカナクションの山口一郎さんとインスタライブコラボしたことである。サカナクションと日向野邦春という一生切っても切り離せない関係を表すためにこの課題に取り組んだ。

# Methods
①地図上で歌詞にあった道を見つけてStravaを起動させて歩いていく。一文字ずつ切り離して表現していくためその都度新しいランニングやウォーキングを作成する。出来るだけ道の上で表現したいが、夜や新などの難しい漢字は公園などで歩いて表現していく。

②StravaからGPXファイルを抽出してして[GeoJson io](https://geojson.io/#map=2/20.0/0.0)でGeoJsonファイルを生成する。<img width="1920" alt="スクリーンショット 2022-01-31 0 21 16" src="https://user-images.githubusercontent.com/40018527/151705822-5775ea43-cfa5-4725-8f8a-55cd2c633518.png">
この時に漢字で切り離して描いた文字は複数のGPXデータを入れて１文字のGeojsonファイルとする。また③以降で仕様するMapbox Studioでは16以上のレイヤーを読み込むことができないため文字が被らないように全ての文字を15ファイルに振り分けていく。

③GeoJsonファイルを歩いた形跡が被らないように15のレイヤーに分けてMapbox Studioに入れて,opacity(透過率)は0に設定しておく<img width="1918" alt="スクリーンショット 2022-01-31 0 22 55" src="https://user-images.githubusercontent.com/40018527/151705878-5e12bb01-5cbe-4ca9-96a8-a5d83414a3aa.png">
よくやりがちなミスでファイル名を日本語にしてしまうことがある。そうするとStudioで識別されずにtrueというファイルになってしまうので注意。このプロジェクトの場合はkanji_egaku.geojsonこのような形式とする。

④[Mapbox Storytelling](https://github.com/mapbox/storytelling)を使って文字を歌詞通りに表示させる。<img width="1512" alt="スクリーンショット 2022-01-31 0 30 07" src="https://user-images.githubusercontent.com/40018527/151706138-45a25ee7-da25-4140-9f4b-2af51386a69f.png">
[Mapbox storytellingチュートリアル](https://www.mapbox.com/webinars/storytelling-template-live-demo)


# Result

# Disccussion

## GPS Drwingは音楽と文字をつなげる存在となる
GPS Drawingというのは2000年にはすでに確立していた。GPSの進歩に伴いより鮮明な文字や絵を描くことが出来るようになった。しかし、今回「音楽×地図」という新たな表現手法を試みた。その結果として、今までは音だけに価値があった音楽に「場所」という価値（聖地）を作ることができた。これにより多くのファンが真似をし、異なるアーティストや楽曲でも挑戦する事例が出てくると考えられる。



## 参考文献
https://docs.google.com/spreadsheets/d/1g2eXWUpb1BTOZNJHFsx37w00CYwMpBDHIwD3CEFXTY8/edit?usp=sharing

## 当日スライド
https://www.mapbox.com/webinars/storytelling-template-live-demo

## 先行研究
猪苗代湖ズ / I love you & I need you ふくしま [MORE ACTION, MORE HOPE]
https://youtu.be/sQEVUsHt1Bk

沖縄ファミリーマート 国道508号線「結」特別編　180秒CM
https://youtu.be/pUPWhE2Cm4s

THE BOOM 島唄　PV　20周年記念 ver
https://youtu.be/Oq9RkXOyFnY

Stand By Me | Playing For Change | Song Around The World
https://youtu.be/Us-TVg40ExM

Mela! - 全国のアカペラ2年生 & 緑黄色社会
https://youtu.be/bKkXOdZrXVY





