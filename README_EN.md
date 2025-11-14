# AstroWAMP Portable Node.js Application

> **Language / Dil:** [🇹🇷 Türkçe](README.md) | [🇬🇧 English](README_EN.md)

## 🚀 Standalone Executable

This is the portable version of the AstroWAMP Node.js application. It runs as a single .exe file with Node.js runtime included.
<img width="1914" height="1025" alt="image" src="https://github.com/user-attachments/assets/df255f66-d1d2-4e83-bbf9-98eff522de02" />

<img width="1971" height="634" alt="image" src="https://github.com/user-attachments/assets/5c251090-576a-4961-b34b-100902e82932" />

<img width="1917" height="1005" alt="image" src="https://github.com/user-attachments/assets/8e587391-4b6f-44e5-ace7-839d76d4b25c" />

<img width="1918" height="1029" alt="image" src="https://github.com/user-attachments/assets/288caebd-808f-48db-baed-8b581adfae41" />

<img width="1913" height="1032" alt="image" src="https://github.com/user-attachments/assets/eda1fdb3-58ab-4582-b109-da30bc79655d" />

<img width="1215" height="922" alt="image" src="https://github.com/user-attachments/assets/7bbb5f08-b6a1-4204-951a-1ff5d175c5a5" />

<img width="1303" height="894" alt="image" src="https://github.com/user-attachments/assets/68b3ec67-8cc4-4e31-af88-aca05f912cdd" />
## 📦 Contents

```
portable/
├── AstroWAMP-NodeApp.exe    # Main executable (Node.js runtime included)
├── data/                     # Data storage (auto-created)
├── uploads/                  # File uploads (auto-created)
└── logs/                     # Application logs (auto-created)
```

## ⚡ Quick Start

### Windows

1. Double-click the `AstroWAMP-NodeApp.exe` file
2. Open `http://localhost:5000` in your browser
3. Start using it!

## 🔧 Configuration

### Changing Port

Use an environment variable to change the port number:

```cmd
set PORT=3000
AstroWAMP-NodeApp.exe
```

Or via command line:

```cmd
AstroWAMP-NodeApp.exe --port 3000
```

### Running from Different Locations

Copy the entire `portable/` folder anywhere you want:
- Different drive (C:, D:, E:, etc.)
- USB drive
- Network drive
- Cloud storage folder

The executable always runs within its containing folder.

## 🌐 API Endpoints

Once the application is running, you can access these endpoints:

- **Home Page**: `http://localhost:5000/`
- **Status API**: `http://localhost:5000/api/status`
- **System Info**: `http://localhost:5000/api/info`
- **Portable Paths**: `http://localhost:5000/api/paths`
- **Health Check**: `http://localhost:5000/api/health`

## 📝 Features

✅ **Single File**: Node.js runtime included, no additional installation required
✅ **Portable**: Runs from any location
✅ **Auto Folders**: Automatically creates required folders
✅ **Logging**: All operations are automatically logged
✅ **Modern UI**: Interface compatible with AstroWAMP design
✅ **RESTful API**: Full-featured API endpoints

## 🗂️ Data Management

### Data Folder
You can save any data to the `data/` folder:
```javascript
// Example usage in code
const filePath = path.join(DATA_DIR, 'mydata.json');
fs.writeFileSync(filePath, JSON.stringify(data));
```

### Uploads Folder
The `uploads/` folder is used for file uploads.

### Logs Folder
All operations are logged in `logs/app-YYYY-MM-DD.log` format.

## 🔒 Security

- Port is only accessible from localhost by default
- You may need to configure firewall settings for external access
- Implement additional security measures in production environments

## 🐛 Troubleshooting

### "Port Already in Use" Error
```cmd
# Use a different port
set PORT=3001
AstroWAMP-NodeApp.exe
```

### Folders Not Being Created
- Ensure you have write permissions
- Run as administrator (if necessary)

### Executable Not Running
- Check Windows Defender / Antivirus
- Add the .exe file to the "allow" list

## 📊 System Requirements

- **OS**: Windows 7/8/10/11 (x64)
- **RAM**: At least 256 MB
- **Disk**: At least 50 MB free space
- **Network**: Optional (not required for localhost only)

## 🔄 Updating

When a new version is released:
1. Backup existing `data/`, `uploads/`, `logs/` folders
2. Replace the `AstroWAMP-NodeApp.exe` file with the new version
3. Run the executable

Your data will be preserved!

## 📚 More Information
Apache (If httpd won't start, don't forget to install) -> VC_redist.x64.exe
For the main project: [AstroWAMP GitHub](https://github.com/onder7/astrowamp)

## 📄 License

MIT License - You can freely use, modify, and distribute.

---

**Made with ❤️ for AstroWAMP** | Portable Development Environment
