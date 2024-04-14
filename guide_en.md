# Building Guide

## Firmware

> **Note**
>
> The firmware programming method of RP2040 series is more or less the same, no matter whether it is the version of MCU with Reset and Bootloader dual buttons or not, all of them have the same programming method.

- Press and hold the Bootloader button and then connect to the computer, the local computer will show you the location of the hard drive where the firmware is burned.
![guide](pic/guide0.jpg)

- Then move the .uf2 firmware file to the hard drive to finish flashing.
![guide](pic/guide1.png)

## PCB and MCU

- 首先將燒錄好韌體的2片主控板跟左右手電路板準備好。
![](pic/1-01.jpg)

- 接著剪下一段紙膠帶，對好位置把主控板用膠帶先固定好。
![](pic/1-02.jpg)

- 先將其中一排焊盤先用焊錫固定好，再將膠帶撕掉。
![](pic/1-03.jpg)

- 最後再用焊錫把其他位置的焊盤都焊上。
![](pic/1-04.jpg)

## SMD Parts

- 1N4148二極體的安裝方式請參照圖片所示。
![](pic/2-01.png)

- 接著將52個二極體用焊錫焊接好。
![](pic/2-02.jpg)

- 下圖是SK6812Mini-E的安裝方式，如果沒有要安裝LED燈的話，請跳過這個步驟。
![](pic/2-03.png)

- 貼片LED燈務必留意電烙鐵不要在焊盤上停留過久的時間，LED燈有機率會被燒壞。
![](pic/2-04.jpg)

- LED固定好之後可以先接上電腦測試，鍵盤預設燈亮。
![](pic/2-05.jpg)

- 二極體、LED燈都完成之後最後再將熱插拔座固定在電路板上。
![](pic/2-06.jpg)

## Encoder and Jack

> **Warning**
>
> 現階段版本問題的原因，這裡的做法會跟照片有所出入，請務必留意文字說明。

- 將滑鼠滾輪、滑鼠微動、滑鼠編碼器、旋鈕編碼器、TRRS座及Joy-con搖桿準備好，並依序將它們固定在電路板上。
![](pic/3-01.jpg)

- 第一步先將滑鼠編碼器焊接固定好之後，再把滑鼠滾輪固定在六角輪上。
![](pic/3-02.jpg)

- 接著再將滑鼠微動卡在定位點焊接固定好。
![](pic/3-03.jpg)

> **Note**
>
> 如果不先這麼做的話，滑鼠滾輪會無法正常安裝到編碼器上，務必留意。

- 接著再將旋鈕、TRRS座、Joy-con搖桿也都焊接起來。
![](pic/3-04.jpg)

- 然後就可以測試鍵盤左右側通電的狀況，務必在這個時候就進行LED燈測試及左右鍵盤按鍵的訊號狀況。（照片為示意圖，沒有完成整體的安裝）
![](pic/3-05.jpg)

## Keyboard Building

- 接著將15mm的銅柱、3mm的螺絲準備好，先來安裝固定滑鼠滾輪的銅柱。
![](pic/4-01.jpg)

- 從左右手的電路板背面將銅柱固定上去。 
![](pic/4-02.jpg)

- 接著準備8mm螺絲、M2螺帽及M2螺絲墊片，將它們依序固定在左右側的鍵盤底板上。
![](pic/4-03.jpg)

- 左右側按照照片示意固定8mm的螺絲。
![](pic/4-04.jpg)

- 對好電路板上的螺絲孔，將電路板放在底板上。
![](pic/4-05.jpg)

- 接著準備6mm、7mm銅柱。
![](pic/4-06.jpg)

- 6mm銅柱安裝在Joy-con搖桿的位置、7mm銅柱安裝在旋鈕編碼器及主控板的位置。
![](pic/4-07.jpg)

- 接著準備定位板、4mm銅柱及3mm螺絲。
![](pic/4-08.jpg)

- 把它們固定在定位板上的螺絲孔上。
![](pic/4-09.jpg)

- 接著把定位板跟底板組合在一起。
![](pic/4-10.jpg)

- 使用3mm螺絲從底板後面把定位板固定起來。
![](pic/4-11.jpg)

- 最後一步將所有的擋板固定到鍵盤上。
![](pic/4-12.jpg)

- 完成之後把鍵盤翻到背面，把自黏腳貼貼上去。
![](pic/4-13.jpg)

- 大致像下圖這樣貼即可，需要受較大力的地方多貼一些比較穩固。
![](pic/4-14.jpg)

- 將兩隻手的部分完工就結束了。
![](pic/4-15.jpg)

- 上軸。
![](pic/4-16.jpg)

- 上鍵帽，測試燈光效果
![](pic/4-17.jpg)

## Troubleshooting

- LED燈預設是開著燈，如果LED燈沒有焊接固定完整，燈效會跑掉，嚴重時電腦會無法辨識鍵盤，這時設法將燈光關閉可以直接排除這個問題，屆時再將LED焊接固定好即可。
- 如果單顆按鍵沒有觸發，請依序檢查：熱插拔座、二極體、鍵軸。
- 如果單排按鍵沒有觸發，請檢查看看是不是主控座沒有焊接好。
- 旋鈕及搖桿本身自帶按鍵，不要忘記測試。
- 編碼器的測試方式即測試預設的功能：音量大小、滾輪上下滾動。

希望這個能夠幫助大家解決任何在安裝上的困難，謝謝大家。











