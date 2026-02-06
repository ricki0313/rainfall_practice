# day2 12 月累積雨量網格資料製作
## 目標
參考氣象署雨量網格化資料生產履歷，產出全台 12 月月雨量網格資料

## 資料確認
準備測站雨量資料，需包含測站經度、緯度、時間與雨量值。

## 月累積雨量
以測站為單位，將同測站逐時雨量加總。
產出欄位包含 stno、lon、lat、rain_dec

## 建立全台固定網格系統
- 設定網格空間範圍：
    - 左下角經緯度為 (117.43, 20.76)
    - 右上角經緯度為 (123.92, 26.70)
- 設定網格解析度：
    - 2.5 公里解析度，網格大小為 260 × 260

## 月雨量 simple Kriging
- Variogram model (資料隨距離變化之空間相關性)
    - sill: the population variance (資料變異量上限)
    - range: the distance with less correlation (空間相關性幾乎消失的距離，超過此range可視為獨立)
    - nugget: uncertainly as distance is zero (距離趨於0時仍存在的不確定性)

- Simple Kriging




