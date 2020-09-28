# mosaic_picture
画像を輝度情報に合わせてグリッド表示するプログラム
# usage
該当ファイルをGoogle Colabに入れた後，　Pathを自身の環境に合わせてください

パラメータ調整は以下


- 分割量の調整
```
# 入力画像の情報
motogazo = './src/pearl.png'
x_bunkatsu = 13*10*2
y_bunkatsu = 11*10*2

# 出力画像の情報
result_filename = './result/mozaiku.png'
x_size_result = 1430*4
y_size_result = 1210*4
```
- 文字の大きさ調整
```
def number_maker(element, count):
  ttfontname = "./font/Helvetica.ttc"
  fontsize = 100
  text = str(element[0])

  # 画像サイズ，背景色，フォントの色を設定
  canvasSize    = (200, 200)
  RGB = (element[1],element[2],element[3])
  alpha = 0.1
  backgroundRGB = (int(element[1]*alpha),int(element[2]*alpha),int(element[3]*alpha))
```
# 参考
文字列を画像に変換する
(https://qiita.com/implicit_none/items/a9bf7eebe125c9d773eb)

【Python】モザイクアートを作成する
(https://tanakatarou.tech/308/)
