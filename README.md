# PM2.5-forecasting-based-on-attention-based-LSTM-neural-network 基於混合式長短期記憶網路架構之PM2.5預測
## College Student Research Scholarship, NSC 國科會大專生科技部計畫

### 計畫摘要
隨著近年來國人健康意識抬頭，空氣汙染已經成為眾人關注的議題。除了氣象預報以外，空氣品質指標（AQI）也成為日常生活中不可或缺的項目，其中考量多種空氣汙染因子，如：細懸浮微粒(PM2.5)、一氧化碳(CO)等。其中「細懸浮微粒(PM2.5)」對人體的影響尤為嚴重。空氣汙染濃度可能受周遭地區降雨、風向、風速等影響，若能將氣象因子加入模型中，預期能提高預測的準確度。本計畫使用我國行政院環保署所提供之空氣品質歷年監測資料作為訓練集與測試集，共分為兩階段。第一階段使用長短期記憶模型（LSTM）與注意力機制（attention mechanism），分別考慮風向與降雨量的空間變化對鄰近地區 PM2.5濃度的影響，通過 LSTM 神經網路得到PM2.5濃度預測結果。第二階段將前述模型結合，透過注意力機制同時考慮風向與降雨量的影響，計算兩者對PM2.5濃度變化的權重，得出最終PM2.5濃度預測結果。本計畫考慮不同時間長度的歷史資料預測未來不同時間長度的PM2.5濃度的結果，最終製作的風雨長短期記憶模型（Wind-and-Rainfall sensitive LSTM, WRLSTM）能有效預測未來6-18小時的PM2.5濃度，且結果優於其他常見演算法，如：MLP regression等。

### 模型架構
![image](https://github.com/WillHBX/PM2.5-forecasting-based-on-attention-based-LSTM-neural-network/blob/main/architecture.png?raw=true)

### 模型比較
![image](https://github.com/WillHBX/PM2.5-forecasting-based-on-attention-based-LSTM-neural-network/blob/main/Comparison%20(2).png?raw=true)
