# AR Character Test

GitHub Pagesで確認する用のMindARサンプルです。

## ファイル構成

- `index.html`
- `assets/character.webm`
- `assets/target.mind`

## GitHub Pagesで公開する手順

1. GitHubで新しいリポジトリを作成
2. このフォルダ内の `index.html` と `assets` フォルダをアップロード
3. リポジトリの `Settings` → `Pages`
4. `Build and deployment` の `Source` を `Deploy from a branch` にする
5. `Branch` を `main` / `/root` にして `Save`
6. 数十秒〜数分後に表示されるURLをスマホで開く

## 調整場所

`index.html` 内の以下を変更すると、キャラクターの大きさや位置を調整できます。

```html
<a-video
  position="0 0 0"
  width="1"
  height="1">
</a-video>
```

- 大きくしたい：`width="1.3" height="1.3"`
- 上に動かしたい：`position="0 0.2 0"`
- 下に動かしたい：`position="0 -0.2 0"`
