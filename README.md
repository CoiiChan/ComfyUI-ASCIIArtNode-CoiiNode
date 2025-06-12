# ComfyUI ASCII Art Nodes

A set of custom nodes for ComfyUI that enable the creation of various ASCII art effects from static images or text.
Features include: force_monospace option, easy font selection, and a dedicated fonts folder.

ComfyUI 的一组自定义节点，可用于从静态图片或文本生成多种 ASCII 艺术效果。
主要特性：支持强制等宽字体、便捷字体选择、独立字体文件夹。

![Preview](https://github.com/CoiiChan/CComfyUI-ASCIIArtNodeCoii/blob/main/example/CoiiNodeScreenShot.png)

## Features / 功能

This suite includes the following nodes:

1.  **ASCII Art Generator (Static):** Converts a single image into a static ASCII art image.
    - 静态 ASCII 艺术生成器：将单张图片转换为静态 ASCII 艺术图像。
2.  **ASCII Art Render:** Renders multi-line ASCII text into an image, supporting font, size, character spacing, and line height adjustments.
    - ASCII 艺术渲染：将多行 ASCII 文本渲染为图片，支持字体、字号、字间距、行高等参数。
3.  **ASCII Charset Replace:** Replaces characters in ASCII text according to two charset mappings, enabling style or symbol transformation.
    - ASCII 字符集替换：根据两个字符集顺序，将 ASCII 文本中的字符逐一替换，实现风格或符号变换。


## Installation / 安装

1.  **Download/Clone:**
    * Place the `ComfyUI_ASCIINodes` folder (containing all the `.py` node files and the `__init__.py`) into your `ComfyUI/custom_nodes/` directory.
    * Alternatively, you can use `git clone <repository_url>` into your `custom_nodes` directory if this project is hosted on a Git platform.

2.  **Install Dependencies:**
    The `requirements.txt` file should contain `Pillow>=9.0.0`

3.  **Restart ComfyUI:** After installation, restart your ComfyUI instance for the new nodes to be recognized.


## Nodes Overview & Parameters / 节点参数概览

Most nodes share a common set of parameters for ASCII generation and appearance. Unique parameters are noted for specific nodes.

### Common Parameters / 常用参数：

* `image` (IMAGE): The input image.  
  输入图片。
* `char_width` (INT): The width of the ASCII art in characters. Higher values mean more detail.  
  ASCII 艺术宽度（字符数），数值越大细节越丰富。
* `font` (STRING): The font file to use for rendering, selectable from the fonts folder or system fonts.  
  用于渲染的字体文件，可从 fonts 文件夹或系统字体中选择。
* `font_clarity_pixels` (INT): The font size (in pixels) used to render ASCII characters.  
  渲染 ASCII 字符时使用的字体像素大小。
* `ascii_charset` (STRING): The set of characters used to represent different brightness levels.  
  用于表示不同亮度的字符集。
* `background_color` (STRING): The background color of the output image (hex format, e.g., `#000000`).  
  输出图片背景色（十六进制）。
* `text_color` (STRING): The color of the ASCII characters (hex format, e.g., `#FFFFFF`).  
  ASCII 字符颜色（十六进制）。
* `invert_brightness_mapping` (BOOLEAN): If `True`, inverts the mapping of brightness to characters.  
  是否反转亮度与字符的映射。
* `force_monospace` (BOOLEAN): If `True`, enforces the use of monospace fonts for alignment.  
  是否强制使用等宽字体以保证对齐。
* `character_spacing` (FLOAT): Multiplier for the space between characters.  
  字符间距倍率。
* `line_height_scale` (FLOAT): Multiplier for the space between lines.  
  行高倍率。

---

### ADDING Node Briefs / 补充节点简述

- **ASCII Art Render**: Render multi-line ASCII text into an image with customizable font, size, spacing, and line height.  
  多行 ASCII 文本渲染为图片，支持自定义字体、字号、字间距、行高。
- **ASCII Charset Replace**: Replace characters in ASCII text according to two charset mappings, enabling style or symbol transformation.  
  按两个字符集顺序替换 ASCII 文本字符，实现风格或符号变换。

---
[![CoiiChan](https://avatars.githubusercontent.com/u/49615294?v=4)](https://github.com/CoiiChan)
## Thanks

- ASCII Art Generator code reference from LamEmil/ComfyUI_SSCIIArtNode
- 部分代码参考自LamEmil/ComfyUI_ASCIIArtNode

