
直播源列表工具TeleList
运行使用需要安装Microsoft .NET Framework 4.5+以上版本
WindowsXP请下载专用的版本并且需要Microsoft.NET Framework 4.0
如果遇到乱码请尝试将文本编码转为UTF-8带BOM的编码，至少做一次转换。

UTF-8（Unicode Transformation Format - 8-bit）是一种 Unicode 字符编码方式，它是 Unicode 字符集的一种编码方案之一。UTF-8 使用变长编码方式，可以表示 Unicode 字符集中的所有字符，并且与 ASCII 编码兼容。在 UTF-8 中，单个字符的编码长度可以是 1 到 4 个字节，具体取决于字符的 Unicode 码点。

UTF-8（无 BOM）指的是不包含字节顺序标记（Byte Order Mark，BOM）的 UTF-8 编码。BOM 是一个特殊的 Unicode 字符（U+FEFF），用于标识文本文件的字节顺序（大端序或小端序），以及文件的编码方式（UTF-8、UTF-16 等）。在 UTF-8 编码的文本文件中，通常不包含 BOM，因为 UTF-8 是一种无字节顺序的编码方式。

UTF-8（带 BOM）指的是包含字节顺序标记的 UTF-8 编码。UTF-8 编码的 BOM 由三个字节组成（0xEF, 0xBB, 0xBF），用于标识文件的编码方式为 UTF-8，并且不包含字节顺序信息。带 BOM 的 UTF-8 文件通常用于指示文件的编码方式，并且在 Windows 环境下常见。

在实践中，大多数情况下，UTF-8 编码的文本文件都不包含 BOM。因为 BOM 在一些场景下可能会引起解析问题，特别是在处理器或解析器不支持 BOM 的情况下。但是，在某些环境下，带 BOM 的 UTF-8 文件可能有其特定的用途，比如在 Windows 平台下与一些应用程序或工具的兼容性要求。