<!-- English: [README.md](./README.md) — 片方を直したら、同じコミットでもう片方も直してください -->

# hora-ort-sample-spec

[Hora Kit](https://github.com/openreachtech/hora-core) で作った小さなアプリケーションについて、Hora Kit が生成した仕様書のサンプル集です。

## 何が置いてあるか

ディレクトリ1つがアプリケーション1つで、`/hora-spec` が書いたままの仕様書を収めています。

```
<application>/
  specs/<version>/spec.md     仕様書。承認された1節ずつ書かれたもの
  README.md                   そのアプリケーションが何をするか、作るのに何が要ったか
```

**後から書き直したものはありません。** ここにある仕様書は、実行が実際に生成し、実際にそれを元に作られた文書そのものです。公開する意味はそこにあります。読んで引っかかる行があれば、本物でも同じように引っかかります。

## 読んで得られるもの

- **完成した Hora Kit の仕様書がどんな見た目か** — どの節があり、各節がどの粒度まで書かれ、受入基準が「関所が判定できる形」でどう表現されるか。
- **どれだけが対話で決まるか。** `/hora-spec` は尋ね、提案し、承認されたものだけを書きます。完成した仕様書は、その回答の記録です。
- **規模の目安。** ここにあるのは1日で作り切れる大きさのアプリケーションなので、仕様書も通しで読める長さです。

## 仕組みの documentation

| | |
|---|---|
| 各コマンドが何をするか | `hora-core` の [`commands.ja.md`](https://github.com/openreachtech/hora-core/blob/main/docs/commands.ja.md) |
| 作業がどう実行されるか | `hora-core` の [`architecture.ja.md`](https://github.com/openreachtech/hora-core/blob/main/docs/architecture.ja.md) |
| 仕様書の書式 | [`spec-format.md`](https://github.com/openreachtech/hora-core/blob/main/kit/skills/hora/references/spec-format.md) |
| キットでプロジェクトを始める | [`hora-boilerplate`](https://github.com/openreachtech/hora-boilerplate) |

## コントリビューション

サンプルは「ディレクトリを1つ足すプルリクエスト」として入ります。中身は生成された仕様書と、そのアプリケーションの説明を書いた README だけです。それ以外は手を加えません。

## ライセンス

本プロジェクトは Apache License 2.0 で公開しています。

詳細は [LICENSE ファイル](./LICENSE) をご覧ください。

## 開発元

[Open Reach Tech Inc.](https://openreach.tech)

## 著作権

© 2026 Open Reach Tech Inc.
