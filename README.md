# 修正版

ユーザーが添付した、元々動いていた index.html をベースにしています。

変更点：
- AR起動の流れは元のまま
- 余計な動画再生ボタンは無し
- キャラ動画をマーカー面から90度起こす設定に変更
- `position` は Y ではなく Z を上げています

調整場所：

```html
<a-video
  src="#characterVideo"
  width="1"
  height="1.7"
  position="0 0 0.85"
  rotation="90 0 0"
  material="transparent: true; side: double;"
></a-video>
```

逆向き・倒れる場合：
- `rotation="90 0 0"` を `rotation="-90 0 0"` に変更
- 表裏が逆なら `rotation="90 180 0"` に変更

高さ：
- `position="0 0 0.85"` の `0.85` を調整
