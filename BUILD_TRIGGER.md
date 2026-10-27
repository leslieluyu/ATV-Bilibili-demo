# Build Trigger

专门用来触发 GitHub Actions 打未签名 IPA。

用法：把下面的 `build` 数字加 1，然后 push 到 `main`。

```
git add BUILD_TRIGGER.md
git commit -m "chore: bump build trigger"
git push origin main
```

首次使用前请打开仓库 Actions 页，若提示启用 workflow，先点 Enable。

构建完成后在 Actions 对应 run 的 Artifacts 里下载 `BilbiliAtvDemo.ipa`，再用 Sideloadly 装到 Apple TV。

build: 1
