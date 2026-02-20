# Lottery Manager App (Burmese)

A web-based lottery ticket management application for Burmese 3-digit lottery, converted to Android APK using Capacitor.

## Features

- 🎯 3-digit lottery ticket management
- 📊 Real-time profit/loss calculation
- 💾 Local storage with backup/restore functionality
- 📱 Mobile-friendly responsive design
- 🔄 Master ticket layoff system
- ⚙️ Customizable commission and limits

## How to Build APK

### Automatic Build (GitHub Actions)
The APK is automatically built on every push to the main branch. You can download the latest APK from the [Releases](https://github.com/Sawkhin558/lottery-app-apk/releases) page.

### Manual Build
1. Clone the repository:
   ```bash
   git clone https://github.com/Sawkhin558/lottery-app-apk.git
   cd lottery-app-apk
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Add Android platform:
   ```bash
   npx cap add android
   ```

4. Sync and build:
   ```bash
   npx cap sync android
   cd android
   ./gradlew assembleDebug
   ```

5. Find the APK at: `android/app/build/outputs/apk/debug/app-debug.apk`

## Permissions

The app requires storage permissions to:
- Export backup files
- Import backup files
- Save data locally

## Usage

1. **Entry Tab**: Enter lottery tickets in format: `123.231=100*100` or `123=100r50`
2. **Vouchers Tab**: View and manage all entered vouchers
3. **Master History**: Track tickets sent to master
4. **Report Tab**: View self and master reports
5. **Profit Tab**: Calculate profit/loss with winning number
6. **Settings**: Configure commission, limits, and backup/restore

## File Format Examples

- Direct bet: `123=100`
- Rolled bet: `123=0*100`
- Mixed: `123=100*50`
- Multiple numbers: `123.231=100*100`
- R format: `123=100r50`

## License

MIT License