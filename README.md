# TReNDS
 TReNDS kaggle competition (ensembling + stacking)

kaggleで初めて参加した(solo)TReNDSコンペ（脳の活性の仕方から年齢を特定するもの）で書いた最終コード(マシンリソースの関係でkagggle notebook上で書いたもの)
テーブルデータのみを使用。

Ridge, Elastic-Net, SVRを1st stage modelとして、
それらの予測の重み付平均をLightGBMを2nd stage model(meta model)としてスタッキングして学習したもの。

SVRはsklearnのものに比べてNVIDIAのcumlのものの方が数倍速かった為、そちらを使用。


----

Code I wrote for the first kaggle competition, TReNDS neuroimaging that I participated in.
I participated solo and wrote this notebook on the kaggle notebook enviroment.
I only used the table data.

Used Ridge, Elastic-Net, SVR as 1st stage model and stacked LightGBM as 2nd stage model(meta model) on top of the weighted average of their predictions.

I used SVR from rapids cuml library because it was several times faster than that of the sklearn library.

