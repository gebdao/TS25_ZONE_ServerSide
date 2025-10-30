# TS25_ZONE_ServerSide

Server-side source code for the TwelveSky2 private server project.

## 🧩 Overview
This repository contains the C++ source files for the **Zone Server**, which handles:
- Player connections and synchronization
- Inventory management and item stacking
- Monster spawning and world updates
- Server-to-server communication

## 📁 Structure
| File | Description |
|------|--------------|
| `S01_Zone.cpp` | Main zone logic |
| `S02_MyServer.cpp` | Server management |
| `S03_MyUser.cpp` | User data handling |
| `S10_MyWorld.cpp` | World state updates |
| `Database.cpp / .h` | Database interface |
| `MyUser.h / .cpp` | Player data structures |

## 🧱 Build Instructions
Use **Visual Studio 2013–2022** (x64 C++).  
This code links to shared TwelveSky2 game libraries and requires the client header files and dependencies used in the main project.

Typical build setup:
1. Open Visual Studio → New Project → Win32 Console Application.
2. Add all `.cpp` and `.h` files from this repository.
3. Configure include paths for shared headers (if part of full TS2 server source).
4. Build in Release mode.

## 🤖 Using GitHub Copilot
Once uploaded to GitHub, you can open any file and use Copilot Chat to ask:
- “Explain what `PutInventory1` does.”  
- “Optimize stacking logic for iSort == 3.”  
- “Show me where player zone transitions are handled.”

Copilot will read all `.cpp` and `.h` files from this repository.

## 🧠 Notes
- Keep `.gitignore` to prevent build files from being committed.
- Make sure your repository is **public** if you want Copilot indexing.

---

© 2025 — Open source for educational and modding purposes.
