---
layout: "default"
title: "🛠️ ctfd-mcp - Easy Challenge Management for CTFd Users"
description: "🛠️ Manage CTFd challenges with ease: list, read details, control docker instances, and submit flags—all from an intuitive MCP server designed for users."
---
# 🛠️ ctfd-mcp - Easy Challenge Management for CTFd Users

[![GitHub Release](https://img.shields.io/github/v/release/umbra2728/ctfd-mcp?sort=semver)](https://github.com/AaryaBhusal/ctfd-mcp/releases)
[![License](https://img.shields.io/github/license/umbra2728/ctfd-mcp)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.13%2B-blue)](https://www.python.org/downloads/)
[![Issues](https://img.shields.io/github/issues/umbra2728/ctfd-mcp)](https://github.com/umbra2728/ctfd-mcp/issues)

CTFd MCP server allows users to manage challenges easily, view details, control dynamic Docker instances, and submit flags.

## 🚀 Getting Started

Follow these steps to download and run the ctfd-mcp server.

### 📥 Download & Install

Visit this page to download:

[Download the latest release](https://github.com/AaryaBhusal/ctfd-mcp/releases)

### 💻 System Requirements

Make sure your system meets these requirements:

- Python 3.13 or higher. You can download it from [Python's official site](https://www.python.org/downloads/).
  
### 🔧 Setting Up Environment Variables

You need to set environment variables to connect to the CTFd server properly. Choose one of the following authentication methods:

- `CTFD_URL`: Enter your CTFd server URL (e.g., `https://ctfd.example.com`).
  
- If you use tokens:
  - `CTFD_TOKEN`: This should be your user token (note: not an admin token).
  
- If tokens are disabled, use:
  - `CTFD_SESSION`: This session cookie connects you to the server.

- Optionally, if required by your server or the plugin:
  - `CTFD_CSRF_TOKEN`: Include this only if your setup requires CSRF protection.

To store these variables, create a file named `.env` in the root of your downloaded repository. Here is an example of what to include in your `.env` file:

```bash
CTFD_URL=https://ctfd.example.com
CTFD_TOKEN=your_user_token
```

### ⚙️ Running the Application

1. Open your terminal or command prompt.
2. Navigate to the directory where you downloaded ctfd-mcp.
3. Run the following command:

```bash
python app.py
```

This command will start the server. Now, you can access the application.

### 🌐 Accessing the Application

After starting the server, you can access it using a web browser. Open your preferred browser and type:

```
http://localhost:5000
```

You should see the ctfd-mcp interface, ready for you to explore.

### ❓ Troubleshooting Common Issues

If you experience any issues, consider these tips:

- **Python Version**: Ensure you have Python 3.13 or higher installed.
- **Environment Variables**: Check that your `.env` file contains the correct information.
- **Firewall Settings**: Ensure your firewall allows connections on the port you are using (default is 5000).
  
If you encounter other issues, you can check the [issues page](https://github.com/umbra2728/ctfd-mcp/issues) for help.

### 📝 Additional Features

The ctfd-mcp server offers several useful features:

- **Challenge Listing**: Easily view and manage challenges available on your CTFd server.
  
- **Dynamic Docker Instances**: Start and stop Docker containers dynamically as needed.

- **Flag Submission**: Seamlessly submit flags during challenges.

### 📣 Community and Support

You can join our community to share tips and get help:

- **GitHub Discussions**: Engage with other users and developers in the discussions section on GitHub.
- **Documentation**: Check the [documentation](https://github.com/umbra2728/ctfd-mcp/wiki) for detailed information on all features.

### 🔗 Useful Links

- [Download the latest release](https://github.com/AaryaBhusal/ctfd-mcp/releases)
- [GitHub Repository](https://github.com/umbra2728/ctfd-mcp)
- [Python Official Site](https://www.python.org/downloads/)
- [Issues Page](https://github.com/umbra2728/ctfd-mcp/issues)

Enjoy using ctfd-mcp to manage your CTFd challenges easily!