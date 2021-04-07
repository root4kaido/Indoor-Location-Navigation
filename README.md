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
- 14…クボタさんデータセット(poxだけ)追加
- 15…posyも追加
