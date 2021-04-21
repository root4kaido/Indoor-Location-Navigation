# Indoor-Location-Navigation

https://www.notion.so/Indoor-b2d7162c354a4d04ba5865b3dbe04665

- 01…[floor予測モデル](https://www.kaggle.com/nigelhenry/simple-99-accurate-floor-model/output)を，pythonで再現実装
- 02…[lgbmモデル](https://www.kaggle.com/hiro5299834/wifi-features-with-lightgbm-kfold)の再実装
- 03…02でできたモデルに対し，floorを01のものに変更
- 04…02を，Groupkfoldに変更
- 05…LSTMのベースライン．[kutoさんのもの](https://github.com/kuto5046/kaggle-indoor/tree/main/exp/exp001)を参考．
- 06…05に[このデータセット](https://www.kaggle.com/dataset/71ef8af781d8e4f976c45c88075da463a6df4116c77f59c1db3c138308793dda)を使ってtime_diffを入れたもの．
- 07…05からsite_idをぬいたもの
- 08…07かた，time_diffの大きいものを抜いたもの
- 09…05をBiLSTMにしてみた
- 10…koukiさんの新しい方の[データセット](https://www.kaggle.com/kokitanisaka/make-dataset-with-wi-fi-and-beacon)(とりあえず，ibeacon無し)
- 11…10にtimegap追加
- 12…timegapの順番に変更
- 13…ビーコンも入れた
- 14…クボタさんデータセット(posxだけ)追加
- 15…posyも追加
- 16…transformerに手を出したけどエラーとれん！！
- 17…metadataの画像を使ってみた
- 18…contrastive learningを使ってみた
- 19…rssiをembeddingにした
- 20…18でつくったembedding空間を使う
- 21…17と大体一緒
- 22…5のベースにおいて，後処理2つを行った
- 23…wifiの出現回数閾値を50にした．また，ここからオリジナルのデータセット使ってる．
- 24…23の，閾値10バージョン
- 25…22で，rssiもembeddingにした
- 26…22に，画像のデータ(contrastive learning後)も追加
- 27…26で，画像のデータをconcatするだけでなく，学習にも用いる
- 28…wifiの閾値を1にしてみた
- 29…100行じゃなくて200行にしてみた
- 30…全部embeddingにした
- 31…並びを，交互になるように変更
- 32…waypointベース
- 33…wifiの下限を増やした
- 34…31でfreq追加
- 35…lastseenとwaypointのtime差離れてるもの削除(trainだけ)
- 36…35，testも
- 37…time差を20秒に変更
- 38…10秒に変更

other

- make_Dataset…データセット作った
