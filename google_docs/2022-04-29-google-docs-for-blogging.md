---
title: Googleドキュメントでブログを書く
---
Googleドキュメントで記事を書けるブログシステムをつくった。

*   [https://github.com/r7kamura/godolog](https://github.com/r7kamura/godolog) (ソースコード)
*   [https://r7kamura.github.io/godolog-example/](https://r7kamura.github.io/godolog-example/) (デモサイト)

※[r7kamura.comに投稿した記事](https://r7kamura.com/articles/2022-04-30-google-docs-for-blogging)と同じ内容の記事を、サンプルとしてここに再掲載しています。

使い方
---

次の手順で、GitHub Pagesでブログを公開できる。

1.  GitHubでテンプレートから新しいリポジトリをつくる
2.  Google CloudでサービスアカウントとOIDCの設定をする
3.  Google Driveでフォルダをつくりサービスアカウントと共有する
4.  GitHubでOIDCの設定値をSecretsに保存する

詳しくはソースコードのREADMEを読むのが吉。

設定を済ませると、フォルダ内のドキュメントが定期的に記事として反映されていくようになる。注意点として、ドキュメントのファイル名に制約があり、“2022-05-05-foobar” のような形式にする必要がある。

既存ブログへの導入
---------

[google-docs-to-github](https://github.com/r7kamura/google-docs-to-github)というcustom actionも用意している。GoogleドキュメントをMarkdownファイル化してリポジトリにPushする機能を提供しているので、既存のブログと組み合わせる場合なんかはこれが便利に使える。最初に紹介したテンプレートでもこれを利用している。

なぜつくったか
-------

Googleドキュメントはエディタが非常によく出来ているので、これで直接ブログ記事を書けたら最高だろう、ということで今回こういうものをつくってみた。

r7kamura.comにも導入してみていて、この記事もGoogleドキュメントで書いている。Googleドキュメントで記事を書けて本当に捗っている。知り合いを共同編集者やレビュアーとして誘えるようになったし、オフラインで書けるモバイルアプリもあるので、外出先でもブログを書けて最高。導入したときの話は『[Googleドキュメントに対応](https://r7kamura.com/articles/2022-05-04-diary)』という記事にも書いている。
