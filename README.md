# Arduino LED 互動裝置

一個基於 Arduino 的 LED 互動裝置，具有多種燈光效果和聲音回饋。

## 小組成員
- 曾玟心
- 楊欣芸

## 硬體需求
- Arduino Uno R3
- LED × 6
- 220Ω 電阻 × 6（LED用）
- 按鈕 × 1
- 蜂鳴器 × 1
- 麵包板
- 跳線若干

## 接線說明
1. LED接線：
   - LED1 → PIN 2（需要 220Ω 電阻）
   - LED2 → PIN 3（需要 220Ω 電阻）
   - LED3 → PIN 4（需要 220Ω 電阻）
   - LED4 → PIN 5（需要 220Ω 電阻）
   - LED5 → PIN 8（需要 220Ω 電阻）
   - LED6 → PIN 9（需要 220Ω 電阻）

2. 按鈕接線：
   - 輸入腳 → PIN 7
   - 觸發腳 → GND

3. 蜂鳴器接線：
   - 正極 → PIN 6
   - 負極 → GND

## 功能說明
裝置共有7種模式，通過按鈕切換：

1. **依序點亮模式**
   - LED 從左到右依序亮起
   - 每個 LED 配有不同音高

2. **來回掃描模式**
   - LED 左右來回移動
   - 配有移動音效

3. **全部閃爍模式**
   - 所有 LED 同時閃爍
   - 配有同步音效

4. **交替閃爍模式**
   - 奇偶 LED 交替閃爍
   - 配有交替音效

5. **隨機閃爍模式**
   - 隨機點亮某個 LED
   - 音高隨 LED 位置變化

6. **快速來回模式**
   - LED 快速正序點亮後倒序關閉
   - 配有漸進音效

7. **全部關閉模式**
   - 關閉所有 LED

## 使用方法
1. 按照接線說明完成硬體連接
2. 上傳程式碼到 Arduino
3. 通過按鈕切換不同模式
4. 每個模式都有對應的燈光效果和聲音

## 程式碼
完整程式碼請見 [LED_Interactive.ino](LED_Interactive.ino)

## 注意事項
1. 確保 LED 正負極接線正確
2. 每個 LED 都需要使用 220Ω 電阻
3. 按鈕接線時注意輸入腳和觸發腳的位置
4. 蜂鳴器注意正負極方向

## 授權
MIT License

## 更新日誌
- 2024/03/22：初始版本
