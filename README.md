# Welcome to your Expo app 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## 1. System requirements
- CPU: AMD / Intel CPU running at 2.8 GHz or higher 
- RAM: 4GB
- Node.js (LTS).
- macOS, Windows (Powershell and WSL 2), and Linux are supported.

## 2. Installation instructions

### 1) Install dependencies

- macOS / Linux (using nvm):

   ```bash
   # install nvm (if needed)
   curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
   # reload shell (or open a new terminal)
   export NVM_DIR="$HOME/.nvm" && [ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh"
   # install an LTS node
   nvm install --lts
   nvm use --lts
   node --version
   npm --version
   ```

- Windows: use nvm-windows (https://github.com/coreybutler/nvm-windows) or the official Node.js installer (https://nodejs.org/).

### 2) (MacOS) Install Watchman and SDK

1. Install Watchman
   ```bash
   brew install watchman
   ```
2. Install SDK

   - Install OpenJDK distribution called Azul Zulu using Homebrew. This distribution offers JDKs for both Apple Silicon and Intel Macs.
   ```bash
   brew install --cask zulu@17
   ```

### 2) Install Java (JDK)

- Recommended: OpenJDK 11 or 17. Verify with:
   
   ```bash
   java -version
   ```
   
### 3) Install Android Studio and SDK

- Download Android Studio: https://developer.android.com/studio
- Open Android Studio -> SDK Manager and install:
  - Android SDK Platform (choose API level e.g., 33)
  - Android SDK Build-Tools
  - Android SDK Platform-Tools
  - Android Emulator
  - Android SDK Command-line Tools
 
  - 

## 3. Configuration steps
### Android environment variables (macOS / Linux - add to `~/.zshrc` or `~/.bashrc`)

Adjust the SDK path if your installation is elsewhere:

```bash
# Android SDK
export ANDROID_HOME=$HOME/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

Reload the path environment variables in your current shell:

zsh
```zsh
source $HOME/.zshrc
```

bash
```bash
source $HOME~/.bashrc
```

## 4. Project creation

1. Create a new React Native CLI project

```bash
npx create-expo-app@latest <your app>
```
   
2. Get a fresh project

When you're ready, run:

```bash
npm run reset-project
```

This command will move the starter code to the **app-example** directory and create a blank **app** directory where you can start developing.

## 5. Running the project in an Android emulator

### 1) Start an Android Virtual Device (AVD)

### 2) Run the app (React Native CLI)

From project root:

```bash
npm run start
```

### 3) Run the app in an Android emulator

```bash
expo start
# press 'a' in the terminal to launch Android emulator 
```

## Learn more

To learn more about developing your project with Expo, look at the following resources:

- [Expo documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with our [guides](https://docs.expo.dev/guides).
- [Learn Expo tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial where you'll create a project that runs on Android, iOS, and the web.

## Join the community

Join our community of developers creating universal apps.

- [Expo on GitHub](https://github.com/expo/expo): View our open source platform and contribute.
- [Discord community](https://chat.expo.dev): Chat with Expo users and ask questions.
