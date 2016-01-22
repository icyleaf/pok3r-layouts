# POK3R 针对 Mac 的键盘布局

如果你还不知道 POK3R 键盘的话，请看[评测](https://www.youtube.com/watch?v=8wjW-Or1jg8)。
对于国内目前的购买渠道请直接淘宝搜索 `poker 3 机械键盘` 或者进行海淘 [amazon](http://smile.amazon.com/Mechanical-Keyboard-Keycaps-Cherry-Mx-Blue/dp/B00OFM51L2/), [mechanicalkeyboards.com](https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=1233)

编辑层分布：

- 默认层：无法进行编辑修改。使用 `FN + M` 切换
- 第二层：OS X 键位 (蓝灯常亮），使用 `FN + ,<` 切换
- 第三层：未设置 (红灯常亮），使用 `FN + .>` 切换
- 第四层：未设置 (红蓝灯，又称紫灯常亮），使用 `FN + /?` 切换

## POK3R 通用信息
- Vortex 网站的[POK3R 用户说明书](http://www.vortexgear.tw/db/upload/webdata4/vortex_20156296454697283.pdf)
- 恢复初始化: 按着左右键位的 `ALT` 键直到 LED 灯停止闪烁（大约 5 秒）
- 恢复当前编辑层: 按着 `FN + R` 键直到 LED 灯停止闪烁（大约 5 秒）

### 键盘编程
- 默认层无法编程
- 按下 `FN + R_Ctrl` 进入编程模式，如果 `FN` 键已经分配使用 `L_Ctrl`键（空格键右侧的 LED 蓝灯常亮）
- 选中你要设置的`目标键` 再按下你要分配的`新键值` (最多可以编程 31 个键）最后按下 `PN` 进行确认保存 (按下目标键后灯会一直闪烁直到改键保存后恢复常亮)
- 重复上面步骤进行多次编程
- 退出编程模式按下 `FN + R_Ctrl` （空格右侧的 LED 蓝灯熄灭）

## OS X 键位布局
- `FN + ,<` 切换到第二编辑层
* [使用 L_Ctrl 替换 FN 键](#Move_FN)
* 按下 `FN + R_Ctrl` 进入编程模式
* [常规绑定](#common_bindings)
* 替换空格左右侧的 Cmd/Option 键:
  * L_Cmd: `L_Alt` -> `L_WIN` -> `PN`
  * L_Option: `L_WIN` -> `L_Alt` -> `PN`
  * R_CMD: `R_Alt` -> `R_FN` (Win) -> `PN`
  * R_Option: `R_FN` (Win) -> `R_Alt` -> `PN`
* `FN + R_Ctrl` to exit programming

可视化键盘布局如下:

![OSX 布局](img/layout-osx.png)
OSX Layout on [keyboard-layout-editor.com](http://www.keyboard-layout-editor.com/##@_name=Pok3r%20Layer%203%20for%20OSX%2F%2FMac&author=davidjenni&notes=See%20%5Bgithub%5D(https%2F:%2F%2F%2F%2Fgithub.com%2F%2Fdavidjenni%2F%2Fpok3r-layouts)%3B&@_y:1.5&c=%233c4041&t=%23aba18b&p=DCS&a:5%3B&=%0A%0A%0A%0A%60%20~%0A%0AEsc&_a:4%3B&=!%0A1%0A%0A%0AF1&=%2F@%0A2%0A%0A%0AF2&=%23%0A3%0A%0A%0AF3&=$%0A4%0A%0A%0AF4&=%25%0A5%0A%0A%0AF5&=%5E%0A6%0A%0A%0AF6&=%2F&%0A7%0A%0A%0AF7&=*%0A8%0A%0A%0AF8&=(%0A9%0A%0A%0AF9&=)%0A0%0A%0A%0AF10&=%2F_%0A-%0A%0A%0AF11&=+%0A%2F=%0A%0A%0AF12&_w:2%3B&=%0ABackspace%0A%0A%0ADel%3B&@_w:1.5%3B&=%0ATab&=Q&=W&=E&=R%0A%0A%0A%0AReset&=T%0A%0A%0A%0A15ms&=Y%0A%0A%0A%0ACal&=U%0A%0A%0A%0APgUp&_c=%23c7c3b5&t=%23ba1312%3B&=I%0A%0A%0A%0AHome&_c=%233c4041&t=%23aba18b%3B&=O%0A%0A%0A%0APgDn&=P%0A%0A%0A%0APrtSc&=%7B%0A%5B%0A%0A%0AScrlk&=%7D%0A%5D%0A%0A%0APause&_w:1.5%3B&=%7C%0A%5C%3B&@_c=%23c7c3b5&t=%23ba1312&w:1.25&w2:1.75%3B&=%0ACtrl&_x:0.5&c=%233c4041&t=%23aba18b%3B&=A&=S&=D&_c=%23c7c3b5&t=%23ba1312%3B&=F%0A%0A%0A%0APgDn&_c=%233c4041&t=%23aba18b%3B&=G%0A%0A%0A%0A0.1s&_c=%23c7c3b5&t=%23ba1312%3B&=H%0A%0A%0A%0ALeft&=J%0A%0A%0A%0ADown&=K%0A%0A%0A%0AUp&=L%0A%0A%0A%0ARight&_c=%233c4041&t=%23aba18b%3B&=%2F:%0A%2F%3B%0A%0A%0AIns&=%22%0A'%0A%0A%0ADel&_w:2.25%3B&=%0AEnter%3B&@_w:2.25%3B&=%0AShift&=Z&=X&=C&=V&_c=%23c7c3b5&t=%23ba1312%3B&=B%0A%0A%0A%0APgUp&_c=%233c4041&t=%23aba18b%3B&=N%0A%0A%0A%0AEnd&=M%0A%0A%0A%0ADefault&=%3C%0A,%0A%0A%0ALayer%202&=%3E%0A.%0A%0A%0ALayer%203&=%3F%0A%2F%2F%0A%0A%0ALayer%204&_w:2.75%3B&=%0AShift%3B&@_c=%23c7c3b5&t=%23ba1312&w:1.25%3B&=%0AFN&_w:1.25%3B&=%0AOption&_w:1.25%3B&=%0ACMD&_c=%233c4041&t=%23aba18b&p=DCS%20SPACE&w:6.25%3B&=&_c=%23c7c3b5&t=%23ba1312&p=DCS&w:1.25%3B&=%0ACMD&_w:1.25%3B&=%0AOption&_c=%233c4041&t=%23aba18b&w:1.25%3B&=%0APn&_w:1.25%3B&=%0ACtrl)

## <a name="common_bindings"></a>适用所有操作系统的常规绑定
* CapsLock 必须改为 Ctrl:
  * 依次按下 `CapsLock` -> `L_Ctrl` -> `PN`
  * `FN + CapsLock` -> `L_Ctrl` -> `PN`
* VIM 党的钟爱的 HJKL 和上下翻页:
  * 左: `FN + H` -> `FN + J` -> `PN`
  * 下: `FN + J` -> `FN + K` -> `PN`
  * 上: `FN + K` -> `FN + I` -> `PN`
  * 下一页: `FN + F` -> `FN + O` -> `PN`
  * 上一页: `FN + B` -> `FN + U` -> `PN`
* Home: `FN + I` -> `FN + H` -> `PN`
* 音量控制 controls:
  * 静音: `FN + X` -> `FN + /?` -> `PN`
  * 减小音量: `FN + C` -> `FN + ,<` -> `PN`
  * 加大音量: `FN + V` -> `FN + .>` -> `PN`

## <a name="Move_FN"></a>使用 L_Ctrl 替换 FN 键
HJKL as cursor keys are more ergonomical to reach by moving the FN to the left Ctrl key location:
* 切换到需要设置的编辑层(2, 3, 4)，这个只是单个编辑层有效
* 拔掉键盘的 USB 连接线
* 把键盘背后的 DIP 4 切换到 ON
* 插上 USB 连接线，依次按下 `FN` -> `L_Ctrl` -> `PN` -> `PN` (仅修改 FN 键，PN 键保持不变)
* 最后把 DIP 4 恢复 OFF (无需再把 USB 连接线)

## 参考来源

特别感谢 [davidjenni/pok3r-layouts](https://github.com/davidjenni/pok3r-layouts) 的布局教程，以上内容基于原文进行了部分的替换和中文化处理。以下是原教程涉及的相关参考：

* [r/mk: HowTo program pok3r](http://www.reddit.com/r/MechanicalKeyboards/comments/35uy60/guide_howto_program_your_pok3r_programming_layers/)
* [r/mk: HowTo media controls pok3r](http://www.reddit.com/r/MechanicalKeyboards/comments/37j3sx/guide_modification_pok3r_media_volume_controls_hw/)
 
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>

This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

