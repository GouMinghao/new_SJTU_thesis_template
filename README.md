# 上海交通大学研究生毕业论文LaTex模板
上海交通大学研究生院今年发布了官方[LaTex模板](https://www.gs.sjtu.edu.cn/info/1136/8374.htm)。但是此模板显然存在一些问题，也存在一些使用不太方便的地方，在此处进行了修改与调整。

## 使用方法
### 本地编译
1. 无论你使用的是什么操作系统，在使用前需要确保已经完成了[texlive](https://tug.org/texlive/)的安装。本项目只支持使用XeLaTex进行编译。


2. 克隆或者直接[下载](https://github.com/GouMinghao/new_SJTU_thesis_template/releases/download/v1.0.0/v1.0.0.zip)本项目
```bash
git clone https://github.com/GouMinghao/new_SJTU_thesis_template.git
```

3. 运行`build.sh` 或者`build.bat`来完成编译。

### 使用Overleaf
1. 下载本模板的[zip包](https://github.com/GouMinghao/new_SJTU_thesis_template/releases/download/v1.0.0/v1.0.0.zip)，或者克隆过后自行压缩打包。
2. 上传至[Overleaf](https://latex.sjtu.edu.cn/)。
3. 选择编译器为`XeLaTex`即可完成编译。

## 与官方模板相比的修改

### BUG修复
1. 修复了官方模板中表格使用了图片计数器导致表格编号不正确的问题。
2. 修复了使用LaTex编译时`\quad`后面不加空格导致编译报错的问题。
3. 修复了使用`section*`部分时，生成超链接位置不对的问题。
4. 修复了使用XeLaTex编译时英文字体不是`Times New Roman`的问题。

### 改进
1. 添加了对`.bib`文件进行引用的支持。
2. 优化了`main.tex`的结构，将文件进行分离，避免在一个文件中写太多代码。
3. 将章节号改为使用引用的方式，避免硬编码章节号。
4. 优化了附录的格式，放弃了`section*`的方式，避免无法引用附录中的章节。

## 感谢
1. 感谢sjtug提供的[非官方模板](https://github.com/sjtug/SJTUThesis)以及递归感谢。

## 软件许可证
1. 本repo绝大部分代码来自于上海交通大学[官方模板](https://www.gs.sjtu.edu.cn/info/1136/8374.htm)，校徽等版权归上海交通大学所有。
2. `biblatex-gb7714-2015`样式文件使用[`LPPL`](https://www.latex-project.org/lppl.txt)许可证。
3. 其余部分使用[Apache License 2.0](./LICENSE)许可证