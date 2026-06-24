# Material Color

[中文](#中文) · [English](#english)

Material Color 是一款为 Visual Studio Code 提供 Material 风格语法高亮、
明暗色界面主题和文件图标的扩展。

Material Color provides Material-style syntax highlighting, light and dark
workbench themes, and a file icon theme for Visual Studio Code.

![Material Color dark theme preview](https://cdn.jsdelivr.net/gh/guobing1993/githubimg@main/utools/1616995482983-show.png)

> 当前截图展示暗色主题。Claude Light 预览图将在后续补充。
>
> The current screenshot shows a dark theme. A Claude Light preview will be
> added later.

## 中文

### 功能

- 一套适用于常见编程语言和标记语言的 Material 风格语法高亮。
- 三个暗色主题和一个 Claude 风格亮色主题。
- 独立的 Material Color 文件图标主题。
- 针对编辑器、终端、Diff、搜索、选中状态和括号高亮的完整界面配色。

### 可用主题

| 主题名称 | 类型 | 说明 |
| --- | --- | --- |
| **Material Color (Claude Light)** | 亮色 | Claude 风格界面，融合 Material Color 语法高亮，并针对亮色背景调整可读性 |
| **Material Color Dark** | 暗色 | 当前主要维护的 Material Color 暗色主题 |
| **Material Color(Dark Modern)** | 暗色 | VS Code Dark Modern 界面与 Material Color 语法高亮的组合 |
| **Material Color** | 暗色 | 原始 Material Color 暗色主题 |

### 安装与启用

1. 在 VS Code 扩展面板中搜索并安装 **Material Color**。
2. 打开命令面板，运行 **Preferences: Color Theme**。
3. 选择上表中的任一主题。

也可以使用快捷键打开主题选择器：

- macOS：`⌘K ⌘T`
- Windows / Linux：`Ctrl+K Ctrl+T`

启用文件图标时，运行 **Preferences: File Icon Theme**，然后选择
**Material Color**。

### Claude Light

**Material Color (Claude Light)** 的工作台配色基于社区项目
[Claude Code Theme](https://github.com/ashwingopalsamy/claude-code-theme)
进行适配。语法 scope、规则顺序和字体样式沿用原始 Material Color
主题，前景色则针对 `#FAF9F5` 亮色编辑器背景进行了调整。

亮色主题默认使用 `#E98A68` 作为编辑器和终端光标颜色。

### 光标设置

颜色主题可以控制光标颜色，但不能控制光标宽度或闪烁方式。若需要
3 像素宽的光标，请在 `settings.json` 中加入：

```json
{
    "editor.cursorWidth": 3,
    "editor.cursorBlinking": "blink"
}
```

如需仅覆盖 Claude Light 的光标颜色，可以使用主题级配置：

```json
{
    "workbench.colorCustomizations": {
        "[Material Color (Claude Light)]": {
            "editorCursor.foreground": "#E98A68",
            "terminalCursor.foreground": "#E98A68"
        }
    }
}
```

## English

### Features

- Material-style syntax highlighting for common programming and markup
  languages.
- Three dark themes and one Claude-inspired light theme.
- A standalone Material Color file icon theme.
- Workbench colors for the editor, terminal, diffs, search, selections, and
  bracket highlighting.

### Available themes

| Theme | Type | Description |
| --- | --- | --- |
| **Material Color (Claude Light)** | Light | Claude-inspired workbench colors combined with Material Color syntax highlighting adjusted for a light background |
| **Material Color Dark** | Dark | The primary maintained Material Color dark theme |
| **Material Color(Dark Modern)** | Dark | VS Code Dark Modern workbench colors with Material Color syntax highlighting |
| **Material Color** | Dark | The original Material Color dark theme |

### Installation and activation

1. Search for and install **Material Color** from the VS Code Extensions view.
2. Open the Command Palette and run **Preferences: Color Theme**.
3. Select one of the themes listed above.

You can also open the theme picker with:

- macOS: `⌘K ⌘T`
- Windows / Linux: `Ctrl+K Ctrl+T`

To enable the file icons, run **Preferences: File Icon Theme** and select
**Material Color**.

### Claude Light

The workbench palette in **Material Color (Claude Light)** is adapted from the
community project
[Claude Code Theme](https://github.com/ashwingopalsamy/claude-code-theme).
Its syntax scopes, rule ordering, and font styles come from the original
Material Color theme. Foreground colors are adjusted for readability on the
`#FAF9F5` editor background.

The light theme uses `#E98A68` for the editor and terminal cursors.

### Cursor settings

Color themes can define cursor colors, but cursor width and blinking are editor
settings. Add the following to `settings.json` to use a 3-pixel cursor:

```json
{
    "editor.cursorWidth": 3,
    "editor.cursorBlinking": "blink"
}
```

To override cursor colors only for Claude Light, use a theme-specific
customization:

```json
{
    "workbench.colorCustomizations": {
        "[Material Color (Claude Light)]": {
            "editorCursor.foreground": "#E98A68",
            "terminalCursor.foreground": "#E98A68"
        }
    }
}
```

## 许可与归属 / License and attribution

Claude Light 的界面颜色来源和 MIT 许可声明见
[THIRD_PARTY_NOTICES.md](./THIRD_PARTY_NOTICES.md)。

The source and MIT license notice for the Claude Light workbench colors are
available in [THIRD_PARTY_NOTICES.md](./THIRD_PARTY_NOTICES.md).

项目的其他许可信息见 [LICENSE](./LICENSE) 和 [LICENSE.md](./LICENSE.md)。

Additional project license information is available in [LICENSE](./LICENSE)
and [LICENSE.md](./LICENSE.md).
