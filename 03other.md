<a id="mulu">目录</a>
<a href="#mulu" class="back">回到目录</a>
<style>
    .back{width:40px;height:40px;display:inline-block;line-height:20px;font-size:20px;background-color:lightyellow;position: fixed;bottom:50px;right:50px;z-index:999;border:2px solid pink;opacity:0.3;transition:all 0.3s;color:green;}
    .back:hover{color:red;opacity:1}
    img{vertical-align:bottom;}
</style>

<!-- @import "[TOC]" {cmd="toc" depthFrom=3 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->



<!-- /code_chunk_output -->

<!-- 打开侧边预览：f1->Markdown Preview Enhanced: open...
只有打开侧边预览时保存才自动更新目录 -->

**IPv6简写规则**：
- 每组前面的0的可以省略不写
    完整`2403:A200:A200:1100:0000:0000:0F00:0003`
    简写`2403:A200:A200:1100:0000:0000:F00:3`
- 连续为0的一组或多组，可以用`::`代替，一个IP中只能用一次`::`
    完整：`2403:A200:A200:1100:0000:0000:0F00:0003`
    简写：`2403:A200:A200:1100::F00:3`
- 如果一组中全为0，又不想用`::`代替，每组中要保留1个0
    完整：`2403:A200:A200:0000:AFFF:0000:0000:0003`
    简写：`2403:A200:A200:0:AFFF::3`

**页表占多少页面**：虚拟地址空间大小*物理页号/页面大小^2^
**磁盘空间利用率**：
- 没有采用成组操作时：每个逻辑记录长度/块大小
- 采用成组操作时：每个逻辑记录长度/块大小*块因子

**每个进程最多可申请的资源数**=总资源数/进程数，向上取整
**用户程序最多可分成多少页**：2^逻辑地址位数^/内存分块大小
