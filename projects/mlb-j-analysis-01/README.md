# 📊 MLB 日本人野手の打撃特徴分析 — 2024 Statcast Dashboard

大谷翔平・吉田正尚・鈴木誠也の3選手の打撃を、2024 シーズンの Statcast データ
(約 16 万打球)と比較したダッシュボードプロジェクトです。
Launch Angle(打球角度)と Exit Velocity(打球初速)を主軸に、
3者三様の打撃タイプを可視化しています。

🔗 **公開ダッシュボード:** <https://egg6112.github.io/about-me/projects/mlb-j-analysis-01/>

## 分析の目的

「日本人野手」と一括りにされがちな3選手は、Statcast の指標で見ると
本当に共通の特徴を持つのか? それとも個々で全く違うタイプなのか? を検証する。

主軸となる問い:

- 3選手の **Launch Angle × Exit Velocity** の分布はどう違うか?
- その違いは、最終的な打撃結果とどう結びついているか?

## 対象選手とデータ

| 項目 | 内容 |
|---|---|
| 対象選手 | 大谷翔平 / 吉田正尚 / 鈴木誠也 |
| データソース | Baseball Savant (Statcast) を pybaseball 経由で取得 |
| 対象シーズン | 2024 年レギュラーシーズン |
| 母集団 | 2024 シーズンのサンプル 160,234 打球 |
| データファイル | ※ リポジトリでの扱い(.gitignore / LFS / 別管理)は今後決定(TBD) |

## 主な発見

- **大谷翔平** — MLB 標準のスイング分布に、異次元の Exit Velocity(110mph 前後の超高速打球)を乗せたパワー型。
- **吉田正尚** — MLB 水準のコンタクト技術に、Launch Angle を低く保つライナー狙いを組み合わせたタイプ。
- **鈴木誠也** — フライ寄りの打球分布ながら、ライナー時の打球品質はトップ。
  ⭐ ライナー打球の質(wOBAcon **0.79**)が大谷(0.71)を上回るのが本分析最大の発見。

## 使用技術

Python · pandas · matplotlib

## ファイル構成

| ファイル | 説明 |
|---|---|
| `index.html` | ダッシュボード本体(WCAG AA 準拠) |
| `images/fig1_panels.png` | パネル散布図(LA × EV / 3選手 vs MLB密度) |
| `images/fig2_LA_hist.png` | Launch Angle 分布ヒストグラム |
| `images/fig3_EV_hist.png` | Exit Velocity 分布ヒストグラム(大谷の二峰性) |
| `images/fig4_result_share.png` | 打球結果の内訳比較 |
| `images/fig5_woba_by_bbtype.png` | 打球タイプ別 wOBAcon 比較 |
| `images/fig6_quality_rates.png` | 打球品質指標(Barrel率・SweetSpot率・HardHit率)比較 |

## 出典・注記

- 打球データは Baseball Savant (MLB Statcast) を出典とする。
- 本プロジェクトは個人の学習・分析目的で作成したもの。
