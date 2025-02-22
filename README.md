[English](#windows-terminal-context-menu) | [简体中文](#windows-terminal-上下文菜单)

# Windows Terminal Context Menu

The script provided by this repository can generate `Terminal here` right-click menus in File Explorer for Windows Terminal.

- Licensed under [the MIT Licence](LICENSE).
- Adapted from [lextm/windowsterminal-shell](https://github.com/lextm/windowsterminal-shell).

## How to use

- These scripts require [new PowerShell](https://github.com/PowerShell/PowerShell) (version at least 6).

Clone this repository and extract it, then open PowerShell and run `generate.ps1`.

- *If your system does not allow to execute unsigned PowerShell scripts, you can execute the following command to allow the current PowerShell process to execute unsigned scripts:*

    ```powershell
    Set-ExecutionPolicy Bypass -Scope Process
    ```

`generate.ps1` supports the following parameters:

`-Layout` : Indicates the menus layout

- `Compact`: Items in nested menus (default)
- `Flat`: Items in the top menu
- `Minimal`: Minimal layout (run Terminal with the default profile)

`-Extended`: Whether are extended menus (shows only when holding down the `Shift` key)

- `No`: No (default)
- `Yes`: Yes
- `Admin`: Only the items that run Terminal as administrator

`-NoAdmin`: Do not add items that run Terminal as administrator

`-Language`: Specifies which language to use for the menu items (if not specified, the system language will be used)

To remove the menus, please run `remove.ps1`.

---

# Windows Terminal 上下文菜单

该仓库提供的脚本可以为 Windows Terminal 在文件管理器中生成 `在此处打开终端` 的右键菜单。

- 以 [MIT Licence](LICENSE) 许可。
- 修改自 [lextm/windowsterminal-shell](https://github.com/lextm/windowsterminal-shell)。

## 怎么用

- 这些脚本需要[新 PowerShell](https://github.com/PowerShell/PowerShell)（版本至少为 6）。

克隆这个仓库，然后打开 PowerShell 运行 `generate.ps1`。

- *如果你的系统不允许执行未签名的 PowerShell 脚本，你可以执行以下命令以允许当前 PowerShell 进程执行未签名脚本：*

    ```powershell
    Set-ExecutionPolicy Bypass -Scope Process
    ```

`generate.ps1` 支持以下参数：

`-Layout`：菜单布局

- `Compact`：条目在二级菜单（默认）
- `Flat`：条目在一级菜单
- `Minimal`：迷你布局（以默认配置运行终端）

`-Extended`：是否为扩展菜单（仅在按住 `Shift` 键时显示）

- `No`：否（默认）
- `Yes`：是
- `Admin`：仅以管理员身份运行的选项

`-NoAdmin`: 不添加以管理员身份运行的选项

`-Language`：指定要在菜单选项中使用的语言（如果未指定，将使用系统语言）

要移除菜单，请运行 `remove.ps1`。
