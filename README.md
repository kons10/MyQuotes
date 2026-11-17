# QuoteiFrameHugo

Hugo で生成するランダム語録・歌詞フレームです。

## iframe への埋め込み

通常ページ（サイトのトップページ）を iframe に指定できます。表示領域の幅・高さに合わせて、文字サイズや余白が自動調整されます。

```html
<iframe
  src="https://YOUR-DOMAIN.example/"
  title="ランダム語録"
  width="420"
  height="240"
  loading="lazy"
  style="width: 100%; max-width: 420px; height: 240px; border: 0;"
></iframe>
```

`width` と `height`、または CSS の `width` と `height` を変更することで、任意の表示サイズに調整できます。実際の公開 URL に合わせて `src` を変更してください。


## 語録に画像を付ける

各語録 Markdown の front matter に \`image\` と \`image_alt\` を指定すると、画像付きレイアウトになります。

画像ファイルは \`static/images/\` に配置します。たとえば \`static/images/quote-01.jpg\` を使う場合：

\`\`\`yaml
---
title: "語録タイトル"
author: "作者"
image: "/images/quote-01.jpg"
image_alt: "画像の説明"
---
語録本文
\`\`\`

- **画像あり：** 広い表示領域では左に画像、右に語録を表示します。
- **小さなiframe：** 画像を上、語録を下に配置します。
- **画像なし：** 語録を従来どおり中央に表示します。
- 画像は自動でモノクロ表示になります。元画像ファイルは変更されません。

\`image\` を省略すれば、画像なしの表示になります。
