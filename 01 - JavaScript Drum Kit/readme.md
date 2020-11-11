# JS 30 - 01 JS Drum Kit

## learning notes

- 利用 `data-key` 讓不同的 DOM 產生關聯
- 將聲音的時間倒帶回 0 ，以達到連續點擊播放的效果 `audio.currentTime = 0`
- 監聽 `transitionend`，在動畫結束時移除 `playing` class

## additional

- 加上 `click` 事件，與 `keydown` 行為相同
- 連續點擊時，class 有時會卡在 active 狀態無法消除，因此加上 `classList.contains` 判斷，若已有 `playing` class 就先移除，避免塞車 🚗
