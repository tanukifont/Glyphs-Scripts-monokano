# Glyphs用スクリプト
Glyphsで使うスクリプトです。
名称末尾に JP とあるものは日本語フォント作成者向けで、コメントやツールチップなどが日本語で書かれています。

## スクリプトのインストールと実行
### インストール
1. Glyphsのメニューバー［スクリプト > Scripts フォルダを開く］を選択します。
2. ScriptsフォルダがFinderに選択状態で表示されるので、その中に.pyファイルを入れます。

入れただけではGlyphsが認識しないので、以下の操作をしてください。
* optionキーを押しながら、Glyphsのメニューバー［スクリプト > スクリプトメニューを更新］を選択。

これでスクリプトメニューに表示されるようになります。

### 実行
スクリプトメニューで選択して実行します。


### Pythonモジュールのインストール
スクリプトには、ウインドウやボタンなどのGUI上で操作するものがあります。このGUIの生成にPythonモジュールが必要です。以下の操作でインストールしてください。
1. Glyphsの［環境設定 > アドオン > Pythonモジュール］の「インストールする」ボタンを押します。しばらく待つと終了します。
2. インストールが延々と終わらない場合は、Glyphsを再起動して再度ボタンを押してください。何回か繰り返すと終了するはずです。

## スクリプトの説明
* **Switch Direction JP**
  * 編集ビューの組方向（ヨコ／タテ）を切り替えます。
  * スクリプトメニューで選択して実行すると、専用のパネルウインドウが表示されます。そこのボタンを押して切り替えの操作をします。
  * 切り替える際、グリフ表示と情報表示が一致するように更新するのが特徴です。
  * Pythonモジュールが必要。
* **Make vrt2 Glyph JP**
  * 選択グリフを基にvrt2（.rotat）グリフを新規作成します。
    * すでに.rotatグリフがある場合は、そこにベースグリフのコンポーネントを配置します。
    * 選択グリフが.rotatグリフの場合は、そこにベースグリフのコンポーネントを配置します。
  * グリフを選択してから、スクリプトメニューで選択して実行します。
  * Pythonモジュールは不要。
