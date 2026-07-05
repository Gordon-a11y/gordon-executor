# 🥷 GORDON — Protected Python Executor

**GORDON** is a high‑security Python obfuscation and execution tool.
It encrypts Python scripts using multi‑layer AES‑256 with PBKDF2 key derivation, making reverse‑engineering extremely difficult.

> 🔒 **Encryption Level:** Maximum (3 layers, 1.2M iterations per layer)

---

## 📦Features

- 🔐 **Triple‑layer Fernet encryption** (AES‑256 in CBC mode)
- 🧂 **Dynamic salt per layer** – prevents rainbow table attacks
- 🌀 **PBKDF2‑HMAC‑SHA256** with 1,200,000 iterations
- 📁 **Key‑file based authentication** – no hardcoded passwords
- ⚡ **One‑command execution** – just provide the key file
- 🐧 Cross‑platform (Linux, Termux, macOS)

---

## 🚀 Installation

### 📱 Termux (Android)

```bash
pkg update && pkg upgrade -y
pkg install python git -y
pip install cryptography
git clone https://github.com/Gordon-a11y/gordon-executor.git
cd gordon-executor
💻 Kali Linux / Debian
bash
sudo apt update
sudo apt install python3 python3-pip git -y
pip3 install cryptography
git clone https://github.com/Gordon-a11y/gordon-executor.git
cd gordon-executor
🔑 How to Use
Place your .gordonkey file in the same folder as the protected script.

Or use the --key argument to specify a custom path.

Run the protected script:

bash
python3 "[§]Gordon🥷🏻_ATTACK⚔️_protected.py"
Or with a custom key:

bash
python3 "[§]Gordon🥷🏻_ATTACK⚔️_protected.py" --key /path/to/your/keyfile
🗂️ File Structure
text
gordon-executor/
│
├── [§]Gordon🥷🏻_ATTACK⚔️_protected.py # Encrypted script
├── [§]Gordon🥷🏻_ATTACK⚔️.gordonkey # Secret key file (required)
└── README.md
⚙️ Technical Details
Parameter Value
Encryption Fernet (AES‑256‑CBC)
Key Derivation PBKDF2‑HMAC‑SHA256
Iterations 1,200,000 per layer
Layers 3
Unique Salt per layer
Payload Encoding Base64
❗ Important Notes
The .gordonkey file is mandatory – without it, the script will not run.

The key is not stored inside the script – it must be provided externally.

This tool is designed for legitimate protection of proprietary code.

Misuse for malicious purposes is not supported.

📄 License
This project is released under the MIT License – use it responsibly.

🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

📬 Contact
GitHub: @Gordon-a11y

Telegram: t.me/Gordon_a11y

⭐ Star this repo if you find it useful!

text

---

## 🔄 Shortened version of commands only (for quick copying)

```bash
# Termux
pkg update && pkg upgrade -y
pkg install python git -y
pip install cryptography
git clone https://github.com/Gordon-a11y/gordon-executor.git
cd gordon-executor

# Kali Linux
sudo apt update
sudo apt install python3 python3-pip git -y
pip3 install cryptography
git clone https://github.com/Gordon-a11y/gordon-executor.git
cd gordon-executor

# Run
python3 "[§]Gordon🥷🏻_ATTACK⚔️_protected.py"
