# Antigravity 提示音 - 基本鈴聲 (WSL)

在 Antigravity 提問或停止時，自動播放提示音通知用戶。

## 前置需求

在 WSL 中使用此插件前，請先安裝 PulseAudio 工具：

```bash
sudo apt install pulseaudio-utils
```

## 功能特色

- 💬 **PreToolUse (`ask_question`) 事件**: 當 Antigravity 主動提問需要你回覆時播放提示音
- 🛑 **Stop 事件**: 當 Antigravity 停止執行時播放提示音

## 安裝插件

在 Antigravity CLI 中安裝插件：

```bash
agy plugin install https://github.com/ycs77/agy-notifications/tree/main/plugins/basic-wsl
```

## 使用說明

安裝插件後，它會自動運作，無需額外設定。

## Hook 觸發時機

### PreToolUse (`ask_question`) Hook

- 當 Antigravity 呼叫 `ask_question` 工具向用戶提問時觸發
- 用於提醒用戶有問題需要回覆

### Stop Hook

- 當 Antigravity 主代理準備停止執行時觸發
- 用於通知用戶任務已完成

## 作者

Lucas Yang (yangchenshin77@gmail.com)

## 授權

MIT License
