# Qreki_nako3
　[日本語プログラミング言語「なでしこ３」](https://nadesi.com/doc3/)で、歴史上使用されていた実際の暦と合うよう、文献データを元に西暦と旧暦（和暦）を相互変換したりなんだりするNAKO3プラグインです。（一口に旧暦と言っても幾度も改暦が繰り返されており、人為的に操作が加えられている場合もあるため、天文学的な計算で算出するのは限界があります）

　西暦から旧暦、和暦への変換、和暦から西暦への変換、日単位での元号取得、紀元前の修正ユリウス日の取得や、修正ユリウス日から西暦への変換が出来ます。また、二十四節気や七十二候、干支、九星、六曜などの歴註も取得出来ます。

　現在、旧暦が取得できるデータの範囲は645/2/2(大化元年1月1日)から2099/12/31です。

　また、二十四節気や七十二候が取得できる範囲は、1900～2099年の間です。
 
## 使い方
　[なでしこ３貯蔵庫にライブラリとして公開しています。](https://n3s.nadesi.com/id.php?1778)

　プログラム冒頭で取り込みます。

```
!『https://n3s.nadesi.com/plain/Qreki.nako3』を取り込む。
```


## 旧暦データについて

### 旧暦表

　645(大化元)から2099(令和81)までの元日、閏、月の大小を表にしたもの。

- 「元日」は旧暦1/1の西暦日付。
- 「閏」は閏月がある場合その月番。
- 「大小」は、大の月1、小の月0の配列で、いわゆる大小暦になっています。

　大化元年から明治5年までは『日本暦日原典』を参照。また、『国立天文台 暦計算室』の計算結果の校訂を参照。

　明治6年以降については、なでしこｖ１の旧暦変換で作成。

　2033年問題については『暦文協』の見解に基づき閏11月案に修正。

### 元号一覧

　645(大化元)から2099(令和81)までの元号と改元日のリスト。元号未制定期間は天皇の年期を代用しています。

- 「和暦」は和暦での改元日。
- 「西暦」はそれを西暦に直したもの。
- 「開始」「終了」は元号未制定時期と南北朝の元号並立期間に関連した例外処理用。
- 「南北朝」は、その元号が南朝で使われたものか北朝で使われたものか。

### 参考
- 『日本暦日原典』　内田正男　雄山閣出版　463900091X
- 『国立天文台 暦計算室』　http://eco.mtk.nao.ac.jp/koyomi/
- 『暦文協』　https://www.rekibunkyo.or.jp/top.html

## 歴註データについて

### 二十四節気
- 「二十四節気」
- 「仮名」
- 「新暦」
- 「旧暦」
- 「節中」
- 「暦便覧」
- 「干支」
- 「太陽視黄経」
- 「説明」
- 「六ツ」
- 「算出データ」

### 七十二候
- 「本朝七十二候」
- 「読下」
- 「仮名」
- 「二十四節気」
- 「初次末」
- 「新暦」
- 「説明」

### 十二支
- 「十二支」
- 「仮名」
- 「動物」
- 「時刻」
- 「方位」
- 「五行」
- 「旧暦」
- 「説明」

### 十干
- 「十干」
- 「仮名」
- 「読み」
- 「意味」
- 「説明」

### 参考
- 『現代こよみ読み解き事典』　岡田芳朗・阿久根末忠　柏書房　476010951X
- 『二十四節気の略算式（AddinBox）』　http://addinbox.sakura.ne.jp/sekki24_topic.htm
- 『こよみのページ』　http://koyomi8.com/

## おことわり

　CC0で公開していますので、自己責任で自由にご利用下さい。なでしことか関係なく、データだけ使ってもらっても構いません。

　旧暦の出力については十分確認したつもりですが、万一間違いがありましたらすみません。
 
　プログラムでもデータでも、間違いを発見されたら教えていただけると大変助かります☆

