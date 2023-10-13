# Golangとwailsで簡単なアプリを作ってみた．

https://wails.io/ja/docs/gettingstarted/installation
* とりあえずこの公式チュートリアルサイトから環境構築し，ひとまずtypescriptのテストアプリケーションの実行まで行けた．
* ここからたくさん弄り倒して使い勝手を確認したい．

```go
go install github.com/wailsapp/wails/v2/cmd/wails@latest
```
これでwailsをインストール
```go
wails doctor
```
これでwailsがインストールされているかを確認する
## mdb-react-ui-kitのインストール
* uiの開発効率を上げるため，mdb-react-ui-kitというライブラリをインストールする
	
	まずはnpmコマンドでインストールする
	```bash
	npm i mdb-react-ui-kit
	```

	fontawesomeをダウンロード
	```bash
	npm i @fortawesome/fontawesome-free
	```

	/frontend/src/**main.tsx**に以下のコードを追記し，mdb-react-ui-kitのstyle関係のファイルをインポートする．
	```css
	import 'mdb-react-ui-kit/dist/css/mdb.min.css';
	import "@fortawesome/fontawesome-free/css/all.min.css";
	```

	https://mdbootstrap.com/docs/react/#demo
	
	このサイトを参考に色んなUIを実装できる．