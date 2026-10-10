# C3 Miner

C3Pool 官方桌面挖矿工具：填入收款地址和矿工名称，一键开始 CPU / 显卡挖矿。挖矿程序（xmrig-C3）自动下载并校验，在后台运行，显示算力、日志、硬件信息和矿池收益。

C3Pool's official desktop miner. Enter your payout address and a worker name, then start CPU or GPU mining with one click. The mining program (xmrig-C3) is downloaded and verified automatically, runs in the background, and the app shows hashrate, logs, hardware info and pool earnings.

## 下载 / Download

| 版本 Version | 系统 System | 下载 Download | SHA-256 |
|---|---|---|---|
| **1.2.0**（最新 / latest） | Windows 10 / 11（64 位 / 64-bit） | [GitHub](https://github.com/C3Pool/c3-miner-releases/releases/download/v1.2.0/C3Miner-1.2.0-setup.exe) · [亚洲镜像 Asia mirror](https://download.c3pool.org/c3-miner-releases/C3Miner-1.2.0-setup.exe) | `d8fc18a0227b82be4174c13ce001328f515cf24825bc3107189dc3ab8eba19e3` |
| 1.1.0 | Windows 10 / 11（64 位 / 64-bit） | [GitHub](https://github.com/C3Pool/c3-miner-releases/releases/download/v1.1.0/C3Miner-1.1.0-setup.exe) · [亚洲镜像 Asia mirror](https://download.c3pool.org/c3-miner-releases/C3Miner-1.1.0-setup.exe) | `19cbe61bb16e3e0ec8ff067e40b0ffe782aa0ea79232203db94b0c12210f9d4d` |
| 1.0.3 | Windows 10 / 11（64 位 / 64-bit） | [GitHub](https://github.com/C3Pool/c3-miner-releases/releases/download/v1.0.3/C3Miner-1.0.3-setup.exe) · [亚洲镜像 Asia mirror](https://download.c3pool.org/c3-miner-releases/C3Miner-1.0.3-setup.exe) | `3ab519a5ad5da52990844d1a793ad9090d0344139a58208f8a78902e566f5083` |
| 1.0.2 | Windows 10 / 11（64 位 / 64-bit） | [GitHub](https://github.com/C3Pool/c3-miner-releases/releases/download/v1.0.2/C3Miner-1.0.2-setup.exe) · [亚洲镜像 Asia mirror](https://download.c3pool.org/c3-miner-releases/C3Miner-1.0.2-setup.exe) | `bfd69a40f97acee4d4e2a8b521085295ff46a6057b05e0216c5a0af0cdff013f` |
| 1.0.1 | Windows 10 / 11（64 位 / 64-bit） | [GitHub](https://github.com/C3Pool/c3-miner-releases/releases/download/v1.0.1/C3Miner-1.0.1-setup.exe) · [亚洲镜像 Asia mirror](https://download.c3pool.org/c3-miner-releases/C3Miner-1.0.1-setup.exe) | `f767f65f8b4b40d16e4a1cdcf16dec5cd862aeb71463c7f839910e0db528528e` |
| 1.0.0 | Windows 10 / 11（64 位 / 64-bit） | [GitHub](https://github.com/C3Pool/c3-miner-releases/releases/download/v1.0.0/C3Miner-1.0.0-setup.exe) · [亚洲镜像 Asia mirror](https://download.c3pool.org/c3-miner-releases/C3Miner-1.0.0-setup.exe) | `01adea168494ca113e52a0513d4282501a508c61db1ca60a01ef89df6eddf00c` |

中国大陆及亚洲用户建议使用亚洲镜像，两个链接的文件完全相同。Users in Asia should use the Asia mirror; both links serve the same file.

所有版本与更新说明见 [Releases](https://github.com/C3Pool/c3-miner-releases/releases)。All versions and release notes: [Releases](https://github.com/C3Pool/c3-miner-releases/releases).

所有版本的校验值见 [SHA256SUMS](SHA256SUMS)。Checksums for all versions are in [SHA256SUMS](SHA256SUMS).

## 安装说明

1. **浏览器提示「通常不会下载 C3Miner-…-setup.exe」**（Edge）：在下载列表中右键该文件 →「保留」→ 展开「删除」旁的箭头 →「仍然保留」。
2. **Windows 提示「Windows 已保护你的电脑」**：安装包暂未做代码签名，点「更多信息」→「仍要运行」即可。
3. **需要管理员权限**：启动时会弹出一次权限确认。挖矿程序需要它来开启大页内存和 MSR 优化，否则算力明显偏低。
4. **把以下两个目录加入杀毒软件白名单（信任区 / 排除项）**：挖矿程序常被杀毒软件（如 360、火绒、电脑管家、Microsoft Defender）误报并删除。
   - `C:\Program Files\C3 Miner`
   - `%LOCALAPPDATA%\com.c3pool.miner\miners`
5. 首次开始挖矿时，挖矿程序会先测试各算法性能，约 3 分钟，之后自动开始挖矿。
6. 首次启用大页内存后需要**重启一次电脑**，算力可提升约 50%。

支持的收款地址：XMR、USDT-TRC20、USDT-BEP20 / Polygon（0x 地址，需选择结算链）、USDT-SPL（Solana）。

在「设置」里可以设置 CPU 占用上限、使用电脑时暂停挖矿（空闲后自动恢复）、使用电池时暂停挖矿，以及开机自动启动。

卸载：Windows「设置 → 应用」中卸载 C3 Miner。卸载会同时删除开机启动任务；收款地址等设置会保留，重新安装后继续使用。

## Installation notes

1. **The browser says the installer "isn't commonly downloaded"** (Edge): right-click it in the downloads list → "Keep" → open the arrow next to "Delete" → "Keep anyway".
2. **"Windows protected your PC"**: the installer is not code-signed yet. Click "More info" → "Run anyway".
3. **Administrator rights**: you confirm once at start. The miner needs them for huge pages and MSR tuning; without them the hashrate is much lower.
4. **Add these two folders to your antivirus allow list (exclusions)**. Antivirus software (including Microsoft Defender) often flags and deletes mining programs by mistake.
   - `C:\Program Files\C3 Miner`
   - `%LOCALAPPDATA%\com.c3pool.miner\miners`
5. On the first start the miner measures algorithm performance for about 3 minutes, then starts mining automatically.
6. After huge pages are enabled for the first time, **restart the computer once** for about 50% more hashrate.

Supported payout addresses: XMR, USDT-TRC20, USDT-BEP20 / Polygon (0x address, choose a settlement chain), USDT-SPL (Solana).

Settings include a CPU usage limit, pausing while you use the computer (resumes when idle), pausing on battery, and starting at sign-in.

To uninstall, remove C3 Miner in Windows Settings → Apps. The sign-in task is removed too; your payout address and settings are kept for a reinstall.

## 更新记录 / Changelog

### 1.2.0

- 全新窗口：去掉 Windows 原生边框，右上角为最小化 / 精简窗口 / 关闭三个按钮，窗口固定尺寸。
- 精简窗口：一个圆形小窗，显示当前算力、平均算力和是否在挖矿。
- 悬浮球（在设置中开启）：始终置顶的小圆球，轮播实时算力 / 平均算力 / 今日收益（右键选择显示内容）；单击打开主窗口，可拖到任意位置并记住位置。
- 在线更新：「关于」页可检查更新，一键自动下载、校验并安装新版本，装好后自动继续挖矿。
- 仪表盘显示显卡矿工的矿池侧算力。
- New window: no native Windows frame; minimize / compact / close buttons at the top right; fixed window size.
- Compact window: a small round view with current and average hashrate and whether mining is running.
- Floating orb (turn it on in Settings): a small always-on-top circle cycling through hashrate / average / today's earnings (right-click to choose); click it to open the main window; drag it anywhere and it stays there.
- Online update: check for updates on the About page; one click downloads, verifies and installs the new version, then mining carries on.
- The dashboard shows the GPU worker's hashrate as seen by the pool.

### 1.1.0

- 新增显卡挖矿与混合挖矿（CPU + 显卡同时挖）。支持 ETC、ERG、RVN、PRL、QTC、cn/gpu、XTM-C 等显卡币种，可自动挑选收益最高的币，也可手动指定；挖矿程序（SRBMiner-Multi / BzMiner / PeakMiner）自动下载。
- Adds GPU mining and hybrid mining (CPU and GPU at the same time). Supports ETC, ERG, RVN, PRL, QTC, cn/gpu and XTM-C; auto-selects the most profitable coin or mines one you choose, and downloads the mining programs (SRBMiner-Multi / BzMiner / PeakMiner) for you.

### 1.0.3

- 可以安装在未预装 WebView2 的系统上（如 Windows Server、部分 Windows 10 版本）：安装包自带 WebView2 引导程序。
- 挖矿程序管理与下载机制重构，稳定性改进。
- Installs on systems without WebView2 (Windows Server, some Windows 10 editions): the installer now carries the WebView2 bootstrapper.
- Reworked miner management and downloads; stability improvements.

### 1.0.2

- 升级更顺畅：覆盖安装新版本时不再弹出旧版卸载窗口，也不再询问是否关闭正在运行的 C3 Miner，设置和开机启动全部保留。
- Smoother upgrades: installing a new version no longer opens the old uninstaller or asks to close the running C3 Miner; settings and start-at-sign-in are kept.

### 1.0.1

- 「关于」页加入软件介绍、官网（c3pool.com / c3pool.org）与社区链接（X、Telegram、Discord、GitHub、邮箱）。
- 挖矿模式新增「混合挖矿」（CPU 与显卡同时挖矿），与显卡挖矿一起即将推出。
- About page: introduction, websites (c3pool.com / c3pool.org) and community links (X, Telegram, Discord, GitHub, email).
- New "Hybrid mining" mode (CPU and GPU together), coming soon together with GPU mining.

### 1.0.0

首个正式版。First public release.
