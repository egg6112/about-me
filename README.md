# egg6112の自己紹介ページ

このリポジトリは **GitHub Pages** で自己紹介ページを公開しています。

## 公開URL

**https://egg6112.github.io/about-me/**

## プロジェクト

自己紹介ページ本体に加えて、以下の学習プロジェクトを公開しています。

### 📊 MLB 日本人野手の打撃特徴分析 — 2024 Statcast Dashboard

大谷翔平・吉田正尚・鈴木誠也の3選手の打撃を、2024 シーズンの Statcast データ約162,000打球と比較したダッシュボード。
Launch Angle と Exit Velocity を軸に、3者三様の打撃タイプを可視化しています。

- **公開ページ:** <https://egg6112.github.io/about-me/projects/mlb-j-analysis-01/>
- **データソース:** Baseball Savant (Statcast) / pybaseball 経由
- **使用技術:** Python · pandas · matplotlib · seaborn
- **発見の要点:** 鈴木誠也のライナー打球の質(wOBAcon 0.79)が、大谷の0.71を上回る ⭐

### 🧩 15パズル アルゴリズム比較ビジュアライザー

A* と IDA* を同じ盤面で並走させ、探索過程をリアルタイムに可視化するアプリ。
Manhattan Distance + Linear Conflict ヒューリスティックを採用。

- **公開ページ:** <https://egg6112.github.io/puzzle-visualizer/>
- **使用技術:** HTML · CSS · JavaScript

### ⚔️ 決戦・関ヶ原 3D俯瞰シミュレーション `CLAUDE FABLE5`

慶長五年九月十五日、天下分け目の関ヶ原をリアルタイム3Dで再現。
地形・14部隊・進軍矢印・朝霧・シネマティックカメラをブラウザで体験できる。

- **公開ページ:** <https://egg6112.github.io/sekigahara-3d/>
- **使用技術:** React · Three.js · GitHub Pages

### 🌌 三体問題 カオス軌道シミュレーター `CLAUDE FABLE5`

重力で引き合う3天体のカオス軌道をリアルタイム描画。
4次ルンゲ=クッタ法 + 適応刻み幅による高精度物理エンジンと、加算合成の発光軌跡で視覚的な美しさも追求。

- **公開ページ:** <https://egg6112.github.io/three-body-simulator/>
- **使用技術:** React · Canvas 2D API · Vite · GitHub Actions

## ファイル構成

| ファイル / フォルダ                    | 説明                                          |
| ------------------------------ | --------------------------------------------- |
| `index.html`                   | 自己紹介ページ本体（HTML/CSS/JS 一体型）          |
| `projects/mlb-j-analysis-01/`  | MLB 日本人野手の打撃特徴分析ダッシュボード           |
| `CLAUDE.md`                    | Claude Code 用のプロジェクト憲法                  |
| `NOTES.md`                     | 開発メモ                                        |
