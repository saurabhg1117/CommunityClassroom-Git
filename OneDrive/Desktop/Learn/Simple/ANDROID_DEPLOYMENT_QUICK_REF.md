# Android Deployment - Quick Reference

## 🎯 Choose Your Method

### ✅ Zero Local Setup (Recommended for Beginners)

**Use GitHub Actions (Cloud Build)**

1. **Already have a GitHub repo?**
   - The workflow file is ready: `.github/workflows/android.yml`
   - Just push your code: `git push`
   - Download APK from GitHub Actions tab

2. **Don't have GitHub?**
   - Sign up at https://github.com (free)
   - Push your code
   - APK builds automatically!

**Time:** 10 minutes | **Download:** 0 MB

---

### ⚡ Minimal Setup (Command-Line)

**Use Android Command-Line Tools**

1. Download: https://developer.android.com/studio#command-tools
2. Extract to `C:\Android\cmdline-tools\latest\`
3. Set environment variables (see `ANDROID_ALTERNATIVES.md`)
4. Run: `flutter build apk --release`

**Time:** 15-30 minutes | **Download:** ~100 MB

---

### 💻 VS Code User?

**Use VS Code + Flutter Extension**

1. Install VS Code: https://code.visualstudio.com/
2. Install Flutter extension
3. Install Android SDK (use command-line tools method)
4. Press `F5` to run or use terminal: `flutter build apk --release`

**Time:** 20-40 minutes | **Download:** ~50 MB + SDK

---

### 📱 Have Physical Android Device?

**Use ADB Only**

1. Download Platform Tools: https://developer.android.com/tools/releases/platform-tools
2. Extract to `C:\Android\platform-tools\`
3. Enable USB Debugging on phone
4. Connect phone
5. Run: `flutter build apk --release`

**Time:** 10 minutes | **Download:** ~10 MB

---

## 🚀 Quick Commands

### Build APK
```powershell
flutter build apk --release
```

### Build App Bundle (for Play Store)
```powershell
flutter build appbundle --release
```

### Install to Connected Device
```powershell
flutter install
```

### Check Setup
```powershell
flutter doctor
```

### List Devices
```powershell
flutter devices
```

---

## 📦 Output Locations

- **APK:** `build\app\outputs\flutter-apk\app-release.apk`
- **App Bundle:** `build\app\outputs\bundle\release\app-release.aab`

---

## 📚 Full Guides

- **Complete Alternatives Guide:** See `ANDROID_ALTERNATIVES.md`
- **Android Setup Guide:** See `ANDROID_SETUP.md`
- **Deployment Guide:** See `DEPLOYMENT.md`

---

## 💡 Recommendation

**For fastest setup:** Use **GitHub Actions** (cloud build)
- No installation needed
- Works on any computer
- Automatic builds
- Free for public repos

**For local development:** Use **Command-Line Tools** or **VS Code**
- Faster iteration
- Offline builds
- Full control

---

**Ready to deploy? Choose a method above and follow the steps!** 🎉

