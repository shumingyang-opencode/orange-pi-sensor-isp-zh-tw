# Orange Pi 感測器影像調適繁中教學站

把 Orange Pi 上的 sensor 影像調適（V4L2 驅動 / sensor bring-up / 影像品質調校）做成**中英對照**的 16 單元分層教學，以 OmniVision OV5640 為主要實例。

- 目標讀者：嵌入式 / 相機 / 影像工程師、學生
- 單元數：16（含 5 個影像調校專章 + 跨平台比較）
- 授權：本站內容 CC-BY-4.0
- 網站：https://shumingyang-opencode.github.io/orange-pi-sensor-isp-zh-tw/

## 單元一覽

| # | 單元 | 內容 |
|---|------|------|
| 01 | 平台相機生態總覽 | SoC 差異、V4L2、CSI 現況 |
| 02 | 影像感測器基礎 | Bayer、快門型態 |
| 03 | 感測器通訊介面 | I2C/SCCB、register |
| 04 | 相機框架與驅動 | V4L2 subdev、ov5640.c |
| 05 | 第一個鏡頭跑起來 | v4l2-ctl 拍照與取流 |
| 06 | Sensor Bring-up 與除錯 | 上電、clock、register dump |
| 07 | ISP 管線深入 | 感測器內 ISP vs 平台 |
| 08 | RAW 擷取與資料格式 | Bayer format、V4L2 格式 |
| 09 | 各平台 ISP 架構差異 | 不同 SoC 的 ISP 有無 |
| 10 | 曝光與自動曝光（AE） | sensor AEC/AGC |
| 11 | 白平衡與色彩（AWB/CCM） | 感測器端白平衡 |
| 12 | 鏡頭陰影校正（LSC） | shading 校正 |
| 13 | 雜訊與降噪 | 後處理 NR |
| 14 | 清晰度/HDR/調校工作流 | 後處理與調校流程 |
| 15 | 四平台影像調校比較 | Orange Pi 視角 |
| 16 | 多感測器與實作案例 | 客製 OV 接入 |

## 開發

純靜態 HTML，無建置步驟。

```sh
python3 -m http.server 8000 -d .
```

## 相關連結

- 學習路徑建議服務：[learning-path-advisor](https://shuming-yang.github.io/learning-path-advisor/) — 依角色推薦教學網站學習路徑
