##编辑
ctrl + space 自动完成名称（任意类，方法名，变量名）注意系统输入法切换的快捷键冲突
ctrl + shift + space  职能代码完成（所期望类型的变量和方法列表供选择）
ctrl + alt + space  类名自动完成，如果没有import会自动import（project里的任意类名，包括jar包里）
ctrl + shift + enter  在末尾自动添加";"完成当前语句
ctrl + p 提示当前调用方法参数信息
ctrl + q 快速查看描述
shift + f1 外部文档
ctrl + mouse over code 按住ctrl键，然后鼠标移动上面会显示信息摘要
ctrl + f1 在错误或者警告上显示说明
alt + insert 代码自动生成（getter,setter,构造方法，hashcode等对象常用方法）
ctrl + o 重写（覆盖）方法
ctrl + i 实现方法
ctrl + alt + t 调用代码模板
ctrl + / 行注释的启用和取消
ctrl + shift + / 代码块注释启用和取消
ctrl +ｗ　递进式选择代码块
ctrl + shift + w 返回上一次选择的代码状态
alt + q 上下文信息，如在类的任意地方按此快捷键查看类的定义
alt + enter 显示坑你的动作和快速修复的方式供选择
ctrl + alt + l 代码格式化
ctrl + alt + o 优化import 导入，其实就是将每个类中的导入无效的import移除
ctrl + alt +l 自动缩进
tab /shift + tab 缩进和取消缩进
ctrl + x/shift +delete 剪贴当前行或选定块到剪贴板
ctrl + c/ctrl + insert 复制当前行或选择块到剪贴板
ctrl + v /shift + insert 从剪贴板粘贴
ctrl + shift +v 从剪贴板缓存中选择信息粘贴
ctrl + d 复制并粘贴当前行或选择块
ctrl + y 删除当前行或者选定块
ctrl + shift +j 自动将下一行合并到当前行末尾
ctrl + enter  智能分隔行
shift + enter 开始新一行
ctrl + shift + u  切换当前词或者选定块的大小写（全大写或者小写）
ctrl + shift + ]/[ 从当前光标选定到代码结束/开始（注意是代码块，不是代码行）
ctrl + delete 删除到当前词结尾
ctrl + backspace 删除到当前词开头
ctrl +  +/- 展开/折叠代码块
ctrl + shift + + 展开所有代码
ctrl + shift + -折叠所有
ctrl + f4 关闭当前编译tab
##搜索替换
ctrl + f  查找
f3 查找下一个
shift + f3 查找上一个
ctrl + r 替换
ctrl + shift + f 在制定路径查找
ctrl + shift + r 在指定路径替换
ctrl + shift + s 搜索结构，这里的结构可以是方法，代码模板等
ctrl + shift + m 替换结构，这里的结构可以是方法，代码模板等
alt + f7/ ctrl + f7搜索最近使用的地方/在文件中搜索使用的地方
ctrl + shift + f7高亮显示文件中使用的部分
ctrl + alt + f7 显示使用地方（可以显示方法、变量等在哪些地方使用）
##编译和执行
ctrl + f9 项目构建（编译修改和相关）
ctrl + shift + f9 编译选定的文件，包或模块
alt + shift + f10 选择配置和运行（弹出窗口，选择要运行的项目，运行）
alt + shift + f9 选择配置和调试（弹出窗口，选择要调试的项目，调试
shift + f10 运行
shift + f9 调试
ctrl + shift + f10 从编译器运行配置的上下文（运行选定的类或当前编译的类）
##调试
f8 跳过
f7 步入
shift + f7 智能步入
shift + f8 跳出
alt + f9 运行到光标处
alt + f8 计算表达式
f9 恢复程序运行
ctrl + f8 切换断点
ctrl + shift + f8 查看断点
##导航
ctrl + n 打开制定类
ctrl +　shift + n 打开制定文件
ctrl + alt + shift + n 前往制定的变量，方法
alt + right/left 转到下一个/上一个编辑器标签
f12 回到前一个工具窗口
esc 进入编辑器（从工具窗口）
shift + esc 隐藏当前或最后一个激活的工具窗口
ctrl + shift + f4 关闭当前运行/消息/查找...标签
ctrl +　ｇ调到指定行
ctrl + e 弹出最近查看过的文件
ctrl + alt + left/right 导航前进/后退
ctrl + shift +backspace 跳到最近一次编辑的位置
alt + f1 在任意视图弹出选择当前文件或者功能窗口
ctrl + b / ctrl + click 跳到声明
ctrl + alt + b 调到具体的实现方法，查找抽象方法的具体实现
ctrl + shift + i 快速查找定义
ctrl + shift + b 前往类型声明
ctrl ＋u 前往父类方法/父类
alt + up/down 上一个/下一个方法
ctrl + ]/[ 移动到代码块结束/开始
ctrl + f12 弹出文件结构，支持快速查找当前类的变量，方法，可以使用模糊查询
ctrl + h 类层次结构
ctrl + shift + h 方法层次结构
ctrl + alt + h 调用层次
f2/shift + f2 下一个/上一个高亮
f4/ctrl + enter 编译源/查看源
alt + home 显示导航栏
f11 设定/取消书签
ctrl + shift + f11 使用助记符设定/取消书签
ctrl + #【0-9】跳转指定标号的书签
shift + f11 查看书签

##重构
f5 文件复制
f6 文件移动
alt +　delete 安全删除
shift + f6 改名
ctrl + f6 更改签名
ctrl + alt + n 内联
ctrl + alt + m 提取方法
ctrl + alt +v 提取局部变量
ctrl + alt + f 提取实例变量
ctrl + alt + c 提取常量
ctrl + alt + p 提取作为方法入参

##代码管理
ctrl + k 提交项目
ctrl + t 更新项目
alt + shift + c 查看最近更改
alt + backquote 弹出快速做做的窗口

##模板
ctrl + alt + j  弹出模板选择窗口
ctrl +　ｊ　插入动态模板
iter  循环迭代模板
inst instanceof模板
itit 迭代器的循环模板
itli list的循环模板
psf  静态常量模板
thr 抛出新异常模板
##general
alt + #[0-9] 打开响应工具窗口
ctrl + s 全部保存
ctrl + alt + y 同步刷新
ctrl + alt + f11 切换全屏模式
ctrl + shift + f12编辑器最大化
alt + shift + f 添加到收藏夹
alt + shift + i 查看项目当前文件
ctrl + backquote 款速切换当前系统架构（配色、代码模板、快捷键）
ctrl + alt + s 打开ide 系统设置
ctrl + alt + shift +ｓ当前项目的结构设置
ctrl + shift +a 查找操作
ctrl + tab 标签和工具窗口快速切换
