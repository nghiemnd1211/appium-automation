# Setup environments
1. Install nodejs
2. Install appium : npm install -g appium
   (Know issues and fix): sudo chown -R $USER/usr/local
3. Default location
On WinOS
- Globally: C:\Android\sdk
- User: C:\Users\<current-username>\AppData\Local\Android\sdk
On MacOS
- ~/Library/Android/sdk
4. Install commandline-tools
- C:\Android\sdk\cmdline-tools\tools\bin
5. Execute sdkmanager
- Locate to ...sdk
- execute: sdkmanager platform-tools emulator
6. Setup path for C:\Android\sdk\platform-tools
7. install appium-doctor
- npm i appium-doctor -g
- appium-doctor

install vysor > adb devices
(udid-unique device identifier)
   Note: need to remember that enable debugging(2modes), disable (verifying ...)

Download maven apache > set up path

Launch App Test
- Run appium -p 4725
- run: adb shell dumpsys window | grep -E mCurrentFocus
- or just adb shell dumpsys window
  alternative: dumpsys window windows

** Resolver personal issue
Need to install build-tools by running sdkmanager "build-tools;29.0.3"
