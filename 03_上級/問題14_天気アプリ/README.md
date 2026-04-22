# 上級 問題14: 天気アプリ（API連携）

**難易度: ★★★★★★★★★☆**

## 🎯 やること

**Open-Meteo 無料 API** を使って、都市名から天気予報を取得する簡単な天気アプリを作ります。

## ✅ 要件

1. 都市名の入力欄と「取得」ボタン
2. 都市名 → **ジオコーディング API** で緯度経度を取得
   - `https://geocoding-api.open-meteo.com/v1/search?name=Tokyo&count=1&language=ja`
3. 緯度経度 → **天気 API** で現在の気温・天気を取得
   - `https://api.open-meteo.com/v1/forecast?latitude=XX&longitude=YY&current=temperature_2m,weather_code,wind_speed_10m&timezone=auto`
4. 取得した「気温」「風速」「天気コード」を表示
5. 天気コードに応じて**絵文字**を表示（0: ☀️, 1-3: 🌤, 45-48: 🌫, 51-67: 🌧, 71-77: 🌨, 80-82: 🌦, 95-99: ⛈）
6. エラーハンドリング（都市が見つからない／ネットワークエラー）

## 💡 ヒント

無料・認証不要の API なので気軽に使えます。
