# HTMLファイル編集規定

## 商品紹介ページHTML
	<!-- 編集箇所１カラム目 -->
		<div class="column">
			<img src="http://rakuten.brotures.com/cabinet/items/leaderbike/721/721-black-03.jpg" alt="" class="column-image">
			<h4>リーダーバイクを知るには、このフレームから</h4>
			<p>
				全ての人にLEADER BIKEを体感して欲しい、そんな思いが込められ全ラインナップの中で最も幅広くサイズを揃えている。
				<br>
				手元が高いライザーハンドルは初めてピストに乗る方でも戸惑うことがない。
				<br>725・735とは異なるアルミ材を用いることで、フレーム自体の作りの頑丈さにも定評がある。
			</p>
		</div>
	<!-- 編集箇所２カラム目 -->
		<div class="column">
			<img src="http://rakuten.brotures.com/cabinet/items/leaderbike/721/721-black-04.jpg" alt="" class="column-image">
			<h4>エントリー向けでも妥協なし</h4>
			<p>
				スローピング形状のフレームは乗り降りや停車時など跨がった状態での足付きがいいので通勤や通学など、日常あらゆるシーンで活躍できる。
				<br>
				しかし、ドロップハンドルやブルホーンハンドルをセットすると、一転してストイックで攻撃的な表情を見せる。
				<br>まさに万能型のエントリーフレーム、リーダーを乗り始める方にはまずこのフレームを試していただきたい。
			</p>
		</div>

上記の`<img src="">`と`<p></p>`の部分を編集。  
画像URLは楽天cabinetではなく、別のサーバーで用意する。

## スペック紹介ページ
まずはヘッダーのmetaデータとlinkを変更

	1 <!doctype html>
	2 <meta charset="utf-8">
	3 <link href="http://www.rakuten.ne.jp/gold/brotures/css/spec.css" rel="stylesheet" />
	
↓

	1 <!DOCTYPE html>
	2 <meta charset="utf-8">
	3 <meta name="robots" content="noindex,nofollow">
	4 <meta http-equiv="X-UA-Compatible" content="IE=edge">
	5 <link href="../../stylesheets/bootstrap.css" rel="stylesheet">
	6 <link href="../../stylesheets/custom.css" rel="stylesheet">
	7 <link href="../../stylesheets/product.css" rel="stylesheet">

テンプレートに従い、項目と内容を記述。  
偶数奇数のクラス名（odd,even）を順番通りに必ずつけること。

	<!-- スペック編集箇所 -->
	<div id="spectab">
		<div id="tab1">
			<table class="geotable" border="0">
				<tbody>
					<tr class="odd">
						<td class="title">Weight</td>
						<td>310g</td>
					</tr>
					<tr class="even">
						<td class="title">Size</td>
						<td>700c</td>
					</tr>
					<tr class="odd">
						<td class="title">Hole</td>
						<td>32H</td>
					</tr>
					<tr class="even">
						<td class="title">Color</td>
						<td>BLACK (Side CNC)</td>
					</tr>
				</tbody>
			</table>
		</div>
	</div>
