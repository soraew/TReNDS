# TReNDS
TReNDS kaggle competition (ensembling + stacking)

kaggleで初めて参加したTReNDSコンペ（脳の活性の仕方から年齢を特定するもの）で書いたコード

Ridge, Elastic-Net, SVRを1st stage modelとして、
それらの予測の重み付平均をLightGBMを2nd stage modelとしてスタッキングして学習したもの。

SVRはsklearnのものに比べてNVIDIAのcumlのものの方が倍速かった為、そちらを使用。
