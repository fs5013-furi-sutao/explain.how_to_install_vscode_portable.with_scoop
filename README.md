# explain.how_to_install_vscode_portable.with_scoop
Scoop を使って VSCode のポータブル版を導入する方法を説明する

## Scoop でインストール
Scoop に存在するか、どの Buckert にあるかを確認する。
```console 
scoop search vscode-portable
```
実行結果:
```
'extras' bucket:
    vscode-portable (1.49.2)
```

extras バケットにあるのが分かる。

VSCode Portable をインストールする。
```console
scoop install vscode-portable
```

## 実行ファイルの場所
```
C:\Users\＜ユーザ名＞\scoop\apps\vscode-portable\current\Code.exe
```

## ユーザデータの格納場所
```
C:\Users\＜ユーザ名＞\scoop\apps\vscode-portable\current\data
```

この data フォルダの中にユーザ設定や拡張機能がすべて保存される。そのため、他の VSCode を利用する際も、この data フォルダを実行する Code.exe の階層に置けば、同じ状態、同じ設定で VSCode を使用することができる。

## Update
VSCode Portable を更新する。
```console
scoop update vscode-portable
```

## アンインストール
VSCode Portable をアンインストールする。
```console 
scoop uninstall vscode-portable
```
