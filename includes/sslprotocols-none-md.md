从 .NET Framework 4.7 开始，此方法使用 <xref:System.Security.Authentication.SslProtocols.None> 进行身份验证，这允许操作系统选择要使用的最佳协议，并将其用于阻止不安全的协议。 在 .NET Framework 4.6（以及安装了最新安全修补程序的 .NET Framework 4.5）中，允许的 TLS/SSL 协议版本为 1.2、1.1 和 1.0（除非通过编辑 Windows 注册表禁用强加密）。