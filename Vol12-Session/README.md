# Vol12-Session-Numpad

天キーVol.12のセッション用に設計したテンキーケースです。


![Render Default](Images/render-default.PNG)
![Render Default](Images/render-side.PNG)
![Render Default](Images/render-front.PNG)

## プリントリスト
- `Top Unsupported.stl` - ケース上側
  - 下にする面は後ろの斜めの部分です。
    ![Bottom face](Images/bottom-face.png)
  - サポートを以下の面に追加してください。
    ![Support locations](Images/support-locs.png)
    ![Support settings](Images/support-enable.png)
  - 正しく設定した場合、スライス後はこのような見た目になります。
    ![Top sliced - Front](Images/top-sliced-front.png)
    ![Top sliced - Rear](Images/top-sliced-rear.png)
  - 横面の壁が印刷中に歪む場合、ケースを補助ファンの送風方向へ向けたり、歪み防止構造が追加された`Top Supported.stl`を利用したりしてください。
  - ビルドプレートへの定着が不足している場合、ブリムなどを有効化してください。
    ![Brim settings](Images/brim.png)
- `Bottom.stl` - ケース下側
  - ケース上側と同様に、後ろの斜めの面が下になるように印刷してください。
    必要に応じてUSBポート周りにサポートを追加してください。
    ![Bottom supports](Images/bottom-usb-supports.png)
    ![Bottom sliced](Images/bottom-sliced.png)
- `Plate.stl` - プレート

## パーツリスト
- 8 x DIN 562 M3四角ナット
- 8 x M3x8mmネジ
- 4x 8mm径ゴム足

## PCBについて
セッションの内容用にケース側を優先したため、PCBデータは存在しません。  
`Source/`フォルダー内にあるSTEPファイルにPCBの形状データが内蔵されています。  

## 組み立て手順
1. パーツを印刷します。
  ![Print top unsupported](Images/print-top-supported.jpg)
  ![Print bottom](Images/print-bottom.jpg)
1. DIN 562ナットをケース上側のスロットに入れます。
  ![Nut installation](Images/nut-inserting.jpg)
  ![Plier usage](Images/nut-pliers.jpg)
  ![Nuts installed](Images/nut-inserted.jpg)
1. PCBにスタビライザーを搭載し、プレートにスイッチを入れて内部部分を組み立てます。
1. 内部部分（プレート＋スイッチ＋PCB）をケース上側にネジで固定します。
1. ケース上下を組み合わせ、ネジ止めします。