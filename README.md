# IgniMailer

IgniMailer is a high-performance, professional-grade bulk email automation suite designed for businesses that demand reliability and speed. Engineered with a modern Chromium core, it delivers pixel-perfect HTML previews and robust SMTP delivery management.

## 🚀 Key Features

- **⚡ Advanced SMTP Engine**: Built-in support for intelligent SMTP rotation with session memory and failover. Easily load multiple SMTP servers from a text file to prevent spam blocks and rate limits.
- **💎 Rich Composition**: Full-featured HTML editor with live visual synchronization powered by PyQt6 WebEngine. Import existing HTML templates or compose from scratch.
- **🔄 Dynamic Personalization (Mail Merge)**: Seamlessly integrate custom attributes using mail merge. Automatically extract placeholders like `{Name}` or `{Company}` from your loaded recipient lists to personalize each email.
- **📂 Broad Format Support**: Load recipient lists from Excel (`.xlsx`, `.xls`), CSV (`.csv`), or plain text (`.txt`) files.
- **📎 Attachment Support**: Easily attach multiple files to your email campaigns.
- **💾 Campaign Management**: Save your current subject, message, delay settings, and configurations as an `.imc` template file to quickly reload future campaigns.
- **📊 Real-time Monitoring**: Live status log and progress bar. Keep track of successful and failed deliveries in real-time, and export the detailed system log or recipient lists once the campaign finishes.
- **🔄 Auto-Updates**: Built-in GitHub release checker ensures you are always running the latest version.

## 🛠️ Prerequisites

Before running IgniMailer, ensure you have Python installed along with the following required libraries:

```bash
pip install PyQt6 PyQt6-WebEngine pandas openpyxl
```

## 💻 How to Use

1.  **Clone or Download** this repository.
2.  **Run the application**:
    ```bash
    python ready.py
    ```
3.  **Configure SMTP**: Navigate to the **SMTP Settings** tab to enter your manual configuration or load a bulk list of SMTP servers for auto-rotation.
4.  **Compose Campaign**: Go to the **Compose** tab. Load your recipients list, set an appropriate delay (e.g., 1.0 to 5.0 seconds), and draft your subject and message. You can use `{ColumnName}` variables for mail merge.
5.  **Send**: Click "Start Sending" to begin your campaign. Monitor progress in the **Status Log** tab.

## ⚠️ Important Notes

- **Delay**: It is highly recommended to set a sending delay (e.g., 1.0 - 5.0 seconds) to avoid rate limiting and IP blacklisting from email providers.
- **SMTP Format**: When bulk loading SMTPs from a `.txt` file, ensure they follow the exact format: `host|port|user|pass` (one per line).

## 📄 License & Copyright

Copyright © 2026 IGNIVION. All Rights Reserved.  
Crafted with precision by Vijay Vairagade.
