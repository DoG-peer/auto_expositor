data
	基礎ファイルが置いてある．
	header.tex
	tail.tex
	があり，これらに挟まれる形でtexファイルを生成する．
	パッケージを追加する時はここにかく．


lib
	ライブラリのフォルダここにライブラリを入れる．
	ライブラリを公開する時は，他の人のライブラリと名前が被らず，中身の扱うテーマが分かるような名前をつけましょう．
	auto_expositor\lib\<ライブラリ名>
	中身は
	auto_expositor\lib\<ライブラリ名>\hoge.tex
	auto_expositor\lib\<ライブラリ名>\ref.bib
	texファイルは一行目に
%tag : tag0 tag1 tag2 ･･･
	というようにタグを入れる．スペースの個数を間違えないよう注意してください
	bibファイルは通常通りに作成．ただし，ほかのライブラリとラベル名が被らないように，
	ライブラリ名_本来つけたいラベル名というようにするのを勧めます．

config.ini

	用いるライブラリを指定する．書き方は，
	library all
	ですべて指定．
	指定したい時は，
	library lib0 lib1 lib2 ･･･
	と書く

a.txt
	ここにチェックしたい文章を書く

main.rb
	いろいろ出来たらこれを実行！

temp/temp.tex
temp/temp.pdf
	完成したtex・pdfファイル


おまけ
auto_expositor.exe
	わざわざそれぞれのファイルを作るのが大変なので，これを使っていただけるとよろしいかと
	メイン
		a.txtを編集してmain.rbを動かしてってするのをまとめてしてくれる．

	config
		config.iniを編集する．チェックを入れるだけで設定が出来る！
	ライブラリ作成
		libの中身を作る
	ライブラリ要素
		lib/hogeの中身を作る

src/auto_expositor.hsp
	auto_expositor.exeのソース