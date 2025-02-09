---
title: 欢迎使用 go-mail 文档
geekdocNav: false
#geekdocAlign: center
geekdocAnchor: false
---

[![GoDoc](https://godoc.org/github.com/wneessen/go-mail?status.svg)](https://pkg.go.dev/github.com/wneessen/go-mail)
[![codecov](https://codecov.io/gh/wneessen/go-mail/branch/main/graph/badge.svg?token=37KWJV03MR)](https://codecov.io/gh/wneessen/go-mail)
[![Go Report Card](https://goreportcard.com/badge/github.com/wneessen/go-mail)](https://goreportcard.com/report/github.com/wneessen/go-mail)
[![Crowdin](https://badges.crowdin.net/go-mail/localized.svg)](https://crowdin.com/project/go-mail)
[![GitHub release](https://img.shields.io/github/v/release/wneessen/go-mail)](https://github.com/wneessen/go-mail/releases/latest)
[![在 Awesome Go 中提到](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/avelino/awesome-go) [![#go-mail on Discord](https://img.shields.io/badge/Discord-%23gomail-blue.svg)](https://discord.gg/dbfQyC4s)
[![REUSE status](https://api.reuse.software/badge/github.com/wneessen/go-mail)](https://api.reuse.software/info/github.com/wneessen/go-mail)
<a rel="me" href="https://s.pebcak.de/@go_mail"><img alt="Mastodon Follow" src="https://img.shields.io/mastodon/follow/109378026621298088?domain=https%3A%2F%2Fs.pebcak.de&style=social"></a>
<a href="https://ko-fi.com/D1D24V9IX"><img src="https://uploads-ssl.webflow.com/5c14e387dab576fe667689cf/5cbed8a4ae2b88347c06c923_BuyMeACoffee_blue.png" height="20" alt="buy ma a coffee"></a>

<p align="center"><img src="/go-mail-2.svg" width="250" alt="go-mail logo"/></p>

go-mail 是一个易于使用的 Go 库，用于格式化和发送邮件。它使用惯用的 Go 风格，并遵循最佳实践和合理的默认值。该库仅依赖于 Go 标准库。

go-mail 的工作方式类似于编程式电子邮件客户端，并提供了许多您在 MUA 中考虑的标准方法和功能。

<div class="btn-centered btn-huge">
{{< button size="huge" relref="getting-started/introduction/" >}}开始使用 go-mail{{< /button >}}
</div>

## 特色亮点

{{< columns >}}

### 仅依赖于标准库

go-mail 不需要任何第三方模块，仅运行在 Go 标准库上

<--->

### 现代、惯用的 Go

我们使用现代和惯用的 Go 标准，遵循最先进的最佳实践和合理的默认值

<--->

### 完整的 TLS 支持

go-mail 支持不同策略的隐式 STARTTLS，以及用于发送邮件服务器的显式 SSL/TLS 的连接

{{< /columns >}}

{{< columns >}}

### 上下文

我们利用 Go 上下文进行更好的控制流和超时/取消处理

<--->

### SMTP 认证

支持三种常见的 SMTP 认证机制（LOGIN、PLAIN、CRAM-MD5）以及自定义身份验证。

<--->

### 邮件地址验证

go-mail 遵循 RFC5322 并验证提供的邮件地址

{{< /columns >}}

{{< columns >}}

### 常见邮件头支持

go-mail 提供了许多常见邮件头的生成器（Message-ID、Date、Bulk-Precedence、Priority 等）

<--->

### 连接重用

您可以在同一 SMTP 连接上发送多个邮件

<--->

### 附件/嵌入

来自不同来源（本地文件系统、`io.Reader` 或 `embed.FS`）的附件和内联嵌入的完全支持

{{< /columns >}}

{{< columns >}}

### 编码和内容类型

go-mail 支持不同的编码和内容类型

<--->

### 中间件

第三方库的中间件支持，以便更改邮件消息以满足其需求

<--->

### Sendmail 和文件存储

支持通过本地 sendmail 安装发送邮件消息以及输出到本地文件（例如作为磁盘上的 `.eml` 文件以在 MUA 中打开它们）

{{< /columns >}}

{{< columns >}}

### MDN 和 DSN

go-mail 提供了请求 MDN（RFC 8098）和 DSN（RFC 1891）的支持

<--->

### 模板支持

支持 Go 的 `html/template` 和 `text/template`（作为消息正文、替代部分或附件/嵌入）

<--->

### DKIM 支持

通过 [go-mail-middlware/dkim](https://github.com/wneessen/go-mail-middleware/tree/main/dkim) 中间件的 DKIM 签名支持

{{< /columns >}}

{{< columns >}}

### 调试日志记录

支持 SMTP 客户端将任何 SMTP 通信记录到 STDERR 以进行调试目的

<--->

### 自定义交付错误

使用 `SendError` 类型，用户可以获取有关交付错误的详细信息，包括错误是否为临时性质

<--->

{{< /columns >}}

## 支持
我们在 Discord 上有一个支持和一般讨论频道。找到我们：[#go-mail](https://discord.gg/dbfQyC4s)
