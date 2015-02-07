# 🐼 — a better way to start an iOS project

1. Start from the archetype

  ```console
  cd ima-make-an-ios-app
  git init
  git fetch --depth=1 -n https://github.com/toolbear/panda.git
  git reset --hard $(git commit-tree FETCH_HEAD^{tree} -m "start with 🐼 archetype")
  pod install
  open -a Xcode .
  ```

2. Press **⌘U**; tests ✅

3. Push to GitHub; enable Travis; tests ✅

---

[![Build Status](https://travis-ci.org/toolbear/panda.svg?branch=master)](https://travis-ci.org/toolbear/panda)

---

## Features

* [ ] One-time project customization
  1. Bootstrap from 🐼 archetype
  2. Customize
  3. Go!
* [x] Schemes and Build configurations ready for continuous deployment
  * [x] `Debug` → `AdHoc` → `AppStore` or
  * [ ] `Debug` → `AdHoc` → `Enterprise`
* [x] Project keychain for your signing identity
  * [x] Avoid codesigning pitfalls
  * [ ] Run Travis CI builds against real devices
  * [ ] Distribute beta builds from Travis
* [x] Side-by-side install of development, beta, and release builds
  * [x] Customized names
  * [ ] Customized app icons and launch images
* [x] Single Target with parameterized `Info.plist`
* [ ] Less `.xcodeproj` churn; many settings externalized  in `.xcconfig`
* [x] CocoaPods pre-configured
* [x] Spec-style Logic Tests
* [ ] Modern Xcode defaults
  * [ ] strict warnings
  * [x] 2-space indent

## License

Choose your own adventure.

* MIT: see [LICENSE](LICENSE)
* Public Domain
