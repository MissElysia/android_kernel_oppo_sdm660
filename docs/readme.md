<img align='left' src='cyrene.png' width='180px' alt="logo">

*记忆的涟漪，等待被流星的亲吻唤醒——要用「爱」铭记我，在那美丽的明天。*

# OPPO R11/s 系列内核源码
*本仓库是[Elysia的仓库](https://github.com/MissElysia/android_kernel_oppo_sdm660)的下游，使用时出现问题请不要反馈至上游issue*

---
## 🔧 内核文件概览
- 基于 Android Pie 的 CAF（Code Aurora Forum）代码
- 内核主线版本：Linux 4.4.y
- 硬件驱动来源：[Qualcomm](https://git.codelinaro.org/clo/la/kernel/msm-4.4) 与 [OPPO](https://github.com/oppo-source).
- 设备架构：arm64-v8

## 🔧 改动如下
  - 使用 SukiSU-Ultra（无SusFs） 作为默认 Root 支持。
  - 合并 5.4 的 netbpf 与 BinderFS。
  - 加入 EAS 调度。
  - 使用 Capacity Aware Superset Scheduler + utilization clamping（利用率钳制）用于实时（RT）/公平（FAIR）任务。
  - 支持 KPM（Kernel Patching Module）。
  - 使用 Simple Android Low Memory Killer（简易 Android 低内存杀手）。
  - 使用 Cgroup v2 与 freeze v2。
  - 添加额外的 I/O 调度器与 Boeffla WakeLock Blocker。
  - 开启 pstore 支持。
  - 添加 EROFS 文件系统。
  - 添加 SBalance IRQ 负载均衡器。
  - 添加 effective affinity mask（有效亲和性掩码）。
  - 启用 TCP 与 “TTL” target 支持。

---

## ⚠️ **设备要求**
1. 设备为Oppo R11 （16051）
2. 系统为**Android 11+**
3. 刷入前先安装SukiSU-Ultra管理器并确保无任何其他root管理器的su残留

---

## ⚠️ **刷入步骤**
1. 下载[release](https://github.com/kelsuita/android_kernel_oppo_sdm660/releases)中的anykernel3与no-verity-force-encrypt.zip
2. 用twrp刷入anykernel3
3. 再用twrp刷入no-verity-force-encrypt.zip
4. 开机，enjoy！


---

## 🌟 支持者，感谢！
- [Kelsuita](https://github.com/kelsuita)
- [愛莉希雅](https://github.com/mihoy3rd)
- [WenHao](https://github.com/WenHao2130)
- [WenHao-dev](https://github.com/WenHao-dev)
- [CY](https://github.com/ltdq)
- [Color](https://github.com/color597)
- [oppo-source](https://github.com/oppo-source)
- [Qualcomm](https://git.codelinaro.org/clo/la/kernel/qcom)

