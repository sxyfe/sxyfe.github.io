# my-blog

## Hugo 启动报错：`TOCSS ... this feature is not available in your current Hugo version`

这是因为主题（`hugo-theme-stack`）会用 Hugo Pipes 的 `toCSS` 编译 SCSS，而该能力 **只在 Hugo Extended** 里提供。

- **推荐修复（恢复正常样式）**：安装/切换到 Hugo Extended

  - Homebrew（macOS）：
    - `brew install hugo`（或）`brew reinstall hugo`
  - 验证命令输出里包含 `extended`：
    - `hugo version`
  - 如果你 `brew install hugo` 后仍然不是 extended，通常是 **PATH 指向了旧的 hugo** 或 **brew 没有 link 成功**：
    - 查看当前使用的是哪个：
      - `which -a hugo`
    - 典型修复（/usr/local/bin/hugo 冲突）：
      - `mv /usr/local/bin/hugo /usr/local/bin/hugo.bak`（或删除它）
      - `brew link --overwrite hugo`
      - `hash -r`
      - 再跑 `hugo version` 确认包含 `extended`

- **兜底修复（能启动，但无主题样式）**：本仓库已在 `layouts/partials/` 增加覆盖模板；当检测到非 extended Hugo 时，会跳过 SCSS 编译并输出 warning，从而让 `hugo server` 能正常启动。
