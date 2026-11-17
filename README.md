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
