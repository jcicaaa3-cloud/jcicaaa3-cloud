# jcicaaa3

[English](README.md) · [한국어](README_KO.md)

韓国外国語大学でコンピュータ工学を専攻し、北東アジア外交・通商を複数専攻しています。セキュリティと機械学習を一緒に勉強しています。Windowsのランサムウェアを解析していて、機械学習によるマルウェア検知にも取りかかったところです。

[サイト](https://jcicaaa3-cloud.github.io/ja/) · [記事](https://jcicaaa3-cloud.github.io/ja/research/) · [プロジェクト](https://jcicaaa3-cloud.github.io/ja/projects/) · [jcicaaa3@gmail.com](mailto:jcicaaa3@gmail.com)

## マルウェア解析

### Calipsoランサムウェア（2026）

Ghidraで静的解析しました。記事では、暗号化の仕組み（各ファイルの先頭5MBをXChaCha20で暗号化し、セッションキーをRSA-4096 OAEPで包む）、MFTを直接列挙するファイル探索（`FSCTL_ENUM_USN_DATA`）、シャドウコピーやイベントログの削除といった復旧妨害、そしてIOC・YARAルール・MITRE ATT&CKのマッピングをまとめています。

[解析 v2.0](https://jcicaaa3-cloud.github.io/ja/research/calipso-v2/) · [解析画面](https://jcicaaa3-cloud.github.io/ja/evidence/)

マルウェアの検体は公開リポジトリに置きません。

## プロジェクト

### [LiteRaceSegNet](https://github.com/jcicaaa3-cloud/LiteRaceSegNet-FINAL-)

境界ヘッドを持つ、パラメータ0.125Mの道路損傷セグメンテーション用CNNです。検証mIoUは10枚で0.807、CUDAで3.1 ms/枚、7変種のアブレーションがあります。縁の品質はまだ弱く（テストの境界F1は0.058）、READMEにもそう書いています。

### [HPLS-Eval](https://github.com/jcicaaa3-cloud/HPLS-Eval-v0.2.7)

小さなマスクのセグメンテーションを、ランタイム（CPU、GPU、NPU、TPU）と精度（FP32、FP16、INT8）を変えて評価するツールです。実際にどの実行プロバイダーで動いたか、INT8モデルが本当に量子化されているかを確認します。

### [Financial Risk Scoring](https://github.com/jcicaaa3-cloud/financial-risk-scoring-service-FINAL)

企業の四半期データから次の四半期の3つのリスクをスコアにするMLバックエンドです。入力の検証、時系列順の評価、FastAPI、モニタリングのレポートを備えています。データは合成データのみです。

### [MachiLens](https://github.com/jcicaaa3-cloud/machilens-shibuya-ai-predictor)

渋谷の都市戦略シナリオを合成データで比べるBiLSTMモデルです。授業の企画を作り直しました。ランダムフォレストのベースラインのほうが成績がよく、READMEには両方を載せています。

### ロボット動作の成功・失敗評価

ロボットが作業をやり遂げたかをどう判定するかを調べた、2026年1学期の研究プロジェクトです。80回の実験から得た874件を分析し、判定基準によって結果がどう変わるかを見ました。[概要](https://jcicaaa3-cloud.github.io/ja/projects/robot-evaluation/)

## 使っているツール

- マルウェア解析：Ghidra、YARA、MITRE ATT&CK、Python、PowerShell
- 機械学習・コンピュータビジョン：PyTorch、scikit-learn、OpenCV、NumPy、Pandas
- 開発：Git、Linux、FastAPI、Docker、GitHub Actions

## 連絡先

[jcicaaa3@gmail.com](mailto:jcicaaa3@gmail.com)
