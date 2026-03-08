# Claude Code Skills Collection

我的 Claude Code 技能集合，包含 DNS 管理和 VPS 运维的自动化工具。

## 📦 技能列表

### dns-api.skill
DNS 管理自动化技能，支持多个主流云服务商的 DNS API 操作。

**支持的服务商：**
- 🌐 **Cloudflare** - 全球知名的 CDN 和 DNS 服务提供商
- ☁️ **腾讯云 (Tencent Cloud)** - 国内主流云服务商
- 🔷 **阿里云 (Aliyun)** - 国内领先的云计算平台

**主要功能：**
- DNS 记录的增删改查 (CRUD)
- 动态 DNS (DDNS) 支持
- 批量域名管理
- API 密钥安全存储
- 多服务商切换指南

**适用场景：**
- 自动化域名解析更新
- 动态 IP 地址绑定
- 多域名批量配置
- DNS 记录备份与迁移

---

### vps-ops.skill
VPS 服务器运维管理技能，简化日常运维操作。

**主要功能：**
- 服务器状态监控
- 批量命令执行
- 系统配置自动化
- 日志分析与管理
- 性能优化建议

**适用场景：**
- 多台 VPS 集中管理
- 自动化部署脚本
- 系统健康检查
- 安全配置优化

## 🚀 使用方法

### 安装
将 `.skill` 文件复制到 Claude Code 的 skills 目录：

```bash
# Linux/MacOS
cp *.skill ~/.claude/skills/

# Windows
copy *.skill %USERPROFILE%\.claude\skills\
```

### 调用技能
在 Claude Code 中使用 `/` 命令调用技能：

```
/dns-api      # 启动 DNS 管理技能
/vps-ops      # 启动 VPS 运维技能
```

## 📋 依赖要求

- Claude Code CLI 工具
- 对应云服务商的 API 凭证（用于 dns-api）
- SSH 访问权限（用于 vps-ops）

## 🔐 安全提示

- 请妥善保管 API 密钥和 SSH 凭证
- 建议使用环境变量存储敏感信息
- 定期轮换访问凭证

## 📝 更新日志

### v1.0.0
- 初始版本发布
- 支持 Cloudflare、腾讯云、阿里云 DNS API
- 基础 VPS 运维功能

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

MIT License
