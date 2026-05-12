# タイタニック号生存予測 - 機械学習

## 概要
KaggleのTitanic - Machine Learning from Disasterコンペに参加。
ランダムフォレストを用いて生存者を予測しました。

## 結果
- **Kaggleスコア：0.77990**（上位約20%）
- 訓練精度：86.31%

## 使用技術
- Python
- Pandas / NumPy
- scikit-learn（RandomForestClassifier）

## 工夫した点
- 名前から敬称（Mr/Mrs/Miss等）を抽出して特徴量に追加
- 家族人数・一人旅フラグを新たに作成
- 過学習を防ぐためmax_depthを調整

## スコア改善の記録
| バージョン | スコア | 改善内容 |
|---|---|---|
| V1 | 0.73205 | ベースラインモデル |
| V2 | 0.77990 | 特徴量エンジニアリング追加 |
