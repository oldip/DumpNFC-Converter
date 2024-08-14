# Dump NFC 转换器 2.1

Dump NFC 转换器 2.1 是一个用于将 `.dump` 文件转换为 `.nfc` 文件，或者将 `.nfc` 文件转换为 `.dump` 文件的工具。该工具提供了简单的拖放功能，使得文件转换变得更加容易。

## 特性

- 支持 `.dump` 文件转换为 `.nfc` 文件
- 支持 `.nfc` 文件转换为 `.dump` 文件
- 处理未完全破解的 NFC 文件
- 简单的拖放界面

## 使用方法

1. 下载可执行文件。
2. 双击 `DumpNFC转换器2.1.exe` 运行程序。
3. 将一个或多个 `.dump` 或 `.nfc` 文件拖放到程序窗口中。
4. 程序将自动转换文件，并将结果保存到以下目录：
   - `.dump` 文件转换后的 `.nfc` 文件保存在 `dump2nfc` 文件夹中。
   - `.nfc` 文件转换后的 `.dump` 文件保存在 `nfc2dump` 文件夹中。

### 处理未完全破解的 NFC 文件

如果在 `.nfc` 文件中检测到未完全破解的块（包含 `??`），程序将提示用户是否继续转换。若用户选择继续，未破解的区域将被替换为预设字符：

- 每第四个块替换为 `FF FF FF FF FF FF FF 07 80 69 FF FF FF FF FF FF`
- 其他块替换为 `00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00`

## 示例

### 转换 `.dump` 文件为 `.nfc` 文件

1. 打开程序。
2. 将 `.dump` 文件拖放到程序窗口中。
3. 转换后的 `.nfc` 文件将保存在 `dump2nfc` 文件夹中。

### 转换 `.nfc` 文件为 `.dump` 文件

1. 打开程序。
2. 将 `.nfc` 文件拖放到程序窗口中。
3. 如果文件包含未完全破解的块，程序将提示用户是否继续转换。
4. 转换后的 `.dump` 文件将保存在 `nfc2dump` 文件夹中。

## 许可证

版权所有 © 2024 oldip

未经许可，不得复制、修改、发布、传播、出售、分发本软件或其任何部分。

### 禁止商业用途

本软件仅供个人学习和研究使用，禁止用于任何商业目的。

### 免责声明

本软件按“原样”提供，不提供任何形式的明示或暗示担保，包括但不限于适销性、特定用途适用性和非侵权性。在任何情况下，作者均不对因使用或无法使用本软件而产生的任何索赔、损害或其他责任负责，无论是在合同诉讼、侵权诉讼或其他诉讼中。
