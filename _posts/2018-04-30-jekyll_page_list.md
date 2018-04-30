---
title: GitHub Pagesで記事一覧を出す方法
---

# GitHub Pagesで記事一覧を出す方法
こんな感じの記事一覧を出します。

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>


# やりかた
## 1. `_posts`フォルダに、決まったファイル名で記事を作成
1. `_posts`フォルダを作成
2. YYYY-MM-DD-タイトル.md というファイル名で記事を作成

  例：`_posts/2018-04-30-jekyll_page_list.md`

## 2. 各記事にタイトルを入れる
各記事のファイルの頭に以下のようにタイトルをいれます。

```
---
title: GitHub Pagesで記事一覧を出す方法
---
```

## 3. index.mdに記事一覧を出すコードを追加
index.mdに以下のコードを追加します。

{% raw %}
```
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
```
{% endraw %}

## 4. git push
あとはgit pushするだけ！

# 参考
- https://jekyllrb.com/docs/posts/
