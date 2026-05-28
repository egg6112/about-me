# egg6112の自己紹介ページ

このリポジトリは **GitHub Pages** で自己紹介ページを公開しています。

## 公開URL

**https://egg6112.github.io/about-me/**

## プロジェクト

このリポジトリでは、自己紹介ページ本体に加えて、サブディレクトリ `projects/<name>/` 配下に学習プロジェクトを配置しています。

### 📊 MLB 日本人野手の打撃特徴分析 — 2024 Statcast Dashboard

大谷翔平・吉田正尚・鈴木誠也の3選手の打撃を、2024 シーズンの Statcast データ約162,000打球と比較したダッシュボード。
Launch Angle と Exit Velocity を軸に、3者三様の打撃タイプを可視化しています。

- **公開ページ:** <https://egg6112.github.io/about-me/projects/mlb-j-analysis-01/>
- **データソース:** Baseball Savant (Statcast) / pybaseball 経由
- **使用技術:** Python · pandas · matplotlib · seaborn
- **発見の要点:** 鈴木誠也のライナー打球の質(wOBAcon 0.79)が、大谷の0.71を上回る ⭐

## ファイル構成

| ファイル / フォルダ                    | 説明                                                            |
| ------------------------------ | ------------------------------------------------------------- |
| `index.html`                   | 自己紹介ページ本体（HTML/CSS/JS 一体型）                                    |
| `projects/mlb-j-analysis-01/`  | MLB 日本人野手の打撃特徴分析ダッシュボード(Statcast 2024)                         |
| `CLAUDE.md`                    | Claude Code 用のプロジェクト憲法                                        |
| `NOTES.md`                     | 開発メモ                                                          |

## GitHub Pages の有効化方法

まだ有効化していない場合は、以下の手順で設定してください。

1. このリポジトリの **Settings** を開く
2. 左メニューの **Pages** をクリック
3. **Source** のドロップダウンで `main` ブランチを選択
4. **Save** を押す
5. しばらく待つと上記の公開URLでアクセスできるようになる
