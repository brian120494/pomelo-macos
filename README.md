# Pomelo · 柚電

**Every watt, clearly.** A free native macOS app for battery status, power flow, memory pressure and peripheral batteries.

[English website](https://pomelo-mac.silverlime68.chatgpt.site/en/) · [繁體中文網站](https://pomelo-mac.silverlime68.chatgpt.site/) · [Downloads](https://github.com/brian120494/pomelo-macos/releases) · [Optional support on Ko-fi](https://ko-fi.com/brian1204)

![Pomelo menu panel with demonstration values](https://pomelo-mac.silverlime68.chatgpt.site/assets/menu-en.png)

## Public beta

**0.12.0** supports English and Traditional Chinese. Choose **Settings → General → Language**, then restart Pomelo. Select System to follow your preferred language. Existing activity logs keep their original language.

Download the **Pomelo-0.12.0-beta.zip** asset from Releases and verify it against **SHA256SUMS.txt** if desired. GitHub's automatically generated “Source code” archives contain this distribution repository's documentation, not the app or its implementation.

- Apple silicon MacBook; macOS 26.4 or later recommended.
- The beta is ad-hoc signed, **not Developer ID signed or notarized by Apple**. macOS may block it. A formally signed release is still pending; disabling system security is not required.
- Free to use, with optional tips. All users get the same features.
- This repository hosts downloads and issue tracking. It does not publish the application source or grant an open-source license.

## What it does

- Visual power flow between the charger, Mac, battery and reported peripherals, with optional gentle animation.
- Menu bar watts, memory usage, pressure colors and peripheral battery cards.
- Battery health, temperature when available, history and CSV export.
- App CPU energy and memory rankings, with unavailable readings marked clearly.
- Configurable refresh intervals and energy-saving behavior.
- Charge limits through Apple Shortcuts. Charge fully once, then restore 80%; optionally trigger at home using Wi-Fi or a daily schedule.
- Local settings and history, with no app accounts, analytics trackers or cloud sync.

Charge control needs initial shortcut setup. See the [installation and charging guide](https://pomelo-mac.silverlime68.chatgpt.site/en/guide.html).

## Current limitations

iPhone/iPad USB and Wi-Fi access requires trust pairing. Wireless battery readings, direct Bluetooth and overnight reconnection are still being validated and are not guaranteed on every device. App energy readings cover available **CPU energy**, not total GPU/display/shared-service power. Sensors may update at different times; estimates and missing data are labeled. Protected processes such as WindowServer may be unreadable. The public package excludes the administrator helper installer still awaiting validation.

The release build and 149 core, native, animation and localization checks passed. These checks do not replace physical testing across Mac and phone models.

## Feedback and support

[Open an issue](https://github.com/brian120494/pomelo-macos/issues) or email **a2006941204@gmail.com** with the app version, macOS version, Mac model and steps to reproduce. Remove device identifiers before sharing diagnostics.

[Privacy notice](https://pomelo-mac.silverlime68.chatgpt.site/en/privacy.html) · [Release notes](https://pomelo-mac.silverlime68.chatgpt.site/en/release-notes.html)

---

柚電是一款免費的 Mac 電池、電力流向、記憶體與周邊電量工具。0.12.0 新增英文介面；在「偏好設定 → 一般 → 語言」選擇跟隨系統、繁體中文或 English，重新開啟後套用。

目前提供 Apple 晶片 MacBook 測試版，建議 macOS 26.4 以上，尚未經 Apple 正式簽署與公證。手機無線電量、隔夜重連與部分系統程序讀取仍有限制。請先閱讀[中文使用說明](https://pomelo-mac.silverlime68.chatgpt.site/guide.html)。免費下載，自由贊助，沒有付費功能牆。

Independently made. Not affiliated with Apple or Juicy.
