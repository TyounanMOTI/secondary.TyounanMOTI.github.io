# GitHub Pagesでブログ記事を書く方法
Markdown記法でGitHub Pagesにブログ記事を書く方法を解説します。

# 前提知識
- GitHubを使える
- Gitを使える

# やりかた
1. [ユーザー名].github.io というリポジトリを作る
2. index.md にMarkdown記法で記事を書く
3. GitHubにgit pushする
4. https://[ユーザー名].github.io/ をブラウザで開く

これだけ！

# 補足
手順3 -> 4は１分くらい待つといけるかも。

# 仕組み
1. git push
2. GitHubのサーバー上で[Jekyll](https://jekyllrb.com/)が動く
3. 静的なWebサイトが生成される

たぶんこんな感じ。

# 次は？
[見た目を変えてみよう！](jekyll_github_pages_theme.html)
