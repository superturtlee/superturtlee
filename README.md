<div align="center">

# 🐢 Hi, I'm superturtlee

**Android 底层 / 内核 / Root 玩家 · Low-level Android · Kernel · Root Tinkerer**

从引导加载器到 Wayland 桌面，专注于把不可能跑在手机上的东西塞进手机。<br/>
*From the bootloader up to a Wayland desktop — making phones run things they were never meant to.*

<br/>

![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![Linux Kernel](https://img.shields.io/badge/Linux%20Kernel-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![EDK2 / UEFI](https://img.shields.io/badge/EDK2%20UEFI-007396?style=for-the-badge&logo=intel&logoColor=white)
![Magisk](https://img.shields.io/badge/Magisk-00AF9C?style=for-the-badge&logo=magisk&logoColor=white)

</div>

---

## 🔧 What I work on / 我在折腾什么

- 🥾 **Bootloader & UEFI** — Qualcomm ABL 修补、GBL 漏洞利用、Snapdragon 8 Gen 5 / Elite 设备的伪锁引导
- 🧩 **Root frameworks** — Zygisk / ART Hook、Magisk 模块
- 🐧 **Kernel hacking** — GKI 兼容的内核配置裁剪与功能注入（Docker、NTSYNC …）
- 🖥️ **Display & graphics** — 在 Android 上跑 Wayland/Weston，虚拟 DRM 缓冲共享

---

## 📦 Featured Projects / 精选项目

### 🥾 [gbl_root_canoe](https://github.com/superturtlee/gbl_root_canoe)
> 基于 EDK2 的高通 ABL（Android Bootloader）修补工作区。利用 GBL（Generic Bootloader Loader）漏洞注入自定义 EFI，在骁龙 8 Gen 5 / 8 Elite 设备上实现 **伪锁引导（Fake Locked Bootloader）**，绕过解锁检测，并附带 `superfastboot`。
>
> *An EDK2-based workspace for patching Qualcomm ABL via a GBL vulnerability — achieving a Fake Locked Bootloader state on Snapdragon 8 Gen 5 / Elite, with a bundled superfastboot.*
>
> `EDK2` · `UEFI` · `C` · `Magisk Module` · 内嵌反汇编引擎 + 自动补丁器

### 🐳 fulldocker
> 一套内核补丁（`superkernel.diff` + `defconfig_append`），在 **保持 GKI 兼容** 的前提下加入近 100 个配置选项，让 Android 内核完整支持 Docker 容器运行。
>
> *A kernel patch set that enables ~100 config options for full Docker support on Android while keeping GKI compatibility.*
>
> `Linux Kernel` · `Docker` · `GKI` · `defconfig`
>
> > 「这很丑，但是为了加入近 100 个配置选项并保留 GKI 兼容，我不得不如此。」

### 🖥️ anland
> 在 Android 上运行完整 Linux 桌面的显示桥接方案：虚拟 DRM 守护进程 + 生产者/消费者共享缓冲，把 **Wayland / Weston** 合成器画面与触控/键鼠输入桥接到 Android 应用，附带 KWin / XWayland 补丁，以 Magisk 模块形式分发。
>
> *A display-bridge stack that runs a real Linux (Wayland/Weston) desktop on Android via a virtual-DRM daemon and shared producer/consumer buffers, with KWin / XWayland patches.*
>
> `Wayland` · `Weston` · `DRM/GBM` · `JNI` · `Magisk Module`

### 🪝 [Vector](https://github.com/JingMatrix/Vector) (miuix fork)
> 基于 Zygisk 的 ART Hook 框架（与 Xposed API 保持一致），构建于 LSPlant 之上。这里维护的是带 **miuix UI** 的分支。
>
> *A Zygisk-based ART hooking framework with Xposed API compatibility, built on LSPlant — this is the miuix-UI fork.*
>
> `Zygisk` · `ART Hook` · `LSPlant` · `Xposed API`

---

## 📊 GitHub Stats

<div align="center">

![superturtlee's GitHub stats](https://github-readme-stats.vercel.app/api?username=superturtlee&show_icons=true&theme=tokyonight&hide_border=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=superturtlee&layout=compact&theme=tokyonight&hide_border=true&langs_count=8)

</div>

---

## ☕ 赞赏支持 / Buy me a coffee

如果我的项目帮到了你，欢迎请我喝杯咖啡，这是持续折腾的最大动力 🐢<br/>
*If my work helped you, a small tip keeps the turtle hacking.*

<div align="center">

<img src="assets/wechatpay.png" alt="WeChat Pay 微信赞赏码" width="280"/>

**微信支付 · WeChat Pay**

</div>

---

<div align="center">
<sub>⭐ 觉得有用的话，给项目点个 Star 吧 · Star the repos if you find them useful</sub>
</div>
