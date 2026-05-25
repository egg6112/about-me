# about-me

GitHub Pages で公開している個人ポートフォリオサイト。

公開URL: https://egg6112.github.io/about-me/

## 品質基準

- WCAG 2.1 AA 相当のアクセシビリティを維持する
- 「重要🔴課題ゼロ」を達成条件とする(完璧主義ではなく実用主義)
- 動いている実装を壊さない。低優先度の改善は慎重に判断する

## Git 運用

- main ブランチに直接コミットして OK(1人開発のため)
- コミットメッセージは日本語で書く
- 作業後は **git push まで必ず実行**してから完了報告する
- 完了前に `git status` で `up to date` を確認する

## 作業スタイル

- フロントエンドのレビューは `@portfolio-frontend-reviewer` を活用する
- サブエージェントが矛盾する提案を出した場合、現状維持を優先する
- AI のアドバイスは絶対視せず、メタ認知で判断する

## 触らないでほしい設定

- OGP メタタグ(og:image など)の URL は実機検証済みのため変更不要
- localStorage の try-catch ヘルパー(getStorage/setStorage)は4箇所統一済み
- FOUC 対策のインラインスクリプトは `<head>` 先頭に必須

## 技術スタック

- 素の HTML / CSS / JavaScript(フレームワーク不使用)
- GitHub Pages で自動デプロイ
- 単一ファイル(index.html)構成
