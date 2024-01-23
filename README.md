# Prog2kakushin
<h2>プログラム１について</h2>
<h3>プログラムの概要</h3>
<p>このプログラムはインプット関数によって指定されたURLを調べ、そのHTMLファイルなどに含まれているコンテンツのリンクを探し出すプログラムです。</p>
<p>またこのプログラムは指定されたURLから見つかったリンクを使ってさらにコンテンツのリンクを調べています。</p>
<h3>どういったときに使うか</h3>
<ul type="disc">
<li>webページから何か検索したいものがありそのURLが分からないとき</li>
<li>webページが何を呼び出しているか気になった時</li>
<li・webページについて勉強したい時(javascriptがどのように使われているかなど)</li>
</ul>
<h3>入力と出力</h3>
<p>入力はユーザが詳しく調べたいか気になるURLを入力する</p>
<p>出力はページのソースから検出されたURLをPandasのデータフレームとして出力</p>
<p>項目は検出したURLとそのタイプ</p>
<p>拡張子で判断しているため設定していないものはすべて欠損値NaNで出力される</p>
  
<h2>プログラム2について</h2>
<h3>プログラムの概要</h3>
<p>このプログラムは〇×ゲームです。ユーザはどのサイズで〇×ゲームをするかスライダーのフォームで選択することができます</p>
<p>自分を0、相手を8として〇×ゲームが始まります。ルールはほかのものと同じように縦横斜めのいずれかで自分のマークが並んだら勝利です</p>
<h3>どういったときに使うか</h3>
<ul type="disc">
<li>〇×ゲームがしたい時</li>
<li>〇×ゲームの動作を確認したい時</li>
</ul>
<h3>入力と出力</h3>
<p>まずユーザーは自分が先攻か後攻かを入力します</p>
<p>その後、自分が置きたい場所に何行何列という感じで指定し、入力します</p>
<p>その結果、自分が指定した場所に自分のマークが置かれ、なおかつ相手のマークもおかれた状態で出力されます</p>
<p>そしてまた置きたい場所を指定する入力を行います。</p>
<h3>工夫した点</h3>
<p>ユーザが何×何の盤面でやりたいかフォームのスライダを使い指定できるようにした</p>
<p>それに伴いフォームのスライダ変数で置き換えられるものは置き換えることでどの盤面でも動くようにした</p>
<p>ユーザが求められていない数字や文字を入力したときは注意とともにもう一度入力できるようにした</p>

<h2>プログラム3について</h2>
<h3>プログラムの概要</h3>
<p>このプログラムは簡易的にステガノグラフィー解析をできるプログラムです</p>
<p>内容としては次のように処理した画像を見ることができます</p>
<ul type="disc">
<li>ビットのXOR演算（反転処理）</li>
<li>赤色のみ抽出</li>
<li>緑色のみ抽出</li>
<li>青色のみ抽出</li>
<li>ビット左ローテート処理（左にシフトして、その沖あふれたものを最下位ビットに送る）<br>大体0~6,7ビットぐらいまで</li>
<li>赤色のビット抽出　大体0~6,7ビットぐらいまで</li>
<li>緑色のビット抽出　大体0~6,7ビットぐらいまで</li>
<li>青色のビット抽出　大体0~6,7ビットぐらいまで</li>
<li>輝度半分</li>
<li>輝度２倍</li>
<li>ビットプレーン（RGBの同じ位の１ビットに対して0だったら255、逆は0にして画像を出力）<br>大体0~6,7ビットぐらいまで</li>
</ul>
<h3>どういったときに使うか</h3>
<ul type="disc">
<li>画像を面白くしたい時</li>
<li>画像にフィルターをかけたい時</li>
</ul>
<h3>入力と出力</h3>
<p>colabにアップロードしたもののパスをコピーしてimreadのところに張り付け</p>
<p>自分が行いたい処理に合わせてimshowの部分を適切な関数に変更</p>
<h3>工夫した点</h3>
<p>輝度二倍が8ビットのため左シフトしてしまい全く違う画像になってしまったので条件を追加した</p>
<p>できるだけビットに直して処理を行うようにした（ローテートなどがうまくいっているか確認できるようにするため）</p>
<p>使いまわせるデータは使いまわすようにした（画像の幅、高さなどの値）</p>
<h3>どんなフィルタをするか参考にしたソフト</h3>
<p>青い空を見上げればいつもそこに白い猫　for　うさみみハリケーン</p>
