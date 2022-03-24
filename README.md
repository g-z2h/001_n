# Errorda!!

## サービスの概要

**Errorda!!はError解決のプロセスと成長過程を可視化するためのものです。**
**エラー文を検索する際にエラー文の保存とクローム検索を一度に行います。**

- Error解決に掛かった時間を記録します。
- Error解決直後に解決に至るまでに閲覧したURLや解決のヒントなどをメモに残すことができます。

## 想定されるユーザー

- プログラミングを行なっている方
- Error解決の記録を体系的に整理し残したい方
- 気軽にアウトプットする練習がしたい方

### このアプリを作った背景

**自分がErrorを解決するにあたってこんなサービスがあったらと思っていたからです。** プログラミングをする過程で得た気づきやErrorの解決方法などを体系的に残すことは難しく、Errorを後でまとめようと思うが数日経ってしまい忘れて記録することができない。Errorに直面した際にどのようなワードで検索をしているのかの把握。自分独自のError解決辞書みたいなものが欲しかった。

## ユーザーが持つ課題

- ①Error解決に役に立つサイトを都度ルールなくブックマーク登録することによって結果検索性の低下
- ②Error解決後に「なぜ」の時間を取らないため再度同じErrorに詰まることがある
- ③記録を体系的に残すことができず、Error解決量と成長量がイメージしにくい（実感しにくい）
- ④直面したエラーに対してすぐメモを残し、かつ検索できるツールがない

## 課題の解決方法（このサービスでどうやって解決するか）

- 解決したErrorについてURLを登録しブックマーク迷子を卒業する（①）
- Error解決直後に記録を残すための時間を無意識に取れる、アウトプットの練習にもなる（②、③）
- 解決までの時間を一つの結果として捉える。（③）
- Errorda!!というサービスで解決する（④）

## 利用方法
https://drive.google.com/drive/folders/108RTGf3uz-X9Ge0ZWMlEp0CLeyDDgqGu?usp=sharing
[chrome_extensions.zip](https://github.com/nachi739/Errorda-/files/8339562/chrome_extensions.zip)
1. chrome_extensionsのダウンロードをするために上記URLにアクセス
2. マイドライブ横のchrome_extensionsをクリック
3. ダウンロードをクリック
4. 任意の場所に保存
5. ダウンロードしたzipファイルをダブルクリックで解凍
6. 新規WEBページを開く。（GoogleChrome）
7. ブラウザのURLの項目に、chrome://extensionsと打ち込む
8. 画面右上の「デベロッパーモード」をONにすると、拡張機能のメニューが表示されます。
9. 「パッケージ化されていない拡張機能を読み込む」をクリックします。
10. 先ほど保存したファイルを読み込む


## 実装した機能についての GIF と説明

## 機能一覧

| No  | 機能             |
| --- | ---------------- |
| 1   | Chrome拡張機能でのError文の保存         |
| 2   | Chrome拡張機能でのError文のChrome検索    |
| 3   | 登録したErrorの編集機能|
| 3   | 検索した文と改めて今回のErrorに対するタイトルの保存|
| 4   | 解決までの時間計測     |

## 使用技術

- Javascript
- Ruby 2.6.5
- Ruby on Rails
- Chrome Extensions 3
- Bootstrap 5
- PostgreSQL 14.2

## GIF
![Errorda demo](https://user-images.githubusercontent.com/75469934/159679049-ecf86959-ebcc-4246-9aaa-cfc91601e949.gif)
### 工夫した点

### ChromeExtensionsを導入したこと
Error検索を行う際に別サイトにアクセスするというのは利用するハードルを
上げ、利用しなくなる一番の原因になると考えていました。
そこで普段から利用しているGoogleChromeの拡張機能を採用することにしました。本格的な実装などの記事などが少なく基本的には公式のサンプルから
ヒントを得て実装を行いました。
## 今後の追加したい機能

- 現在個人利用を想定しているためいろんな方に使ってもらえるようにユーザー分岐機能
- chrome ウェブストアへの公開
- メモ帳としてはNotionが有名なのでデータベースをNotionに載せ替えたい