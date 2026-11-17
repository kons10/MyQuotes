# QuoteiFrameHugo

Hugo で生成するランダム語録・歌詞フレームです。

## エディション

- **通常版**: `/`
- **iframe edition**: `/embed/`

iframe edition は埋め込み先で指定された幅・高さに合わせて表示を調整します。小さい領域では文字や余白を縮小し、内容が収まりきらない場合はページ内をスクロールできます。

### 埋め込み例

```html
<iframe
  src="https://YOUR-DOMAIN.example/embed/"
  title="ランダム語録"
  width="420"
  height="240"
  loading="lazy"
  style="width: 100%; max-width: 420px; height: 240px; border: 0;"
></iframe>
```

`width` と `height`、または CSS の `width` と `height` を変更することで、任意の表示サイズに調整できます。実際の公開 URL に合わせて `src` を変更してください。
