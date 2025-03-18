# 📚 CTemplate
A simple C project template using **CMake** and **Ninja** for fast, cross-platform builds.

---

## 📂 Project Structure
```
c_template/
├── .vscode/              # VSCode configuration
│   └── settings.json
├── src/                  # Source files
│   └── main.c            # Main C program
├── .editorconfig         # Code style rules
├── .gitignore            # Ignore build artifacts and temporary files
├── CMakeLists.txt        # CMake configuration file
├── README.md             # Project documentation
└── LICENSE               # License file
```

---

## 🚀 Setup Instructions

### ✅ 1. Install Dependencies
- **Linux** (Ubuntu/Debian):
```bash
sudo apt update
sudo apt install cmake ninja-build gcc
```

- **Windows** (Using Chocolatey):
```bash
choco install cmake ninja
```

- **macOS** (Using Homebrew):
```bash
brew install cmake ninja
```

---

### ✅ 2. Clone the Repository
Clone the project and navigate into the directory:
```bash
git clone https://github.com/lzygmanksi/c_template.git
cd c_template
```

---

### ✅ 3. Build the Project
1. Create a `build/` directory:
```bash
mkdir build
cd build
```

2. Configure the project using **CMake**:
```bash
cmake -G Ninja ..
```

3. Build the project:
```bash
ninja
```

---

### ✅ 4. Run the Project
```bash
./bin/c_template
```

---

### ✅ 5. Clean the Build
```bash
ninja clean
```

---

## 🛠️ VSCode Setup
1. Install the following extensions:
   - ✅ CMake Tools
   - ✅ C/C++ Extension Pack

---

## 🌙 Neovim Setup
1. Install `cmake-language-server` in Neovim:
```bash
:MasonInstall cmake-language-server
```

2. Configure Neovim (`init.lua`):
```lua
require'lspconfig'.clangd.setup{}
require'lspconfig'.cmake.setup{}
```

3. Build from Neovim:
```bash
:!ninja -C build
```

4. Run from Neovim:
```bash
:!./build/bin/c_template
```

---

## 🌍 Cross-Platform Compatibility
| Platform | Build Command | Run Command |
|----------|---------------|-------------|
| **Linux** | `cmake -G Ninja .. && ninja` | `./bin/c_template` |
| **Windows** | `cmake -G Ninja .. && ninja` | `./bin/c_template.exe` |
| **macOS** | `cmake -G Ninja .. && ninja` | `./bin/c_template` |

---

## ✅ Troubleshooting
| Problem | Solution |
|---------|----------|
| **CMake not found** | Ensure CMake is installed and available in `PATH` |
| **Ninja not found** | Install Ninja using your package manager |
| **Build errors** | Check `CMakeLists.txt` and build dependencies |
| **Debugging doesn't work** | Ensure `gdb` or `lldb` is installed |

---

## 📜 License
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 🌟 Contributing
1. Fork the project
2. Create a feature branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m "Add feature"`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a pull request

---

## 🚀 That's It!
🎉 You're ready to build and run your C project using **CMake + Ninja** on both Linux and Windows!

🔥 **Happy Coding!** 🔥

