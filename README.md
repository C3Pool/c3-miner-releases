# C3 Miner

C3Pool 官方桌面挖矿工具：填入收款地址和矿工名称，一键开始 CPU / 显卡挖矿。挖矿程序（xmrig-C3）自动下载并校验，在后台运行，显示算力、日志、硬件信息和矿池收益。

C3Pool's official desktop miner. Enter your payout address and a worker name, then start CPU or GPU mining with one click. The mining program (xmrig-C3) is downloaded and verified automatically, runs in the background, and the app shows hashrate, logs, hardware info and pool earnings.

下载安装包与各版本更新说明见 [Releases](https://github.com/C3Pool/c3-miner-releases/releases/latest)；中国大陆及亚洲用户也可从亚洲镜像 download.c3pool.org 下载，文件完全相同。

Downloads and release notes for every version: [Releases](https://github.com/C3Pool/c3-miner-releases/releases/latest). Users in Asia can also download from the download.c3pool.org mirror; the files are identical.

## 安装说明

1. **浏览器提示「通常不会下载 C3Miner-…-setup.exe」**（Edge）：在下载列表中右键该文件 →「保留」→ 展开「删除」旁的箭头 →「仍然保留」。
2. **Windows 提示「Windows 已保护你的电脑」**：安装包暂未做代码签名，点「更多信息」→「仍要运行」即可。
3. **需要管理员权限**：启动时会弹出一次权限确认。挖矿程序需要它来开启大页内存和 MSR 优化，否则算力明显偏低。
4. **把安装目录 `C:\Program Files\C3 Miner` 加入杀毒软件白名单（信任区 / 排除项）**：挖矿程序常被杀毒软件（如 360、火绒、电脑管家、Microsoft Defender）误报并删除。挖矿程序也安装在这个目录里，加这一个目录即可。
5. 首次开始挖矿时，挖矿程序会先测试各算法性能，约 3 分钟，之后自动开始挖矿。
6. 首次启用大页内存后需要**重启一次电脑**，算力可提升约 50%。

支持的收款地址：XMR、USDT-TRC20、USDT-BEP20 / Polygon（0x 地址，需选择结算链）、USDT-SPL（Solana）。

在「设置」里可以设置 CPU 占用上限、使用电脑时暂停挖矿（空闲后自动恢复）、使用电池时暂停挖矿，以及开机自动启动。

卸载：Windows「设置 → 应用」中卸载 C3 Miner。卸载会同时删除开机启动任务；收款地址等设置会保留，重新安装后继续使用。

## Installation notes

1. **The browser says the installer "isn't commonly downloaded"** (Edge): right-click it in the downloads list → "Keep" → open the arrow next to "Delete" → "Keep anyway".
2. **"Windows protected your PC"**: the installer is not code-signed yet. Click "More info" → "Run anyway".
3. **Administrator rights**: you confirm once at start. The miner needs them for huge pages and MSR tuning; without them the hashrate is much lower.
4. **Add the install folder `C:\Program Files\C3 Miner` to your antivirus allow list (exclusions)**. Antivirus software (including Microsoft Defender) often flags and deletes mining programs by mistake. The mining programs are installed inside this folder too, so this one folder is enough.
5. On the first start the miner measures algorithm performance for about 3 minutes, then starts mining automatically.
6. After huge pages are enabled for the first time, **restart the computer once** for about 50% more hashrate.

Supported payout addresses: XMR, USDT-TRC20, USDT-BEP20 / Polygon (0x address, choose a settlement chain), USDT-SPL (Solana).

Settings include a CPU usage limit, pausing while you use the computer (resumes when idle), pausing on battery, and starting at sign-in.

To uninstall, remove C3 Miner in Windows Settings → Apps. The sign-in task is removed too; your payout address and settings are kept for a reinstall.
