# Pomelo · 柚電

**Every watt, clearly.** A free native macOS app for battery status, power flow, memory pressure and peripheral batteries.

[English website](https://pomelo-mac.silverlime68.chatgpt.site/en/) · [繁體中文網站](https://pomelo-mac.silverlime68.chatgpt.site/) · [Download 0.12.2](https://github.com/brian120494/pomelo-macos/releases/tag/v0.12.2) · [Optional support on Ko-fi](https://ko-fi.com/brian1204)

![Pomelo menu panel with demonstration values](https://pomelo-mac.silverlime68.chatgpt.site/assets/menu-en.png)

## Public beta: 0.12.2

This update fixes duplicate AirPods records and keeps menu-bar display/icon controls open during live sensor updates. Older English/Chinese left/right/case records are merged while retaining hidden selections and observation times. Hardware addresses are used when available; different devices with known different addresses remain separate. Polling rates are unchanged.

The app supports English and Traditional Chinese. Choose **Settings → General → Language**, then restart Pomelo. Existing activity logs keep their original language.

Download **Pomelo-macOS-0.12.2.zip** from the [0.12.2 release](https://github.com/brian120494/pomelo-macos/releases/tag/v0.12.2), with **SHA256SUMS.txt** for verification. GitHub's automatically generated “Source code” archives contain this distribution repository's documentation, not the application.

- Apple silicon MacBook; macOS 26.4 or later recommended.
- Ad-hoc signed; **not Developer ID signed or notarized by Apple**. macOS may block it. Disabling system security is not required.
- Free to use with optional tips; all users get the same features.
- This repository hosts downloads and issue tracking. It does not publish application source or grant an open-source license.

## Updating the optional system-process reader

Quit the older app before replacing it; keep your existing preferences and data. For protected processes such as WindowServer, install **PomeloSystemReader.pkg from the same 0.12.2 archive**, authorize it in the macOS installer, then reconnect in Energy Insights. The reader verifies the exact app signature and signed-in user; an older installer authorizes a different build.

Everyday battery, peripheral and whole-Mac memory readings do not need this helper. **RemovePomeloSystemReader.pkg** is only for uninstalling it, not updating it. Version 0.12.2 includes the 0.12.1 authorization and installer-selection fixes.

## What it does

- Visual power flow between the charger, Mac, battery and reported peripherals, with optional gentle animation.
- Menu-bar watts, memory usage, pressure colors and peripheral battery cards.
- Battery health, temperature when available, history and CSV export.
- App CPU energy and memory rankings, with unavailable readings marked clearly.
- Configurable refresh intervals and energy-saving behavior.
- Charge limits through Apple Shortcuts. Charge fully once, then restore 80%; optionally trigger at home using Wi-Fi or a daily schedule.
- Local settings and history, with no app accounts, analytics trackers or cloud sync.

Charge control needs initial shortcut setup. See the [installation and charging guide](https://pomelo-mac.silverlime68.chatgpt.site/en/guide.html).

## Validation and limitations

The release build, installer/app signature matching and **166 automated checks** passed, including 7 accessory identity/cache regressions and 3 native menu integration checks. Physical AirPods reconnect and cross-model compatibility still need confirmation.

iPhone/iPad USB and Wi-Fi require trust pairing. Wireless battery readings, direct Bluetooth and overnight reconnection remain under validation. App energy readings cover available **CPU energy**, not complete GPU/display/shared-service power. Sensors can update at different times; estimates and missing data are labeled. Name-only accessory observations cannot reliably distinguish identical device names.

## Feedback and support

[Open an issue](https://github.com/brian120494/pomelo-macos/issues) or email **a2006941204@gmail.com** with the app version, macOS version, Mac model and reproduction steps. Remove device identifiers before sharing diagnostics.

[Privacy notice](https://pomelo-mac.silverlime68.chatgpt.site/en/privacy.html) · [Release notes](https://pomelo-mac.silverlime68.chatgpt.site/en/release-notes.html)

---

柚電是一款免費的 Mac 電池、電力流向、記憶體與周邊電量工具。**0.12.2** 修正 AirPods 中英文重複紀錄，以及數據更新時選單列圖案設定被關閉的問題，保留原本設定與讀值時間。

先結束舊版，再替換 App。若要讀取 WindowServer 等受保護程序，請安裝 **0.12.2 同包隨附的 PomeloSystemReader.pkg**，完成管理員驗證後回到耗電探索連線；不要沿用舊版安裝包。移除套件不是更新步驟。

支援繁體中文與 English，166 項自動檢查通過。仍是未經 Apple 正式簽署與公證的 Apple 晶片測試版，建議 macOS 26.4 以上；手機無線電量、實體 AirPods 重連與跨機型相容性仍待確認。請閱讀[中文使用說明](https://pomelo-mac.silverlime68.chatgpt.site/guide.html)。免費下載，自由贊助，沒有付費功能牆。

Independently made. Not affiliated with Apple or Juicy.
