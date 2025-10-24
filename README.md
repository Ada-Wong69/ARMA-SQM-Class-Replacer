## 🧩 Executable: SqmClassReplacer.exe

`SqmClassReplacer.exe` is the main executable used to replace classes within `mission.sqm` files for Arma.

### 🔧 How it works

- Optionally uses **CfgConvert.exe** (from Arma 3 Tools) to **debin** and **bin** `.sqm` files.
- Automatically **reads the path to CfgConvert.exe from the Windows Registry**.
- If the path is found, the UI displays:
  - ✅ A checkbox to **debin** (convert binary `.sqm` to text format)
  - ✅ A checkbox to **bin** (convert text `.sqm` back to binary format)
- These options are available only if CfgConvert is detected — but **CfgConvert is not required** for basic class replacement.

### 🧹 Additional Features

- 🧽 **Removes Logic paths** from the SQM file — especially useful when **porting missions from older Arma titles** (e.g., Arma 2 or Arma: Cold War Assault).
- ⚠️ **Important:** Do **not** include `join` and `destroy` in combo file, as they may cause the game to crash.

### 📁 Requirements

- Arma 3 Tools (optional, only needed for debin/bin functionality)
- **Microsoft Visual C++ Redistributable for Visual Studio 2017 (x64)**
[https://aka.ms/vs/17/release/vc_redist.x64.exe](https://aka.ms/vs/17/release/vc_redist.x64.exe)

### ✅ Supported operations

- Replace specific classes in `mission.sqm`
- Create automatic backups (when backup checkbox is **checked**)
- Can remove referenced addons from SQM files
- It can remove logic paths from previous versions of Arma
