# 🐼 — a better way to start a new iOS project

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
