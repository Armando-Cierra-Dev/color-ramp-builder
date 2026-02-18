# 🍎 macOS Installation

## "App is damaged" error?

macOS blocks unsigned apps downloaded from the internet. The app is **NOT damaged** - it just needs Apple's $99/year certificate to avoid this message.

## Quick Fix

After downloading, open **Terminal** and run:

```bash
xattr -cr "/Applications/Color Ramp Builder.app"
```

Then open the app normally.

## Alternative: Right-click Method

1. Open **Finder** → **Applications**
2. **Right-click** (or Control + Click) on **Color Ramp Builder**
3. Click **"Open"**
4. Click **"Open"** again in the dialog

You only need to do this once.

## Why does this happen?

macOS Gatekeeper requires apps to be signed with an Apple Developer certificate. Since this is a free open-source app, it's not signed.

## Is it safe?

Yes, if you downloaded it from the official GitHub repository. The source code is open for inspection.

---

Still having issues? [Open an issue on GitHub](https://github.com/Armando-Cierra/color-ramp-builder/issues)