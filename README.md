# ImageStandUp-NWjs

Electron の仕様が面倒くさくなったので新設

## 使い方

1. `images` に好きな画像を入れる。
2. Windows なら `run.bat` を実行、それ以外なら `yarn start` を実行。
3. Canvas 領域にマウスを触れると画像が表示されるので、
   <br>左クリック(上)と右クリック(下)でポジションを設定する。
4. Enter で次の画像へ。1 つ前の設定を繰り返し使う場合は R キーを押すと復元できる。
5. 全画像を設定し終わると変換プロセスが走る。

## ここまでのあらすじ

### HSP 版

https://github.com/katai5plate/ImageStandUp

- HSP 製エディタで上下を設定し、変換は Node から行う
- 画像ログデータは CSV で出力
- 単純に面倒くさい

### Electron 版

https://github.com/katai5plate/ImageStandUp-Electron

- エディタと変換が統合
- 画像ログデータはここから json に
- R キーを押すことで１つ前のポジション情報を読み込める機能もここから
- ローカルデータの読み込みに制約がついたのでやめることにした
