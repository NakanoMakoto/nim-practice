# コンパイル方法

## 開発中のコンパイル方法

--run　オプションを付与することにより、コンパイルして実行する
```
nim compile --run "file name"
```

コマンドライン引数は以下のように渡せる
```
nim compile --run "file name" arg1 arg2
```

ショートハンド
```
nim c -r "file name"
```

## デプロイ時のコンパイル方法

リリースバージョンはこのように  
ランタイムチェックがされず、最適化が図られる
```
nim c -d:release "file name"
```