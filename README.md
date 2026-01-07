<div align=center>
  
# 🛜 NetAuthLite

![NetAuthLite](./assets/images/NetAuthLite.jpg)

<!-- ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) -->
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

### "*A lightweight tool that automates campus Wi-Fi login and logout without using a browser.*"

</div>

<br>

## ⚠️ Disclaimer
**This script is intended for personal and educational use only.**  
**Use it responsibly and in accordance with your university’s IT and network policies.**  
**The author is not responsible for misuse or policy violations.**  

<br>

## ✨ Features
* One-command Wi-Fi login & logout
* Automatic background keep-alive
* No browser interaction required
* Works even after closing the terminal
* Automatically cleans up background processes

<br>

## 🖥️ Requirements
* Windows OS
* PowerShell 5.1 or later
* `curl` (included in modern Windows)
* Connected to campus/university Wi-Fi

<br>

## 📥 Installation

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Raqeeb27/NetAuthLite.git
cd NetAuthLite
```

### 2️⃣ Allow script execution (run once)
```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

<br>

## 💡Usage
> Change your working directory to the project's root directory first

### 🔐 Login to Campus Wi-Fi
> Username must be exactly 12 digits
```powershell
./NetAuthLite.ps1 login <username> <password>
```

### 🔓 Logout from Campus Wi-Fi
```powershell
./NetAuthLite.ps1 logout <username>
```

<!-- 
<br>

## ⚙️ How It Works
1. Sends login and logout requests directly to the campus gateway
2. After login, a hidden PowerShell process periodically pings the server
3. Keeps the session alive and prevents automatic disconnections
4. Each user gets an isolated keep-alive process -->

<br>

## 🚨 Common Issues

⁉️ Facing an issue? Feel free to open an Issue here, [NetAuthLite Issues](https://github.com/Raqeeb27/NetAuthLite/issues)

**1. Gateway unreachable**  
  &nbsp;&nbsp;→ Ensure you are connected to campus Wi-Fi

**2. Invalid username or password**  
  &nbsp;&nbsp;→ Verify your credentials carefully

**3. Maximum login limit reached**  
  &nbsp;&nbsp;→ You may already be logged in on another device

<br>

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for details.

<br>

## 👨‍💻 Author - Mohammed Abdul Raqeeb
*GitHub:* [Raqeeb27](https://github.com/Raqeeb27)
