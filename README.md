# ld64 编译项目

这个项目使用 GitHub Actions 自动编译 ld64 链接器。

## 使用步骤

### 1. 创建 GitHub 仓库

1. 访问 https://github.com/new
2. 仓库名输入：`ld64-build`
3. 选择 **Public**（公开）
4. 点击 **Create repository**

### 2. 上传文件

将以下文件上传到仓库：
- `.github/workflows/build.yml`
- `README.md`

### 3. 触发编译

1. 进入仓库页面
2. 点击 **Actions** 标签
3. 点击 **Build ld64**
4. 点击 **Run workflow**
5. 点击绿色的 **Run workflow** 按钮

### 4. 下载编译结果

1. 等待编译完成（约 5-10 分钟）
2. 点击编译任务
3. 滚动到底部 **Artifacts** 部分
4. 点击 **ld64-linux-x86_64** 下载

### 5. 上传到 iSH

将下载的 `ld64` 文件上传到 iSH 的 `/var/minis/workspace/` 目录。

---

## 注意事项

- GitHub Actions 每月有 2000 分钟免费额度
- 编译完成后记得下载结果
- 如果编译失败，检查 Actions 日志
