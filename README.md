# OpenCV
Python/電腦辨識/視覺學習小專案
柴犬換色工具 🐕
簡介
這是一個使用 OpenCV 開發的簡易影像處理工具，透過 Trackbar（滑桿）調整 HSV 參數來更改柴犬圖片的顏色，適合用來學習影像處理基礎概念。

功能
載入並縮放圖片

轉換圖片至 HSV 色彩空間

透過 Trackbar 調整色相（Hue）、飽和度（Saturation）、亮度（Value），即時顯示結果

生成遮罩（Mask），篩選特定顏色區域

使用方式
確保已安裝 OpenCV：

複製
pip install opencv-python numpy
執行程式：

複製
python openCV.py
透過 GUI 介面上的 Trackbar 調整 HSV 參數，查看柴犬變色效果。


技術細節
語言：Python

函式庫：OpenCV、NumPy

核心技術：

使用 cv2.cvtColor(img, cv2.COLOR_BGR2HSV) 轉換顏色空間

透過 cv2.createTrackbar 生成可調整的 HSV 參數

cv2.inRange 篩選符合條件的像素，產生遮罩影像

可能改進
增加即時攝影機模式，對動態影像進行變色

增強 GUI 介面，使其更易於使用

支援更多圖片格式及更高效的運算方式
