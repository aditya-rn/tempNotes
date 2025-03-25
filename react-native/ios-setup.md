# React Native iOS Development Environment Setup

## Prerequisites
This guide will help you set up a development environment for React Native iOS development on macOS.

## Step-by-Step Installation Guide

### 1. Install Homebrew (if not already installed)
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### 2. Install Node.js
```bash
brew install node
```

### 3. Install Watchman
```bash
brew install watchman
```

### 4. Install Xcode
- Open the App Store
- Search for Xcode
- Click "Get" or "Install"
- After installation, open Xcode

### 5. Install Xcode Command Line Tools
```bash
xcode-select --install
```

### 6. Install iOS Simulator
1. Open Xcode
2. Go to Xcode > Preferences
3. Click on the "Components" tab
4. Select and download an iOS Simulator from the list

### 7. Install Ruby Version Manager (rbenv)
```bash
brew install rbenv
```

### 8. Initialize rbenv
```bash
rbenv init
```

### 9. Install Ruby 2.7.5
```bash
rbenv install 2.7.5
rbenv global 2.7.5
```

### 10. Configure Shell to Use rbenv
Add the following lines to your `~/.zshrc` file:
```bash
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(rbenv init -)"' >> ~/.zshrc
```

### 11. Install CocoaPods
```bash
sudo gem install cocoapods
sudo gem install -n /usr/local/bin ffi cocoapods
pod setup
```

## Troubleshooting
- If you encounter any Ruby version conflicts, ensure you're using Ruby 2.7.5
- Make sure Xcode Command Line Tools are properly installed
- Restart your terminal after making configuration changes

## References
- [React Native Official Setup Guide](https://reactnative.dev/docs/set-up-your-environment?platform=ios)
- [Stack Overflow Ruby Version Help](https://stackoverflow.com/questions/74189532/your-ruby-version-is-2-6-8-but-your-gemfile-specified-2-7-5)

## Notes
- Always ensure you have the latest versions of the tools
- Some steps may require administrator permissions
- The exact process might vary slightly depending on your macOS version
