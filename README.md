Mi Claro 梆梆企业加固 Frida 检测绕过（学习测试使用）

> 仅用于学习与测试目的  
> 本项目对 **Mi Claro** 应用中的梆梆企业加固（Bangcle）所使用的 `libDexHelper.so` 进行逆向分析，并通过 **ARM64 汇编十六进制 NOP 替换** 绕过 Frida 检测机制。  
> **请勿用于任何商业或非法用途**。如涉及侵权，请联系仓库所有者删除。


**修改后效果**：Frida 可正常附加进程，无需隐藏 Server。

---

使用方法

1. 拉取本仓库修改后的 `libDexHelper.so`
2. 使用 **root 设备**，替换原应用中的同名文件：
libDexHelper.so /data/app/com.claro.xx/base.apk/lib/
3.并给予文件755权限

适用于64位系统因为修改的是64位的libDexHelper.so文件
推测梆梆企业加固的应用通用
