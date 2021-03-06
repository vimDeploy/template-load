# Template local 使用说明

## 说明：

编辑新文件加载模板文件

## 选项：

```
    (数字)g:template_load
            如果设置为0以禁用模板自动加载，1为启用。

    (数字)g:template_loadconfirm
            如果设置为1，每次你编辑一个新文件，你会被要求是否加载模板或没有。

    (字符串)g:template_path
            如果设置，脚本会查找模板文件中的这条道路，如果没有设置，该脚本将查
            找模板文件中与runtimepath每个路径。

    (字符串)g:template_dir_name
            默认情况下，如果g：template_path没有设置，脚本会查找模板文件和
            'runtimepath'里''/template/'，'~/.vim/template/'例如，你可以定制你
            自己的目录中设置此值的名称。如果'g:template_path'被设定，该值永远
            不会被使用

    (字符串)g:template_prefix
            默认的模板文件名是'tpl.extension'，例如，如果你创建一个'foo.c'，
            '~/.vim/template/tpl.c'将被加载。您可以将该值设置为'skel'加载
            'skel.c'

    (数字)g:template_tags_replacing
            如果设置为1，一些预先定义的标记将被替换
            以下变量：
                (字符串)g:T_AUTHOR
                (字符串)g:T_AUTHOR_EMAIL
                (字符串)g:T_AUTHOR_WEBSITE
                (字符串)g:T_LICENSE
                (字符串)g:T_DATE_FORMAT（相同的strftime）
                (数字)g:T_FILENAME_USE_FULL_PATH
                        （如果是1，/foo/bar.c将被使用，否则，bar.c）
            预先定义的标签：
                <T_AUTHOR>，<T_AUTHOR_EMAIL>，<T_AUTHOR_WEBSITE>
                <T_LICENSE>，<T_FILENAME>，<T_CREATE_DATE>
                <T_CURSOR>
                        如果发现<T_CURSOR>，将光标放在这里和<T_CURSOR>将被删除

    (数字)g:template_replace_start_line
            开始标记从这里更换。默认值是1

    (数字)g:template_replace_end_line
            结束标记替换到这里。默认是最后一行("$")

    (数字)g:template_reminder
            默认不提醒模板缺失。默认的参数1是提醒。
```
