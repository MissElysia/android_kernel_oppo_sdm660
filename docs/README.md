<img align='left' src='ElysiaMei.jpg' width='180px' alt="logo">

# OPPO R11/s 系列核心源碼

**粵語**

驍龍660嘅oppo核心源碼倉庫, 裝置驅動來自 [`oppo-source`](https://github.com/oppo-source), 並進行了一些小改動.

[![Latest release](https://img.shields.io/github/v/release/MissElysia/android_kernel_oppo_sdm660?label=Release&logo=github)](https://github.com/MissElysia/android_kernel_oppo_sdm660/releases/latest)
[![License: GPL v2](https://img.shields.io/badge/License-GPL%20v2-orange.svg?logo=gnu)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)
[![GitHub License](https://img.shields.io/github/license/tiann/KernelSU?logo=gnu)](/LICENSE)

[Linux原文檔](./Linux/README)
[倉庫注意事項](./security/SECURITY.md)

[安裝引導](./guide/install.md)

## 第三方支援

1. 使用 ReSukiSU/SukiSU Ultra/Rissu 作為默認 Root 支援.
2. 合併 5.4 嘅 netbpf 與 BinderFS.
3. 加入eas 調度.
4. 使用 Capacity Aware Superset Scheduler+utilization clamping for RT/FAIR task.
5. KPM 支援.
6. 使用 Simple Android Low Memory Killer.
7. 使用 Cgroup v2 與 freeze v2.
8. 添加額外嘅 I/O 調度器 與 boeffla wakelock bl Ocker.
9. 開啟 pstore 支援.
10. 添加 erofs 文件系統.
11. 添加 SBalance IRQ balancer.
12. 添加 effective affinity mask.
13. 啟用 TCP 與 "TTL" target support.

## 核心支援情況

- 基於 Android Pie 嘅 CAF.

- 核心主線： Linux-4.4.y.

- 硬件驅動供應： [Qualcomm](https://git.codelinaro.org/clo/la/kernel/msm-4.4) 與 [OPPO](https://github.com/oppo-source).

- 裝置架構： arm64-v8.

## 內核支援者

- [愛莉希雅](https://github.com/mihoy3rd)
- [WenHao](https://github.com/WenHao2130)
- [WenHao-dev](https://github.com/WenHao-dev)
- [CY](https://github.com/ltdq)
- [Color](https://github.com/color597)
- [oppo-source](https://github.com/oppo-source)
- [Qualcomm](https://git.codelinaro.org/clo/la/kernel/qcom)