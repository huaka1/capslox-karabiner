# capslox-karabiner二改

在https://github.com/yqchilde/capslox-karabiner 的基础上，增加快捷键输入手机号、QQ、身份证功能

## 安装

1. 下载 [Karabiner-Elements](https://karabiner-elements.pqrs.org/) 并安装好
2. 在默认浏览中输入下面网址，并回车
    ```shell
    karabiner://karabiner/assets/complex_modifications/import?url=https://raw.githubusercontent.com/huaka1/capslox-karabiner/main/capslox-karabiner.json
    ```
3. 跳转至Karabiner-Elements并导入
4. 在软件菜单项 `Complex modifications` 中点击左下角 `Add rule` 启用该项目全部功能

![image-20231230下午21923965](https://huaka1-tuchuang.oss-cn-hangzhou.aliyuncs.com/202312301419036.png)



5. 修改配置文件：

文件路径：~/.config/karabiner/assets/complex_modifications/

 Finder下可使用快捷键⌘⇧+G 进入到目录

找到1111行，自行修改后面的数字，手机号、QQ、身份证以此类推。

<img src="https://huaka1-tuchuang.oss-cn-hangzhou.aliyuncs.com/202312301422720.png" alt="11%image-20231230下午22259687" style="zoom: 33%;" />





## 认识键盘符号

README下文将用以下符号来表示按键位及映射键位，其代表释义如下：

| 符号 | Name     | 符号    | Name      |
| ---- | -------- | ------- | --------- |
| `⇪`  | Capslock | `↖`     | Home      |
| `⎋`  | Escape   | `↘`     | End       |
| `⌘`  | Command  | `⇞`     | Page Up   |
| `⌥`  | Option   | `⇟`     | Page Down |
| `⌃`  | Control  | `🖱️` `L` | 鼠标左击  |
| `⇧`  | Shift    | `🖱️` `R` | 鼠标右击  |
| `⌫`  | Delete   | `🖱️` `F` | 鼠标前进  |
|      |          | `🖱️` `B` | 鼠标后退  |

## 用法

### Capslock赋能成Hyper

将Capslock赋能为一个全新的功能修饰键 **✱ Hyper** ，类似于同时按下 `⇧` `⌃` `⌥` `⌘`

| 按键             | 映射为         | 说明                  |
|----------------|-------------| --------------------- |
| `⇪` 单击         | `escape`    | 单击Capslock发送ESC   |
| `⇪` 长按         | `hyper`     | 按住Capslock启用Hyper |
| `⇪` + `escape` | `caps_lock` | 单击ESC切换大写锁定   |
| `⇪` `spacebar` | `ctrl` + `spacebar` | 单击空格切换输入法    |

### Hyper => 光标移动

长按 **Capslock (✱ Hyper) 键** 配合进行操作

| 按键    | 映射为                                      | 说明       |
| ------- |------------------------------------------|----------|
| `⇪` `E` | `↑`                                      | 向上移动     |
| `⇪` `D`     | `↓`                                      | 向下移动     |
| `⇪` `S`     | `←`                                      | 向左移动     |
| `⇪` `F`     | `→`                                      | 向右移动     |
| `⇪` `A`     | `option` + `←`                           | 向左移动一个单词 |
| `⇪` `G`     | `option` + `→`                           | 向右移动一个单词 |
| `⇪` `P`     | `command` + `←` 或 `ctrl` + `A`           | 移动至行首    |
| `⇪` `;`     | `command` + `→` 或 `ctrl` + `E`           | 移动至行尾   |
| `⇪` `⌘` `P` | `fn` + `command` + `←` 或 `command` + `↑` | 移动至页首  |
| `⇪` `⌘` `;` | `fn` + `command` + `→` 或 `command` + `↓` | 移动至页尾    |

### Hyper => 光标选中

| 按键 | 映射为                                                 | 说明       |
| ---- |-----------------------------------------------------|----------|
| `⇪` `I`  | `shift` + `↑`                                       | 向上选中     |
| `⇪` `K`  | `shift` + `↓`                                       | 向下选中     |
| `⇪` `J`  | `shift` + `←`                                       | 向左选中     |
| `⇪` `L`  | `shift` + `→`                                       | 向右选中     |
| `⇪` `H`  | `shift` + `option` + `←`                            | 向左选中一个单词 |
| `⇪` `N`  | `shift` + `option` + `→`                            | 向右选中一个单词 |
| `⇪` `Y`     | `option` + `↑`                                      | 向外括选区域   |
| `⇪` `B`     | `option` + `下`                                      | 向内缩减区域   |
| `⇪` `U`  | `shift` + `command` + `←`                           | 选中至行首    |
| `⇪` `O`  | `shift` + `command` + `→`                           | 选中至行尾    |
| `⇪` `⌘` `U` | `shift` + `fn` + `command` + `←` 或 `shift` + `command` + `↑` | 选中至页首    |
| `⇪` `⌘` `O` | `shift` + `fn` + `command` + `→` 或 `shift` + `command` + `↓` | 选中至页尾    |
| `⇪` `,` | `option` + `←` && `shift` + `option` + `→`          | 选中当前单词   |
| `⇪` `⌘` `,` | `command` + `←` && `shift` + `command` + `→`        | 选中当前行 |
| `⇪` `⌘` `I` | `shift` + `option` + `↑`                            | 选中的行向上移动 |
| `⇪` `⌘` `K` | `shift` + `option` + `↓`                            | 选中的行向下移动 |

### Hyper => 数字输入

| 按键          | 映射为                                     | 说明     |
|-------------|-----------------------------------------| -------- |
| `⇪` `1`    | 136xxxxxxx | 手机号，需修改配置 |
| `⇪`  `2` | 156xxxxxx               | QQ号，需修改配置 |
| `⇪`  `3` | 01xxxxxxxxxxxxxxxx | 身份证号，需修改配置 |

### Hyper => 文本删除

| 按键        | 映射为                                    | 说明             |
| ----------- | ----------------------------------------- | ---------------- |
| `⇪` `W`     | `delete_or_backspace`                     | 向左删除         |
| `⇪` `R`     | `delete_forward`                          | 向右删除         |
| `⇪` `⌘` `W` | `option` + `delete_or_backspace`          | 向左删除一个单词 |
| `⇪` `⌘` `R` | `option` + `delete_forward`               | 向右删除一个单词 |
| `⇪` `[`     | `shift` + `home` && `delete_or_backspace` | 删除至行首       |
| `⇪` `/`     | `shift` + `end` && `delete_or_backspace`  | 删除至行尾       |
| `⇪` `⌫`     | `command` + `delete_or_backspace`         | 删除当前行       |
| `⇪` `⌘` `⌫` | `command` + `A` && `delete_or_backspace`  | 删除全部内容     |

### Hyper => F1~F12

| 按键    | 映射为 | 说明    |
| ------- | ------ | ------- |
| `⇪` `1` | `f1`   | f1按键  |
| `⇪` `2` | `f2`   | f2按键  |
| `⇪` `3` | `f3`   | f3按键  |
| `⇪` `4` | `f4`   | f4按键  |
| `⇪` `5` | `f5`   | f5按键  |
| `⇪` `6` | `f6`   | f6按键  |
| `⇪` `7` | `f7`   | f7按键  |
| `⇪` `8` | `f8`   | f8按键  |
| `⇪` `9` | `f9`   | f9按键  |
| `⇪` `0` | `f10`  | f10按键 |
| `⇪` `-` | `f11`  | f11按键 |
| `⇪` `=` | `f12`  | f12按键 |

## 参考项目

- [https://github.com/BryanHoo/Capslock-Plus](https://github.com/BryanHoo/Capslock-Plus)
- [https://github.com/Vonng/Capslock](https://github.com/Vonng/Capslock)
- https://github.com/yqchilde/capslox-karabiner