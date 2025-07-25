## マインクラフトのデータパックで作られた、
# mcfunctionファイルを一回だけ実行するためのものです。
### 製作者:reizou_00


## 対応バージョンは以下の通りです。

1.21.4(以外でも動くかもしれないが確認していない。)

## 使い方。
### 実行方法
#### 基本型
```mcfunction
/function reizo_onlyonce_lib:_ {func:"<ここに実行したいファイルのパスを記入>"}
```
#### プレイヤー型
``` mcfunction
# 実行したいエンティティを対象にして...
/function reizo_onlyonce_lib:player {obj:"実行したいファイルの名前とか...任意の物。",func:"<ここに実行したいファイルのパスを記入>"}
```
### リセット方法
##### 基本型
```mcfunction
# 「0b」は「false」でもいい
data modify storage reizo_onlyonce:_ <ここに実行したファイルのパス> set valuse 0b
```
#### プレイヤー型
```mcfunction
# 絶対に値は0以外にしないこと
scoreboard players set <セレクター> 0
```

## License

## License

[![CC BY 4.0](https://licensebuttons.net/l/by/4.0/88x31.png)](https://creativecommons.org/licenses/by/4.0/)

This project is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

要するにこれは「使うときは僕の名前だけどっかに書いとけばいいよ～」ってこと