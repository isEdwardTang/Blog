---
layout: post
title: "学习资源汇总"
categories: Kotlin
tags:   primer Kotlin
author: Edward
---

* content
{:toc}

从github上搬运过来的学习站点，具体参考：[伯乐在线]（https://github.com/jobbole/）





## 一、Python

<h3><a id="user-content-环境管理" class="anchor" href="#环境管理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>环境管理</h3>
<p>管理 Python 版本和环境的工具</p>
<ul>
<li>p：非常简单的交互式 python 版本管理工具。<a href="https://github.com/qw3rtman/p">官网</a></li>
<li>pyenv：简单的 Python 版本管理工具。<a href="https://github.com/yyuu/pyenv">官网</a></li>
<li>Vex：可以在虚拟环境中执行命令。<a href="https://github.com/sashahart/vex">官网</a></li>
<li>virtualenv：创建独立 Python 环境的工具。<a href="https://pypi.python.org/pypi/virtualenv">官网</a></li>
<li>virtualenvwrapper：virtualenv 的一组扩展。<a href="https://pypi.python.org/pypi/virtualenvwrapper">官网</a></li>
</ul>
<h3><a id="user-content-包管理" class="anchor" href="#包管理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>包管理</h3>
<p>管理包和依赖的工具。</p>
<ul>
<li>pip：Python 包和依赖关系管理工具。<a href="https://pip.pypa.io/">官网</a></li>
<li>pip-tools：保证 Python 包依赖关系更新的一组工具。<a href="https://github.com/nvie/pip-tools">官网</a></li>
<li>conda：跨平台，Python 二进制包管理工具。<a href="https://github.com/conda/conda/">官网</a></li>
<li>Curdling：管理 Python 包的命令行工具。<a href="http://clarete.li/curdling/">官网</a></li>
<li>wheel：Python 分发的新标准，意在取代 eggs。<a href="http://pythonwheels.com/">官网</a></li>
</ul>
<h3><a id="user-content-包仓库" class="anchor" href="#包仓库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>包仓库</h3>
<p>本地 PyPI 仓库服务和代理。</p>
<ul>
<li>warehouse：下一代 PyPI。<a href="https://github.com/pypa/warehouse">官网</a>
<ul>
<li>Warehouse：PyPA 提供的 PyPI 镜像工具。<a href="https://warehouse.python.org/">官网</a> <a href="https://bitbucket.org/pypa/bandersnatch">bandersnatch</a></li>
</ul>
</li>
<li>devpi：PyPI 服务和打包/测试/分发工具。<a href="http://doc.devpi.net/">官网</a></li>
<li>localshop：本地 PyPI 服务（自定义包并且自动对 PyPI 镜像）。<a href="https://github.com/mvantellingen/localshop">官网</a></li>
</ul>
<h3><a id="user-content-分发" class="anchor" href="#分发" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>分发</h3>
<p>打包为可执行文件以便分发。</p>
<ul>
<li>PyInstaller：将 Python 程序转换成独立的执行文件（跨平台）。<a href="https://github.com/pyinstaller/pyinstaller">官网</a></li>
<li>dh-virtualenv：构建并将 virtualenv 虚拟环境作为一个 Debian 包来发布。<a href="http://dh-virtualenv.readthedocs.org/">官网</a></li>
<li>Nuitka：将脚本、模块、包编译成可执行文件或扩展模块。<a href="http://nuitka.net/">官网</a></li>
<li>py2app：将 Python 脚本变为独立软件包（Mac OS X）。<a href="http://pythonhosted.org/py2app/">官网</a></li>
<li>py2exe：将 Python 脚本变为独立软件包（Windows）。<a href="http://www.py2exe.org/">官网</a></li>
<li>pynsist：一个用来创建 Windows 安装程序的工具，可以在安装程序中打包 Python本身。<a href="http://pynsist.readthedocs.org/">官网</a></li>
</ul>
<h3><a id="user-content-构建工具" class="anchor" href="#构建工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>构建工具</h3>
<p>将源码编译成软件。</p>
<ul>
<li>buildout：一个构建系统，从多个组件来创建，组装和部署应用。<a href="http://www.buildout.org/">官网</a></li>
<li>BitBake：针对嵌入式 Linux 的类似 make 的构建工具。<a href="http://www.yoctoproject.org/docs/1.6/bitbake-user-manual/bitbake-user-manual.html">官网</a></li>
<li>fabricate：对任何语言自动找到依赖关系的构建工具。<a href="https://code.google.com/archive/p/fabricate">官网</a></li>
<li>PlatformIO：多平台命令行构建工具。<a href="https://github.com/platformio/platformio">官网</a></li>
<li>PyBuilder：纯 Python 实现的持续化构建工具。<a href="https://github.com/pybuilder/pybuilder">官网</a></li>
<li>SCons：软件构建工具。<a href="http://www.scons.org/">官网</a></li>
</ul>
<h3><a id="user-content-交互式解析器" class="anchor" href="#交互式解析器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>交互式解析器</h3>
<p>交互式 Python 解析器。</p>
<ul>
<li>IPython：功能丰富的工具，非常有效的使用交互式 Python。<a href="https://github.com/ipython/ipython">官网</a></li>
<li><a href="http://hao.jobbole.com/bpython/">bpython</a>：界面丰富的 Python 解析器。<a href="http://bpython-interpreter.org/">官网</a></li>
<li>ptpython：高级交互式Python解析器， 构建于<a href="https://github.com/jonathanslenders/python-prompt-toolkit">python-prompt-toolkit</a> 之上。<a href="https://github.com/jonathanslenders/ptpython">官网</a></li>
</ul>
<h3><a id="user-content-文件" class="anchor" href="#文件" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>文件</h3>
<p>文件管理和 MIME（多用途的网际邮件扩充协议）类型检测。</p>
<ul>
<li>imghdr：（Python 标准库）检测图片类型。<a href="https://docs.python.org/2/library/imghdr.html">官网</a></li>
<li>mimetypes：（Python 标准库）将文件名映射为 MIME 类型。<a href="https://docs.python.org/2/library/mimetypes.html">官网</a></li>
<li>path.py：对 os.path 进行封装的模块。<a href="https://github.com/jaraco/path.py">官网</a></li>
<li>pathlib：（Python3.4+ 标准库）跨平台的、面向对象的路径操作库。<a href="https://pathlib.readthedocs.org/en/pep428/">官网</a></li>
<li>python-magic：文件类型检测的第三方库 libmagic 的 Python 接口。<a href="https://github.com/ahupp/python-magic">官网</a></li>
<li>Unipath：用面向对象的方式操作文件和目录。<a href="https://github.com/mikeorr/Unipath">官网</a></li>
<li>watchdog：管理文件系统事件的 API 和 shell 工具<a href="https://github.com/gorakhargosh/watchdog">官网</a></li>
</ul>
<h3><a id="user-content-日期和时间" class="anchor" href="#日期和时间" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>日期和时间</h3>
<p>操作日期和时间的类库。</p>
<ul>
<li>arrow：更好的 Python 日期时间操作类库。<a href="https://github.com/crsmithdev/arrow">官网</a></li>
<li>Chronyk：Python 3 的类库，用于解析手写格式的时间和日期。<a href="https://github.com/KoffeinFlummi/Chronyk">官网</a></li>
<li>dateutil：Python datetime 模块的扩展。<a href="https://pypi.python.org/pypi/python-dateutil">官网</a></li>
<li>delorean：解决 Python 中有关日期处理的棘手问题的库。<a href="https://github.com/myusuf3/delorean/">官网</a></li>
<li>moment：一个用来处理时间和日期的Python库。灵感来自于Moment.js。<a href="https://github.com/zachwill/moment">官网</a></li>
<li>PyTime：一个简单易用的Python模块，用于通过字符串来操作日期/时间。<a href="https://github.com/shinux/PyTime">官网</a></li>
<li>pytz：现代以及历史版本的世界时区定义。将时区数据库引入Python。<a href="https://launchpad.net/pytz">官网</a></li>
<li>when.py：提供用户友好的函数来帮助用户进行常用的日期和时间操作。<a href="https://github.com/dirn/When.py">官网</a></li>
</ul>
<h3><a id="user-content-文本处理" class="anchor" href="#文本处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>文本处理</h3>
<p>用于解析和操作文本的库。</p>
<ul>
<li>通用
<ul>
<li><a href="http://hao.jobbole.com/chardet/">chardet</a>：字符编码检测器，兼容 Python2 和 Python3。<a href="https://github.com/chardet/chardet">官网</a></li>
<li>difflib：(Python 标准库)帮助我们进行差异化比较。<a href="https://docs.python.org/2/library/difflib.html">官网</a></li>
<li>ftfy：让Unicode文本更完整更连贯。<a href="https://github.com/LuminosoInsight/python-ftfy">官网</a></li>
<li>fuzzywuzzy：模糊字符串匹配。<a href="https://github.com/seatgeek/fuzzywuzzy">官网</a></li>
<li>Levenshtein：快速计算编辑距离以及字符串的相似度。<a href="https://github.com/ztane/python-Levenshtein/">官网</a></li>
<li>pangu.py：在中日韩语字符和数字字母之间添加空格。<a href="https://github.com/vinta/pangu.py">官网</a></li>
<li>yfiglet-figlet：<a href="https://github.com/pwaller/pyfiglet">pyfiglet -figlet</a> 的 Python实现。</li>
<li>shortuuid：一个生成器库，用以生成简洁的，明白的，URL 安全的 UUID。<a href="https://github.com/stochastic-technologies/shortuuid">官网</a></li>
<li>unidecode：Unicode 文本的 ASCII 转换形式 。<a href="https://pypi.python.org/pypi/Unidecode">官网</a></li>
<li>uniout：打印可读的字符，而不是转义的字符串。<a href="https://github.com/moskytw/uniout">官网</a></li>
<li>xpinyin：一个用于把汉字转换为拼音的库。<a href="https://github.com/lxneng/xpinyin">官网</a></li>
<li>simplejson：Python的JSON编码、解码器。<a href="https://simplejson.readthedocs.io/en/latest/">官网</a>、<a href="https://github.com/simplejson/simplejson">GitHub</a></li>
</ul>
</li>
<li>Slug化
<ul>
<li>awesome-slugify：一个 Python slug 化库，可以保持 Unicode。<a href="https://github.com/dimka665/awesome-slugify">官网</a></li>
<li>python-slugify：Python slug 化库，可以把 unicode 转化为 ASCII。<a href="https://github.com/un33k/python-slugify">官网</a></li>
<li>unicode-slugify：一个 slug 工具，可以生成 unicode slugs ,需要依赖 Django 。<a href="https://github.com/mozilla/unicode-slugify">官网</a></li>
</ul>
</li>
<li>解析器
<ul>
<li>phonenumbers：解析，格式化，储存，验证电话号码。<a href="https://github.com/daviddrysdale/python-phonenumbers">官网</a></li>
<li>PLY：lex 和 yacc 解析工具的 Python 实现。<a href="http://www.dabeaz.com/ply/">官网</a></li>
<li>Pygments：通用语法高亮工具。<a href="http://pygments.org/">官网</a></li>
<li>pyparsing：生成通用解析器的框架。<a href="http://pyparsing.wikispaces.com/">官网</a></li>
<li>python-nameparser：把一个人名分解为几个独立的部分。<a href="https://github.com/derek73/python-nameparser">官网</a></li>
<li>python-user-agents：浏览器 user agent 解析器。<a href="https://github.com/selwin/python-user-agents">官网</a></li>
<li>sqlparse：一个无验证的 SQL 解析器。<a href="https://sqlparse.readthedocs.org/en/latest/">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-特殊文本格式处理" class="anchor" href="#特殊文本格式处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>特殊文本格式处理</h3>
<p>一些用来解析和操作特殊文本格式的库。</p>
<ul>
<li>通用
<ul>
<li>tablib：一个用来处理中表格数据的模块。<a href="https://github.com/kennethreitz/tablib">官网</a></li>
</ul>
</li>
<li>Office
<ul>
<li>Marmir：把输入的Python 数据结构转换为电子表单。<a href="https://github.com/brianray/mm">官网</a></li>
<li>openpyxl：一个用来读写 Excel 2010 xlsx/xlsm/xltx/xltm 文件的库。<a href="https://openpyxl.readthedocs.org/en/latest/">官网</a></li>
<li>python-docx：读取，查询以及修改 Microsoft Word 2007/2008 docx 文件。<a href="https://github.com/python-openxml/python-docx">官网</a></li>
<li>unoconv：在 LibreOffice/OpenOffice 支持的任意文件格式之间进行转换。<a href="https://github.com/dagwieers/unoconv">官网</a></li>
<li>XlsxWriter：一个用于创建 Excel .xlsx 文件的 Python 模块。<a href="https://xlsxwriter.readthedocs.org/en/latest/">官网</a></li>
<li>xlwings：一个使得在 Excel 中方便调用 Python 的库（反之亦然），基于 BSD 协议。<a href="http://xlwings.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/xlwt/">xlwt</a>：读写 Excel 文件的数据和格式信息。<a href="https://github.com/python-excel/xlwt">官网</a> / <a href="https://github.com/python-excel/xlrd">xlrd</a></li>
<li>relatorio：模板化OpenDocument 文件。<a href="http://relatorio.tryton.org/">官网</a></li>
</ul>
</li>
<li>PDF
<ul>
<li>PDFMiner：一个用于从PDF文档中抽取信息的工具。<a href="https://github.com/euske/pdfminer">官网</a></li>
<li>PyPDF2：一个可以分割，合并和转换 PDF 页面的库。<a href="https://github.com/mstamy2/PyPDF2">官网</a></li>
<li>ReportLab：快速创建富文本 PDF 文档。<a href="http://www.reportlab.com/opensource/">官网</a></li>
</ul>
</li>
<li>Markdown
<ul>
<li>Mistune：快速并且功能齐全的纯 Python 实现的 Markdown 解析器。<a href="https://github.com/lepture/mistune">官网</a></li>
<li>Python-Markdown：John Gruber’s Markdown 的 Python 版实现。<a href="https://github.com/waylan/Python-Markdown">官网</a></li>
<li>Python-Markdown2：纯 Python 实现的 Markdown 解析器，比 Python-Markdown 更快，更准确，可扩展。<a href="https://github.com/trentm/python-markdown2">官网</a></li>
</ul>
</li>
<li>YAML
<ul>
<li>PyYAML：Python 版本的 YAML 解析器。<a href="http://pyyaml.org/">官网</a></li>
</ul>
</li>
<li>CSV
<ul>
<li>csvkit：用于转换和操作 CSV 的工具。<a href="https://github.com/wireservice/csvkit">官网</a></li>
</ul>
</li>
<li>Archive
<ul>
<li>unp：一个用来方便解包归档文件的命令行工具。<a href="https://github.com/mitsuhiko/unp">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-自然语言处理" class="anchor" href="#自然语言处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>自然语言处理</h3>
<p>用来处理人类语言的库。</p>
<ul>
<li><a href="http://hao.jobbole.com/nltk/">NLTK</a>：一个先进的平台，用以构建处理人类语言数据的 Python 程序。<a href="http://www.nltk.org/">官网</a></li>
<li>jieba：中文分词工具。<a href="https://github.com/fxsjy/jieba">官网</a></li>
<li>langid.py：独立的语言识别系统。<a href="https://github.com/saffsd/langid.py">官网</a></li>
<li>Pattern：Python 网络信息挖掘模块。<a href="http://www.clips.ua.ac.be/pattern">官网</a></li>
<li>SnowNLP：一个用来处理中文文本的库。<a href="https://github.com/isnowfy/snownlp">官网</a></li>
<li>TextBlob：为进行普通自然语言处理任务提供一致的 API。<a href="http://textblob.readthedocs.org/en/latest/">官网</a></li>
<li>TextGrocery：一简单高效的短文本分类工具，基于 LibLinear 和 Jieba。<a href="https://github.com/2shou/TextGrocery">官网</a></li>
</ul>
<h3><a id="user-content-文档" class="anchor" href="#文档" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>文档</h3>
<p>用以生成项目文档的库。</p>
<ul>
<li><a href="http://hao.jobbole.com/sphinx/">Sphinx</a>：Python 文档生成器。<a href="http://www.sphinx-doc.org/en/latest/">官网</a>
<ul>
<li>awesome-sphinxdoc：<a href="https://github.com/yoloseem/awesome-sphinxdoc">官网</a></li>
</ul>
</li>
<li>MkDocs：对 Markdown 友好的文档生成器。<a href="http://www.mkdocs.org/">官网</a></li>
<li>pdoc：一个可以替换Epydoc 的库，可以自动生成 Python 库的 API 文档。<a href="https://github.com/BurntSushi/pdoc">官网</a></li>
<li>Pycco：文学编程（literate-programming）风格的文档生成器。<a href="https://github.com/pycco-docs/pycco">官网</a></li>
</ul>
<h3><a id="user-content-配置" class="anchor" href="#配置" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>配置</h3>
<p>用来保存和解析配置的库。</p>
<ul>
<li>config：<a href="https://docs.python.org/2/library/logging.html">logging</a> 模块作者写的分级配置模块。<a href="https://www.red-dove.com/config-doc/">官网</a></li>
<li>ConfigObj：INI 文件解析器，带验证功能。<a href="http://www.voidspace.org.uk/python/configobj.html">官网</a></li>
<li>ConfigParser：(Python 标准库) INI 文件解析器。<a href="https://docs.python.org/2/library/configparser.html">官网</a></li>
<li>profig：通过多种格式进行配置，具有数值转换功能。<a href="http://profig.readthedocs.org/en/default/">官网</a></li>
<li>python-decouple：将设置和代码完全隔离。<a href="https://github.com/henriquebastos/python-decouple">官网</a></li>
</ul>
<h3><a id="user-content-命令行工具" class="anchor" href="#命令行工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>命令行工具</h3>
<p>用于创建命令行程序的库。</p>
<ul>
<li>命令行程序开发
<ul>
<li>asciimatics：跨平台，全屏终端包（即鼠标/键盘输入和彩色，定位文本输出），完整的复杂动画和特殊效果的高级API。<a href="https://github.com/peterbrittain/asciimatics">官网</a></li>
<li>cement：Python 的命令行程序框架。<a href="http://builtoncement.com/">官网</a></li>
<li>click：一个通过组合的方式来创建精美命令行界面的包。<a href="http://click.pocoo.org/dev/">官网</a></li>
<li>cliff：一个用于创建命令行程序的框架，可以创建具有多层命令的命令行程序。<a href="http://docs.openstack.org/developer/cliff/">官网</a></li>
<li>clint：Python 命令行程序工具。<a href="https://github.com/kennethreitz/clint">官网</a></li>
<li>colorama：跨平台彩色终端文本。<a href="https://pypi.python.org/pypi/colorama">官网</a></li>
<li>docopt：Python 风格的命令行参数解析器。<a href="http://docopt.org/">官网</a></li>
<li>Gooey：一条命令，将命令行程序变成一个 GUI 程序。<a href="https://github.com/chriskiehl/Gooey">官网</a></li>
<li>python-prompt-toolkit：一个用于构建强大的交互式命令行程序的库。<a href="https://github.com/jonathanslenders/python-prompt-toolkit">官网</a></li>
<li><a href="http://hao.jobbole.com/pythonpy/">Pythonpy</a>：在命令行中直接执行任何Python指令。<a href="https://github.com/Russell91/pythonpy/wiki">官网</a></li>
</ul>
</li>
<li>生产力工具
<ul>
<li>aws-cli：Amazon Web Services 的通用命令行界面。<a href="https://github.com/aws/aws-cli">官网</a></li>
<li>bashplotlib：在终端中进行基本绘图。<a href="https://github.com/glamp/bashplotlib">官网</a></li>
<li>caniusepython3：判断是哪个项目妨碍你你移植到 Python 3。<a href="https://github.com/brettcannon/caniusepython3">官网</a></li>
<li>cookiecutter：从 cookiecutters（项目模板）创建项目的一个命令行工具。<a href="https://github.com/audreyr/cookiecutter">官网</a></li>
<li>doitlive：一个用来在终端中进行现场演示的工具。<a href="https://github.com/sloria/doitlive">官网</a></li>
<li>howdoi：通过命令行获取即时的编程问题解答。<a href="https://github.com/gleitz/howdoi">官网</a></li>
<li>httpie：一个命令行HTTP 客户端，cURL 的替代品，易用性更好。<a href="https://github.com/jkbrzt/httpie">官网</a></li>
<li>PathPicker：从bash输出中选出文件。<a href="https://github.com/facebook/PathPicker">官网</a></li>
<li>percol：向UNIX shell 传统管道概念中加入交互式选择功能。<a href="https://github.com/mooz/percol">官网</a></li>
<li>SAWS：一个加强版的 AWS 命令行。<a href="https://github.com/donnemartin/saws">官网</a></li>
<li>thefuck：修正你之前的命令行指令。<a href="https://github.com/nvbn/thefuck">官网</a></li>
<li>mycli：一个 MySQL 命令行客户端，具有自动补全和语法高亮功能。<a href="https://github.com/dbcli/mycli">官网</a></li>
<li>pgcli：Postgres 命令行工具，具有自动补全和语法高亮功能。<a href="https://github.com/dbcli/pgcli">官网</a></li>
<li>try：一个从来没有更简单的命令行工具，用来试用python库。<a href="https://github.com/timofurrer/try">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-下载器" class="anchor" href="#下载器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>下载器</h3>
<p>用来进行下载的库.</p>
<ul>
<li>s3cmd：一个用来管理Amazon S3 和 CloudFront 的命令行工具。<a href="https://github.com/s3tools/s3cmd">官网</a></li>
<li>s4cmd：超级 S3 命令行工具，性能更加强劲。<a href="https://github.com/bloomreach/s4cmd">官网</a></li>
<li>you-get：一个 YouTube/Youku/Niconico 视频下载器，使用 Python3 编写。<a href="https://www.soimort.org/you-get/">官网</a></li>
<li>youtube-dl：一个小巧的命令行程序，用来下载 YouTube 视频。<a href="http://rg3.github.io/youtube-dl/">官网</a></li>
</ul>
<h3><a id="user-content-图像处理" class="anchor" href="#图像处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>图像处理</h3>
<p>用来操作图像的库.</p>
<ul>
<li><a href="http://hao.jobbole.com/pillow/">pillow</a>：Pillow 是一个更加易用版的 <a href="http://www.pythonware.com/products/pil/">PIL</a>。<a href="http://pillow.readthedocs.org/en/latest/">官网</a></li>
<li>hmap：图像直方图映射。<a href="https://github.com/rossgoodwin/hmap">官网</a></li>
<li>imgSeek：一个使用视觉相似性搜索一组图片集合的项目。<a href="https://sourceforge.net/projects/imgseek/">官网</a></li>
<li>nude.py：裸体检测。<a href="https://github.com/hhatto/nude.py">官网</a></li>
<li>pyBarcode：不借助 PIL 库在 Python 程序中生成条形码。<a href="https://pythonhosted.org/pyBarcode/">官网</a></li>
<li>pygram：类似 Instagram 的图像滤镜。<a href="https://github.com/ajkumar25/pygram">官网</a></li>
<li>python-qrcode：一个纯 Python 实现的二维码生成器。<a href="https://github.com/lincolnloop/python-qrcode">官网</a></li>
<li>Quads：基于四叉树的计算机艺术。<a href="https://github.com/fogleman/Quads">官网</a></li>
<li>scikit-image：一个用于（科学）图像处理的 Python 库。<a href="http://scikit-image.org/">官网</a></li>
<li>thumbor：一个小型图像服务，具有剪裁，尺寸重设和翻转功能。<a href="https://github.com/thumbor/thumbor">官网</a></li>
<li>wand：<a href="http://www.imagemagick.org/script/magick-wand.php">MagickWand</a>的Python 绑定。MagickWand 是 ImageMagick的 C API 。<a href="https://github.com/dahlia/wand">官网</a></li>
</ul>
<h3><a id="user-content-ocr" class="anchor" href="#ocr" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>OCR</h3>
<p>光学字符识别库。</p>
<ul>
<li>pyocr：Tesseract 和 Cuneiform 的一个封装(wrapper)。<a href="https://github.com/jflesch/pyocr">官网</a></li>
<li><a href="http://hao.jobbole.com/pytesseract/">pytesseract</a>：<a href="https://github.com/tesseract-ocr">Google Tesseract OCR</a> 的另一个封装(wrapper)。<a href="https://github.com/madmaze/pytesseract">官网</a></li>
<li>python-tesseract - <a href="https://github.com/tesseract-ocr">Google Tesseract OCR</a> 的一个包装类。</li>
</ul>
<h3><a id="user-content-音频" class="anchor" href="#音频" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>音频</h3>
<p>用来操作音频的库</p>
<ul>
<li>audiolazy：Python 的数字信号处理包。<a href="https://github.com/danilobellini/audiolazy">官网</a></li>
<li>audioread：交叉库 (GStreamer + Core Audio + MAD + FFmpeg) 音频解码。<a href="https://github.com/beetbox/audioread">官网</a></li>
<li>beets：一个音乐库管理工具及 <a href="https://musicbrainz.org/">MusicBrainz</a> 标签添加工具<a href="http://beets.io/">官网</a></li>
<li>dejavu：音频指纹提取和识别<a href="https://github.com/worldveil/dejavu">官网</a></li>
<li><a href="http://hao.jobbole.com/django-elastic-transcoder/">django-elastic-transcoder</a>：Django + <a href="http://aws.amazon.com/elastictranscoder/">Amazon Elastic Transcoder</a>。<a href="https://github.com/StreetVoice/django-elastic-transcoder">官网</a></li>
<li>eyeD3：一个用来操作音频文件的工具，具体来讲就是包含 ID3 元信息的 MP3 文件。<a href="http://eyed3.nicfit.net/">官网</a></li>
<li>id3reader：一个用来读取 MP3 元数据的 Python 模块。<a href="http://nedbatchelder.com/code/modules/id3reader.py">官网</a></li>
<li>m3u8：一个用来解析 m3u8 文件的模块。<a href="https://github.com/globocom/m3u8">官网</a></li>
<li>mutagen：一个用来处理音频元数据的 Python 模块。<a href="https://bitbucket.org/lazka/mutagen">官网</a></li>
<li>pydub：通过简单、简洁的高层接口来操作音频文件。<a href="https://github.com/jiaaro/pydub">官网</a></li>
<li>pyechonest：<a href="http://developer.echonest.com/">Echo Nest</a> API 的 Python 客户端<a href="https://github.com/echonest/pyechonest">官网</a></li>
<li>talkbox：一个用来处理演讲/信号的 Python 库<a href="http://scikits.appspot.com/talkbox">官网</a></li>
<li>TimeSide：开源 web 音频处理框架。<a href="https://github.com/Parisson/TimeSide">官网</a></li>
<li>tinytag：一个用来读取MP3, OGG, FLAC 以及 Wave 文件音乐元数据的库。<a href="https://github.com/devsnd/tinytag">官网</a></li>
<li>mingus：一个高级音乐理论和曲谱包，支持 MIDI 文件和回放功能。<a href="http://bspaans.github.io/python-mingus/">官网</a></li>
</ul>
<h3><a id="user-content-video" class="anchor" href="#video" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Video</h3>
<p>用来操作视频和GIF的库。</p>
<ul>
<li>moviepy：一个用来进行基于脚本的视频编辑模块，适用于多种格式，包括动图 GIFs。<a href="http://zulko.github.io/moviepy/">官网</a></li>
<li>scikit-video：SciPy 视频处理常用程序。<a href="https://github.com/aizvorski/scikit-video">官网</a></li>
</ul>
<h3><a id="user-content-地理位置" class="anchor" href="#地理位置" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>地理位置</h3>
<p>地理编码地址以及用来处理经纬度的库。</p>
<ul>
<li>GeoDjango：世界级地理图形 web 框架。<a href="https://docs.djangoproject.com/en/dev/ref/contrib/gis/">官网</a></li>
<li>GeoIP：MaxMind GeoIP Legacy 数据库的 Python API。<a href="https://github.com/maxmind/geoip-api-python">官网</a></li>
<li>geojson：GeoJSON 的 Python 绑定及工具。<a href="https://github.com/frewsxcv/python-geojson">官网</a></li>
<li>geopy：Python 地址编码工具箱。<a href="https://github.com/geopy/geopy">官网</a></li>
<li>pygeoip：纯 Python GeoIP API。<a href="https://github.com/appliedsec/pygeoip">官网</a></li>
<li>django-countries：一个 Django 应用程序，提供用于表格的国家选择功能，国旗图标静态文件以及模型中的国家字段。<a href="https://github.com/SmileyChris/django-countries">官网</a></li>
</ul>
<h3><a id="user-content-http" class="anchor" href="#http" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>HTTP</h3>
<p>使用HTTP的库。</p>
<ul>
<li>requests：人性化的HTTP请求库。<a href="http://docs.python-requests.org/en/latest/">官网</a></li>
<li>grequests：requests 库 + gevent ，用于异步 HTTP 请求.<a href="https://github.com/kennethreitz/grequests">官网</a></li>
<li>httplib2：全面的 HTTP 客户端库。<a href="https://github.com/jcgregorio/httplib2">官网</a></li>
<li>treq：类似 requests 的Python API 构建于 Twisted HTTP 客户端之上。<a href="https://github.com/twisted/treq">官网</a></li>
<li>urllib3：一个具有线程安全连接池，支持文件 post，清晰友好的 HTTP 库。<a href="https://github.com/shazow/urllib3">官网</a></li>
</ul>
<h3><a id="user-content-数据库" class="anchor" href="#数据库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据库</h3>
<p>Python实现的数据库。</p>
<ul>
<li>pickleDB：一个简单，轻量级键值储存数据库。<a href="https://pythonhosted.org/pickleDB/">官网</a></li>
<li>PipelineDB：流式 SQL 数据库。<a href="https://www.pipelinedb.com/">官网</a></li>
<li>TinyDB：一个微型的，面向文档型数据库。<a href="https://github.com/msiemens/tinydb">官网</a></li>
<li>ZODB：一个 Python 原生对象数据库。一个键值和对象图数据库。<a href="http://www.zodb.org/en/latest/">官网</a></li>
</ul>
<h3><a id="user-content-数据库驱动" class="anchor" href="#数据库驱动" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据库驱动</h3>
<p>用来连接和操作数据库的库。</p>
<ul>
<li>MySQL：<a href="http://shlomi-noach.github.io/awesome-mysql/">awesome-mysql</a>系列
<ul>
<li>mysql-python：Python 的 MySQL 数据库连接器。<a href="https://sourceforge.net/projects/mysql-python/">官网</a></li>
<li>ysqlclient：<a href="https://github.com/PyMySQL/mysqlclient-python">mysql-python</a> 分支，支持 Python 3。</li>
<li>oursql：一个更好的 MySQL 连接器，支持原生预编译指令和 BLOBs.<a href="https://pythonhosted.org/oursql/">官网</a></li>
<li>PyMySQL：纯 Python MySQL 驱动，兼容 mysql-python。<a href="https://github.com/PyMySQL/PyMySQL">官网</a></li>
</ul>
</li>
<li>PostgreSQL
<ul>
<li>psycopg2：Python 中最流行的 PostgreSQL 适配器。<a href="http://initd.org/psycopg/">官网</a></li>
<li>queries：psycopg2 库的封装，用来和 PostgreSQL 进行交互。<a href="https://github.com/gmr/queries">官网</a></li>
<li>txpostgres：基于 Twisted 的异步 PostgreSQL 驱动。<a href="http://txpostgres.readthedocs.org/en/latest/">官网</a></li>
</ul>
</li>
<li>其他关系型数据库
<ul>
<li>apsw：另一个 Python SQLite封装。<a href="http://rogerbinns.github.io/apsw/">官网</a></li>
<li>dataset：在数据库中存储Python字典</li>
<li>pymssql：一个简单的Microsoft SQL Server数据库接口。<a href="http://www.pymssql.org/en/latest/">官网</a></li>
</ul>
</li>
<li>NoSQL 数据库
<ul>
<li>cassandra-python-driver：Cassandra 的 Python 驱动。<a href="https://github.com/datastax/python-driver">官网</a></li>
<li>HappyBase：一个为 Apache HBase 设计的，对开发者友好的库。<a href="http://happybase.readthedocs.org/en/latest/">官网</a></li>
<li>Plyvel：一个快速且功能丰富的 LevelDB 的 Python 接口。<a href="https://plyvel.readthedocs.org/en/latest/">官网</a></li>
<li>py2neo：Neo4j restful 接口的Python 封装客户端。<a href="http://py2neo.org/2.0/">官网</a></li>
<li>pycassa：Cassandra 的 Python Thrift 驱动。<a href="https://github.com/pycassa/pycassa">官网</a></li>
<li>PyMongo：MongoDB 的官方 Python 客户端。<a href="https://docs.mongodb.org/ecosystem/drivers/python/">官网</a></li>
<li>redis-py：Redis 的 Python 客户端。<a href="https://github.com/andymccurdy/redis-py">官网</a></li>
<li>telephus：基于 Twisted 的 Cassandra 客户端。<a href="https://github.com/driftx/Telephus">官网</a></li>
<li>txRedis：基于 Twisted 的 Redis 客户端。<a href="https://github.com/deldotdr/txRedis">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-orm" class="anchor" href="#orm" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>ORM</h3>
<p>实现对象关系映射或数据映射技术的库。</p>
<ul>
<li>关系型数据库
<ul>
<li>Django Models：Django 的一部分。<a href="https://docs.djangoproject.com/en/dev/topics/db/models/">官网</a></li>
<li>SQLAlchemy：Python SQL 工具以及对象关系映射工具。<a href="http://www.sqlalchemy.org/">官网</a>
<ul>
<li><a href="https://github.com/dahlia/awesome-sqlalchemy">awesome-sqlalchemy</a>系列</li>
</ul>
</li>
<li><a href="http://hao.jobbole.com/peewee/">Peewee</a>：一个小巧，富有表达力的 ORM。<a href="https://github.com/coleifer/peewee">官网</a></li>
<li>PonyORM：提供面向生成器的 SQL 接口的 ORM。<a href="https://ponyorm.com/">官网</a></li>
<li>python-sql：编写 Python 风格的 SQL 查询。<a href="https://pypi.python.org/pypi/python-sql">官网</a></li>
</ul>
</li>
<li>NoSQL 数据库
<ul>
<li>django-mongodb-engine：Django MongoDB 后端。<a href="https://github.com/django-nonrel/mongodb-engine">官网</a></li>
<li>PynamoDB：<a href="https://aws.amazon.com/dynamodb/">Amazon DynamoDB</a> 的一个 Python 风格接口。<a href="https://github.com/jlafon/PynamoDB">官网</a></li>
<li>flywheel：Amazon DynamoDB 的对象映射工具。<a href="https://github.com/mathcamp/flywheel">官网</a></li>
<li>MongoEngine：一个Python 对象文档映射工具，用于 MongoDB。<a href="http://mongoengine.org/">官网</a></li>
<li>hot-redis：为 Redis 提供 Python 丰富的数据类型。<a href="https://github.com/stephenmcd/hot-redis">官网</a></li>
<li>redisco：一个 Python 库，提供可以持续存在在 Redis 中的简单模型和容器。<a href="https://github.com/kiddouk/redisco">官网</a></li>
</ul>
</li>
<li>其他
<ul>
<li>butterdb：Google Drive 电子表格的 Python ORM。<a href="https://github.com/Widdershin/butterdb">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-web-框架" class="anchor" href="#web-框架" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Web 框架</h3>
<p>全栈 Web 框架。</p>
<ul>
<li><a href="http://hao.jobbole.com/django/">Django</a>：Python 界最流行的 web 框架。<a href="https://www.djangoproject.com/">官网</a>
<ul>
<li><a href="https://gitlab.com/rosarior/awesome-django">awesome-django</a>系列</li>
</ul>
</li>
<li><a href="http://hao.jobbole.com/flask/">Flask</a>：一个 Python 微型框架。<a href="http://flask.pocoo.org/">官网</a>
<ul>
<li><a href="https://github.com/humiaozuzu/awesome-flask">awesome-flask</a>系列</li>
</ul>
</li>
<li>pyramid：一个小巧，快速，接地气的开源Python web 框架。
<ul>
<li><a href="https://github.com/uralbash/awesome-pyramid">awesome-pyramid</a>系列</li>
</ul>
</li>
<li><a href="http://hao.jobbole.com/bottle/">Bottle</a>：一个快速小巧，轻量级的 WSGI 微型 web 框架。<a href="http://bottlepy.org/docs/dev/index.html">官网</a></li>
<li>CherryPy：一个极简的 Python web 框架，服从 HTTP/1.1 协议且具有WSGI 线程池。<a href="http://www.cherrypy.org/">官网</a></li>
<li>TurboGears：一个可以扩展为全栈解决方案的微型框架。<a href="http://www.turbogears.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/python-webpy/">web.py</a>：一个 Python 的 web 框架，既简单，又强大。<a href="http://webpy.org/">官网</a></li>
<li>web2py：一个全栈 web 框架和平台，专注于简单易用。<a href="http://www.web2py.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/tornado/">Tornado</a>：一个web 框架和异步网络库。<a href="http://www.tornadoweb.org/en/latest/">官网</a></li>
</ul>
<h3><a id="user-content-权限" class="anchor" href="#权限" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>权限</h3>
<p>允许或拒绝用户访问数据或功能的库。</p>
<ul>
<li>Carteblanche：Module to align code with thoughts of users and designers. Also magically handles navigation and permissions.<a href="https://github.com/neuman/python-carteblanche/">官网</a></li>
<li>django-guardian：Django 1.2+ 实现了单个对象权限。<a href="https://github.com/django-guardian/django-guardian">官网</a></li>
<li>django-rules：一个小巧但是强大的应用，提供对象级别的权限管理，且不需要使用数据库。<a href="https://github.com/dfunckt/django-rules">官网</a></li>
</ul>
<h3><a id="user-content-cms" class="anchor" href="#cms" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>CMS</h3>
<p>内容管理系统</p>
<ul>
<li>odoo-cms: 一个开源的，企业级 CMS，基于odoo。<a href="http://www.odoo.com">官网</a></li>
<li>django-cms：一个开源的，企业级 CMS，基于 Django。<a href="http://www.django-cms.org/en/">官网</a></li>
<li>djedi-cms：一个轻量级但却非常强大的 Django CMS ，考虑到了插件，内联编辑以及性能。<a href="http://djedi-cms.org/">官网</a></li>
<li>FeinCMS：基于 Django 构建的最先进的内容管理系统之一。<a href="http://www.feincms.org/">官网</a></li>
<li>Kotti：一个高级的，Python 范的 web 应用框架，基于 Pyramid 构建。<a href="http://kotti.pylonsproject.org/">官网</a></li>
<li>Mezzanine：一个强大的，持续的，灵活的内容管理平台。<a href="http://mezzanine.jupo.org/">官网</a></li>
<li>Opps：一个为杂志，报纸网站以及大流量门户网站设计的 CMS 平台，基于 Django。<a href="http://opps.github.io/opps/">官网</a></li>
<li>Plone：一个构建于开源应用服务器 Zope 之上的 CMS。<a href="https://plone.org/">官网</a></li>
<li>Quokka：灵活，可扩展的小型 CMS，基于 Flask 和 MongoDB。<a href="http://quokkaproject.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/wagtail/">Wagtail</a>：一个 Django 内容管理系统。<a href="https://wagtail.io/">官网</a></li>
<li>Widgy：最新的 CMS 框架，基于 Django。<a href="https://wid.gy/">官网</a></li>
</ul>
<h3><a id="user-content-电子商务" class="anchor" href="#电子商务" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>电子商务</h3>
<p>用于电子商务以及支付的框架和库。</p>
<ul>
<li>django-oscar：一个用于 Django 的开源的电子商务框架。<a href="http://oscarcommerce.com/">官网</a></li>
<li>django-shop：一个基于 Django 的店铺系统。<a href="https://github.com/awesto/django-shop">官网</a></li>
<li>Cartridge：一个基于 Mezzanine 构建的购物车应用。<a href="https://github.com/stephenmcd/cartridge">官网</a></li>
<li>shoop：一个基于 Django 的开源电子商务平台。<a href="https://www.shoop.io/en/">官网</a></li>
<li>alipay：非官方的 Python 支付宝 API。<a href="https://github.com/lxneng/alipay">官网</a></li>
<li>merchant：一个可以接收来自多种支付平台支付的 Django 应用。<a href="https://github.com/agiliq/merchant">官网</a></li>
<li>money：货币类库with optional CLDR-backed locale-aware formatting and an extensible currency exchange solution.<a href="https://github.com/carlospalol/money">官网</a></li>
<li>python-currencies：显示货币格式以及它的数值。<a href="https://github.com/Alir3z4/python-currencies">官网</a></li>
</ul>
<h3><a id="user-content-restful-api" class="anchor" href="#restful-api" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>RESTful API</h3>
<p>用来开发RESTful APIs的库</p>
<ul>
<li>Django
<ul>
<li><a href="http://hao.jobbole.com/django-rest-framework/">django-rest-framework</a>：一个强大灵活的工具，用来构建 web API。<a href="http://www.django-rest-framework.org/">官网</a></li>
<li>django-tastypie：为Django 应用开发API。<a href="http://tastypieapi.org/">官网</a></li>
<li>django-formapi：为 Django 的表单验证，创建 JSON APIs 。<a href="https://github.com/5monkeys/django-formapi">官网</a></li>
</ul>
</li>
<li>Flask
<ul>
<li>flask-api：为 flask 开发的，可浏览 Web APIs 。<a href="http://www.flaskapi.org/">官网</a></li>
<li>flask-restful：为 flask 快速创建REST APIs 。<a href="http://flask-restful.readthedocs.org/en/latest/">官网</a></li>
<li>flask-restless：为 SQLAlchemy 定义的数据库模型创建 RESTful APIs 。<a href="https://flask-restless.readthedocs.org/en/latest/">官网</a></li>
<li>flask-api-utils：为 Flask 处理 API 表示和验证。<a href="https://github.com/marselester/flask-api-utils">官网</a></li>
<li>eve：REST API 框架，由 Flask, MongoDB 等驱动。<a href="https://github.com/nicolaiarocci/eve">官网</a></li>
</ul>
</li>
<li>Pyramid
<ul>
<li>cornice：一个Pyramid 的 REST 框架 。<a href="https://cornice.readthedocs.org/en/latest/">官网</a></li>
</ul>
</li>
<li>与框架无关的
<ul>
<li>falcon：一个用来建立云 API 和 web app 后端的高性能框架。<a href="http://falconframework.org/">官网</a></li>
<li>sandman：为现存的数据库驱动系统自动创建 REST APIs 。<a href="https://github.com/jeffknupp/sandman">官网</a></li>
<li>restless：框架无关的 REST 框架 ，基于从 Tastypie 学到的知识。<a href="http://restless.readthedocs.org/en/latest/">官网</a></li>
<li>ripozo：快速创建 REST/HATEOAS/Hypermedia APIs。<a href="https://github.com/vertical-knowledge/ripozo">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-验证" class="anchor" href="#验证" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>验证</h3>
<p>实现验证方案的库。</p>
<ul>
<li>OAuth
<ul>
<li>Authomatic：简单但是强大的框架，身份验证/授权客户端。<a href="http://peterhudec.github.io/authomatic/">官网</a></li>
<li>django-allauth：Django 的验证应用。<a href="https://github.com/pennersr/django-allauth">官网</a></li>
<li>django-oauth-toolkit：为 Django 用户准备的 OAuth2。<a href="https://github.com/evonove/django-oauth-toolkit">官网</a></li>
<li>django-oauth2-provider：为 Django 应用提供 OAuth2 接入。<a href="https://github.com/caffeinehit/django-oauth2-provider">官网</a></li>
<li>Flask-OAuthlib：OAuth 1.0/a, 2.0 客户端实现，供 Flask 使用。<a href="https://github.com/lepture/flask-oauthlib">官网</a></li>
<li>OAuthLib：一个 OAuth 请求-签名逻辑通用、 完整的实现。<a href="https://github.com/idan/oauthlib">官网</a></li>
<li>python-oauth2：一个完全测试的抽象接口。用来创建 OAuth 客户端和服务端。<a href="https://github.com/joestump/python-oauth2">官网</a></li>
<li>python-social-auth：一个设置简单的社会化验证方式。<a href="https://github.com/omab/python-social-auth">官网</a></li>
<li>rauth：OAuth 1.0/a, 2.0, 和 Ofly 的 Python 库。<a href="https://github.com/litl/rauth">官网</a></li>
<li>sanction：一个超级简单的OAuth2 客户端实现。<a href="https://github.com/demianbrecht/sanction">官网</a></li>
</ul>
</li>
<li>其他
<ul>
<li>jose：JavaScript 对象签名和加密草案的实现。<a href="https://github.com/demonware/jose">官网</a></li>
<li>PyJWT：JSON Web 令牌草案 01。<a href="https://github.com/jpadilla/pyjwt">官网</a></li>
<li>python-jws：JSON Web 签名草案 02 的实现。<a href="https://github.com/brianloveswords/python-jws">官网</a></li>
<li>python-jwt：一个用来生成和验证 JSON Web 令牌的模块。<a href="https://github.com/davedoesdev/python-jwt">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-模板引擎" class="anchor" href="#模板引擎" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>模板引擎</h3>
<p>模板生成和词法解析的库和工具。</p>
<ul>
<li><a href="http://hao.jobbole.com/jinja2/">Jinja2</a>：一个现代的，对设计师友好的模板引擎。<a href="https://github.com/pallets/jinja">官网</a></li>
<li>Chameleon：一个 HTML/XML 模板引擎。 模仿了 ZPT（Zope Page Templates）, 进行了速度上的优化。<a href="https://chameleon.readthedocs.org/en/latest/">官网</a></li>
<li>Genshi：Python 模板工具，用以生成 web 感知的结果。<a href="https://genshi.edgewall.org/">官网</a></li>
<li>Mako：Python 平台的超高速轻量级模板。<a href="http://www.makotemplates.org/">官网</a></li>
</ul>
<h3><a id="user-content-queue" class="anchor" href="#queue" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Queue</h3>
<p>处理事件以及任务队列的库。</p>
<ul>
<li>celery：一个异步任务队列/作业队列，基于分布式消息传递。<a href="http://www.celeryproject.org/">官网</a></li>
<li>huey：小型多线程任务队列。<a href="https://github.com/coleifer/huey">官网</a></li>
<li><a href="http://hao.jobbole.com/mrq/">mrq</a>：Mr. Queue -一个 Python 的分布式 worker 任务队列， 使用 Redis 和 gevent。<a href="https://github.com/pricingassistant/mrq">官网</a></li>
<li>rq：简单的 Python 作业队列。<a href="http://python-rq.org/">官网</a></li>
<li>simpleq：一个简单的，可无限扩张的，基于亚马逊 SQS 的队列。<a href="https://github.com/rdegges/simpleq">官网</a></li>
</ul>
<h3><a id="user-content-搜索" class="anchor" href="#搜索" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>搜索</h3>
<p>对数据进行索引和执行搜索查询的库和软件。</p>
<ul>
<li>django-haystack：Django 模块化搜索。<a href="https://github.com/django-haystack/django-haystack">官网</a></li>
<li>elasticsearch-py：Elasticsearch 的官方底层 Python 客户端。<a href="https://www.elastic.co/guide/en/elasticsearch/client/python-api/current/index.html">官网</a></li>
<li>elasticsearch-dsl-py：Elasticsearch 的官方高级 Python 客户端。<a href="https://github.com/elastic/elasticsearch-dsl-py">官网</a></li>
<li>solrpy：<a href="http://lucene.apache.org/solr/">solr</a>的 Python 客户端。<a href="https://github.com/edsu/solrpy">官网</a></li>
<li>Whoosh：一个快速的纯 Python 搜索引擎库。<a href="http://whoosh.readthedocs.org/en/latest/">官网</a></li>
</ul>
<h3><a id="user-content-动态消息" class="anchor" href="#动态消息" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>动态消息</h3>
<p>用来创建用户活动的库。</p>
<ul>
<li>django-activity-stream：从你的站点行为中生成通用活动信息流。<a href="https://github.com/justquick/django-activity-stream">官网</a></li>
<li>Stream-Framework：使用 Cassandra 和 Redis 创建动态消息和通知系统。<a href="https://github.com/tschellenbach/Stream-Framework">官网</a></li>
</ul>
<h3><a id="user-content-资源管理" class="anchor" href="#资源管理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>资源管理</h3>
<p>管理、压缩、缩小网站资源的工具。</p>
<ul>
<li>django-compressor：将链接和内联的 JavaScript 或 CSS 压缩到一个单独的缓存文件中。<a href="https://github.com/django-compressor/django-compressor">官网</a></li>
<li>django-storages：一个针对 Django 的自定义存储后端的工具集合。<a href="http://django-storages.readthedocs.org/en/latest/">官网</a></li>
<li>fanstatic：打包、优化，并且把静态文件依赖作为 Python 的包来提供。<a href="http://www.fanstatic.org/en/latest/">官网</a></li>
<li>File Conveyor：一个后台驻留的程序，用来发现和同步文件到 CDNs, S3 和 FTP。<a href="http://fileconveyor.org/">官网</a></li>
<li>Flask-Assets：帮你将 web 资源整合到你的 Flask app 中。<a href="http://flask-assets.readthedocs.org/en/latest/">官网</a></li>
<li>jinja-assets-compressor：一个 Jinja 扩展，用来编译和压缩你的资源。<a href="https://github.com/jaysonsantos/jinja-assets-compressor">官网</a></li>
<li>webassets：为你的静态资源打包、优化和管理生成独一无二的缓存 URL。<a href="http://webassets.readthedocs.org/en/latest/">官网</a></li>
</ul>
<h3><a id="user-content-缓存" class="anchor" href="#缓存" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>缓存</h3>
<p>缓存数据的库。</p>
<ul>
<li>Beaker：一个缓存和会话库，可以用在 web 应用和独立 Python脚本和应用上。<a href="http://beaker.readthedocs.org/en/latest/">官网</a></li>
<li>django-cache-machine：Django 模型的自动缓存和失效。<a href="https://github.com/django-cache-machine/django-cache-machine">官网</a></li>
<li>django-cacheops：具有自动颗粒化事件驱动失效功能的 ORM。<a href="https://github.com/Suor/django-cacheops">官网</a></li>
<li>django-viewlet：渲染模板，同时具有额外的缓存控制功能。<a href="https://github.com/5monkeys/django-viewlet">官网</a></li>
<li>dogpile.cache：dogpile.cache 是 Beaker 的下一代替代品，由同一作者开发。<a href="http://dogpilecache.readthedocs.org/en/latest/">官网</a></li>
<li>HermesCache：Python 缓存库，具有基于标签的失效和 dogpile effect 保护功能。<a href="https://pypi.python.org/pypi/HermesCache">官网</a></li>
<li>johnny-cache：django应用缓存框架。<a href="https://github.com/jmoiron/johnny-cache">官网</a></li>
<li>pylibmc：<a href="http://libmemcached.org/libMemcached.html">libmemcached</a> 接口的 Python 封装。<a href="https://github.com/lericson/pylibmc">官网</a></li>
</ul>
<h3><a id="user-content-电子邮件" class="anchor" href="#电子邮件" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>电子邮件</h3>
<p>用来发送和解析电子邮件的库。</p>
<ul>
<li>django-celery-ses：带有 AWS SES 和 Celery 的 Django email 后端。<a href="https://github.com/StreetVoice/django-celery-ses">官网</a></li>
<li>envelopes：供人类使用的电子邮件库。<a href="http://tomekwojcik.github.io/envelopes/">官网</a></li>
<li>flanker：一个 email 地址和 Mime 解析库。<a href="https://github.com/mailgun/flanker">官网</a></li>
<li>imbox：Python IMAP 库<a href="https://github.com/martinrusev/imbox">官网</a></li>
<li>inbox.py：Python SMTP 服务器。<a href="https://github.com/kennethreitz/inbox.py">官网</a></li>
<li>inbox：一个开源电子邮件工具箱。<a href="https://github.com/nylas/sync-engine">官网</a></li>
<li>lamson：Python 风格的 SMTP 应用服务器。<a href="https://github.com/zedshaw/lamson">官网</a></li>
<li>mailjet：Mailjet API 实现，用来提供批量发送邮件，统计等功能。<a href="https://github.com/WoLpH/mailjet">官网</a></li>
<li>marrow.mailer：高性能可扩展邮件分发框架。<a href="https://github.com/marrow/mailer">官网</a></li>
<li>modoboa：一个邮件托管和管理平台，具有现代的、简约的 Web UI。<a href="https://github.com/tonioo/modoboa">官网</a></li>
<li>pyzmail：创建，发送和解析电子邮件。<a href="http://www.magiksys.net/pyzmail/">官网</a></li>
<li>Talon：Mailgun 库，用来抽取信息和签名。<a href="https://github.com/mailgun/talon">官网</a></li>
</ul>
<h3><a id="user-content-国际化" class="anchor" href="#国际化" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>国际化</h3>
<p>用来进行国际化的库。</p>
<ul>
<li>Babel：一个Python 的国际化库。<a href="http://babel.pocoo.org/en/latest/">官网</a></li>
<li>Korean：一个韩语词态库。<a href="https://korean.readthedocs.org/en/latest/">官网</a></li>
</ul>
<h3><a id="user-content-url处理" class="anchor" href="#url处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>URL处理</h3>
<p>解析URLs的库</p>
<ul>
<li>furl：一个让处理 URL 更简单小型 Python 库。<a href="https://github.com/gruns/furl">官网</a></li>
<li>purl：一个简单的，不可变的URL类，具有简洁的 API 来进行询问和处理。<a href="https://github.com/codeinthehole/purl">官网</a></li>
<li>pyshorteners：一个纯 Python URL 缩短库。<a href="https://github.com/ellisonleao/pyshorteners">官网</a></li>
<li>shorturl：生成短小 URL 和类似 bit.ly 短链的Python 实现。<a href="https://github.com/Alir3z4/python-shorturl">官网</a></li>
<li>webargs：一个解析 HTTP 请求参数的库，内置对流行 web 框架的支持，包括 Flask, Django, Bottle, Tornado和 Pyramid。<a href="https://github.com/sloria/webargs">官网</a></li>
</ul>
<h3><a id="user-content-html处理" class="anchor" href="#html处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>HTML处理</h3>
<p>处理 HTML和XML的库。</p>
<ul>
<li>BeautifulSoup：以 Python 风格的方式来对 HTML 或 XML 进行迭代，搜索和修改。<a href="http://www.crummy.com/software/BeautifulSoup/bs4/doc/">官网</a></li>
<li>bleach：一个基于白名单的 HTML 清理和文本链接库。<a href="http://bleach.readthedocs.org/en/latest/">官网</a></li>
<li>cssutils：一个 Python 的 CSS 库。<a href="https://pypi.python.org/pypi/cssutils/">官网</a></li>
<li>html5lib：一个兼容标准的 HTML 文档和片段解析及序列化库。<a href="https://github.com/html5lib/html5lib-python">官网</a></li>
<li>lxml：一个非常快速，简单易用，功能齐全的库，用来处理 HTML 和 XML。<a href="http://lxml.de/">官网</a></li>
<li>MarkupSafe：为Python 实现 XML/HTML/XHTML 标记安全字符串。<a href="https://github.com/pallets/markupsafe">官网</a></li>
<li>pyquery：一个解析 HTML 的库，类似 jQuery。<a href="https://github.com/gawel/pyquery">官网</a></li>
<li>untangle：将XML文档转换为Python对象，使其可以方便的访问。<a href="https://github.com/stchris/untangle">官网</a></li>
<li>xhtml2pdf：HTML/CSS 转 PDF 工具。<a href="https://github.com/xhtml2pdf/xhtml2pdf">官网</a></li>
<li>xmltodict：像处理 JSON 一样处理 XML。<a href="https://github.com/martinblech/xmltodict">官网</a></li>
</ul>
<p>爬取网络站点的库</p>
<ul>
<li>Scrapy：一个快速高级的屏幕爬取及网页采集框架。<a href="http://scrapy.org/">官网</a></li>
<li>cola：一个分布式爬虫框架。<a href="https://github.com/chineking/cola">官网</a></li>
<li>Demiurge：基于PyQuery 的爬虫微型框架。<a href="https://github.com/matiasb/demiurge">官网</a></li>
<li>feedparser：通用 feed 解析器。<a href="http://pythonhosted.org/feedparser/">官网</a></li>
<li>Grab：站点爬取框架。<a href="http://grablib.org/">官网</a></li>
<li>MechanicalSoup：用于自动和网络站点交互的 Python 库。<a href="https://github.com/hickford/MechanicalSoup">官网</a></li>
<li>portia：Scrapy 可视化爬取。<a href="https://github.com/scrapinghub/portia">官网</a></li>
<li>pyspider：一个强大的爬虫系统。<a href="https://github.com/binux/pyspider">官网</a></li>
<li>RoboBrowser：一个简单的，Python 风格的库，用来浏览网站，而不需要一个独立安装的浏览器。<a href="https://github.com/jmcarp/robobrowser">官网</a></li>
</ul>
<h3><a id="user-content-网页内容提取" class="anchor" href="#网页内容提取" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>网页内容提取</h3>
<p>用于进行网页内容提取的库。</p>
<ul>
<li>Haul：一个可以扩展的图像爬取工具。<a href="https://github.com/vinta/Haul">官网</a></li>
<li>html2text：将 HTML 转换为 Markdown 格式文本<a href="https://github.com/Alir3z4/html2text">官网</a></li>
<li>lassie：人性化的网页内容检索库。<a href="https://github.com/michaelhelmick/lassie">官网</a></li>
<li>micawber：一个小型网页内容提取库，用来从 URLs 提取富内容。<a href="https://github.com/coleifer/micawber">官网</a></li>
<li><a href="http://hao.jobbole.com/python-newspaper/">newspaper</a>：使用 Python 进行新闻提取，文章提取以及内容策展。<a href="https://github.com/codelucas/newspaper">官网</a></li>
<li>opengraph：一个用来解析开放内容协议(Open Graph Protocol)的 Python模块。<a href="https://github.com/erikriver/opengraph">官网</a></li>
<li><a href="http://hao.jobbole.com/python-goose/">python-goose</a>：HTML内容/文章提取器。<a href="https://github.com/grangier/python-goose">官网</a></li>
<li>python-readability：arc90 公司 readability 工具的 Python 高速端口。<a href="https://github.com/buriy/python-readability">官网</a></li>
<li>sanitize：为杂乱的数据世界带来调理性。<a href="https://github.com/Alir3z4/python-sanitize">官网</a></li>
<li>sumy：一个为文本文件和 HTML 页面进行自动摘要的模块。<a href="https://github.com/miso-belica/sumy">官网</a></li>
<li>textract：从任何格式的文档中提取文本，Word，PowerPoint，PDFs 等等。<a href="https://github.com/deanmalmgren/textract">官网</a></li>
</ul>
<h3><a id="user-content-表单" class="anchor" href="#表单" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>表单</h3>
<p>进行表单操作的库。</p>
<ul>
<li>Deform：Python HTML 表单生成库，受到了 formish 表单生成库的启发。<a href="http://deform.readthedocs.org/en/latest/">官网</a></li>
<li>django-bootstrap3：集成了 Bootstrap 3 的 Django。<a href="https://github.com/dyve/django-bootstrap3">官网</a></li>
<li>django-crispy-forms：一个 Django 应用，他可以让你以一种非常优雅且 DRY（Don't repeat yourself） 的方式来创建美观的表单。<a href="http://django-crispy-forms.readthedocs.org/en/latest/">官网</a></li>
<li>django-remote-forms：一个平台独立的 Django 表单序列化工具。<a href="https://github.com/WiserTogether/django-remote-forms">官网</a></li>
<li>WTForms：一个灵活的表单验证和呈现库。<a href="http://wtforms.readthedocs.org/en/latest/">官网</a></li>
<li>WTForms-JSON：一个 WTForms 扩展，用来处理 JSON 数据。<a href="http://wtforms-json.readthedocs.org/en/latest/">官网</a></li>
</ul>
<h3><a id="user-content-数据验证" class="anchor" href="#数据验证" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据验证</h3>
<p>数据验证库。多用于表单验证。</p>
<ul>
<li>Cerberus：A mappings-validator with a variety of rules, normalization-features and simple customization that uses a pythonic schema-definition.<a href="http://docs.python-cerberus.org/en/stable/">官网</a></li>
<li>colander：一个用于对从 XML, JSON，HTML 表单获取的数据或其他同样简单的序列化数据进行验证和反序列化的系统。<a href="http://docs.pylonsproject.org/projects/colander/en/latest/">官网</a></li>
<li>kmatch：一种用于匹配/验证/筛选 Python 字典的语言。<a href="https://github.com/ambitioninc/kmatch">官网</a></li>
<li>schema：一个用于对 Python 数据结构进行验证的库。<a href="https://github.com/keleshev/schema">官网</a></li>
<li>Schematics：数据结构验证。<a href="https://github.com/schematics/schematics">官网</a></li>
<li>valideer：轻量级可扩展的数据验证和适配库。<a href="https://github.com/podio/valideer">官网</a></li>
<li>voluptuous：一个 Python 数据验证库。主要是为了验证传入 Python的 JSON，YAML 等数据。<a href="https://github.com/alecthomas/voluptuous">官网</a></li>
</ul>
<h3><a id="user-content-反垃圾技术" class="anchor" href="#反垃圾技术" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>反垃圾技术</h3>
<p>帮助你和电子垃圾进行战斗的库。</p>
<ul>
<li>django-simple-captcha：一个简单、高度可定制的Django 应用，可以为任何Django表单添加验证码。<a href="https://github.com/mbi/django-simple-captcha">官网</a></li>
<li>django-simple-spam-blocker：一个用于Django的简单的电子垃圾屏蔽工具。<a href="https://github.com/moqada/django-simple-spam-blocker">官网</a></li>
</ul>
<h3><a id="user-content-标记" class="anchor" href="#标记" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>标记</h3>
<p>用来进行标记的库。</p>
<ul>
<li>django-taggit：简单的 Django 标记工具。<a href="https://github.com/alex/django-taggit">官网</a></li>
</ul>
<h3><a id="user-content-管理面板" class="anchor" href="#管理面板" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>管理面板</h3>
<p>管理界面库。</p>
<ul>
<li>Ajenti：一个你的服务器值得拥有的管理面板。<a href="https://github.com/Eugeny/ajenti">官网</a></li>
<li>django-suit：Django 管理界面的一个替代品 (仅对于非商业用途是免费的)。<a href="http://djangosuit.com/">官网</a></li>
<li>django-xadmin：Django admin 的一个替代品，具有很多不错的功能。<a href="https://github.com/sshwsfc/django-xadmin">官网</a></li>
<li>flask-admin：一个用于 Flask 的简单可扩展的管理界面框架。<a href="https://github.com/flask-admin/flask-admin">官网</a></li>
<li>flower：一个对 Celery 集群进行实时监控和提供 web 管理界面的工具。<a href="https://github.com/mher/flower">官网</a></li>
<li>Grappelli：Django 管理界面的一个漂亮的皮肤。<a href="http://grappelliproject.com/">官网</a></li>
<li>Wooey：一个 Django 应用，可以为 Python 脚本创建 web 用户界面。<a href="https://github.com/wooey/wooey">官网</a></li>
</ul>
<h3><a id="user-content-静态站点生成器" class="anchor" href="#静态站点生成器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>静态站点生成器</h3>
<p>静态站点生成器是一个软件，它把文本和模板作为输入，然后输出HTML文件。</p>
<ul>
<li>Pelican：使用 Markdown 或 ReST 来处理内容， Jinja 2 来制作主题。支持 DVCS, Disqus.。AGPL 许可。<a href="http://blog.getpelican.com/">官网</a></li>
<li>Cactus：为设计师设计的静态站点生成器。<a href="https://github.com/koenbok/Cactus/">官网</a></li>
<li>Hyde：基于 Jinja2 的静态站点生成器。<a href="http://hyde.github.io/">官网</a></li>
<li>Nikola：一个静态网站和博客生成器。<a href="https://www.getnikola.com/">官网</a></li>
<li>Tinkerer：Tinkerer 是一个博客引擎/静态站点生成器，由Sphinx驱动。<a href="http://tinkerer.me/">官网</a></li>
<li>Lektor：一个简单易用的静态 CMS 和博客引擎。<a href="https://www.getlektor.com/">官网</a></li>
</ul>
<h3><a id="user-content-进程" class="anchor" href="#进程" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>进程</h3>
<p>操作系统进程启动及通信库。</p>
<ul>
<li>envoy：比 Python <a href="https://docs.python.org/2/library/subprocess.html">subprocess</a> 模块更人性化。<a href="https://github.com/kennethreitz/envoy">官网</a></li>
<li>sarge：另一 种 subprocess 模块的封装。<a href="http://sarge.readthedocs.org/en/latest/">官网</a></li>
<li>sh：一个完备的 subprocess 替代库。<a href="https://github.com/amoffat/sh">官网</a></li>
</ul>
<h3><a id="user-content-并发和并行" class="anchor" href="#并发和并行" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>并发和并行</h3>
<p>用以进行并发和并行操作的库。</p>
<ul>
<li>multiprocessing：(Python 标准库) 基于进程的“线程”接口。<a href="https://docs.python.org/2/library/multiprocessing.html">官网</a></li>
<li>threading：(Python 标准库)更高层的线程接口。<a href="https://docs.python.org/2/library/threading.html">官网</a></li>
<li>eventlet：支持 WSGI 的异步框架。<a href="http://eventlet.net/">官网</a></li>
<li>gevent：一个基于协程的 Python 网络库，使用<a href="https://github.com/python-greenlet/greenlet">greenlet</a>。<a href="http://www.gevent.org/">官网</a></li>
<li>Tomorrow：用于产生异步代码的神奇的装饰器语法实现。<a href="https://github.com/madisonmay/Tomorrow">官网</a></li>
<li>uvloop：在libuv之上超快速实现asyncio事件循环。<a href="https://github.com/MagicStack/uvloop">官网</a></li>
</ul>
<h3><a id="user-content-网络" class="anchor" href="#网络" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>网络</h3>
<p>用于网络编程的库。</p>
<ul>
<li>asyncio：(Python 标准库) 异步 I/O, 事件循环, 协程以及任务。<a href="https://docs.python.org/3/library/asyncio.html">官网</a></li>
<li><a href="http://hao.jobbole.com/twisted/">Twisted</a>：一个事件驱动的网络引擎。<a href="https://twistedmatrix.com/trac/">官网</a></li>
<li>pulsar：事件驱动的并发框架。<a href="https://github.com/quantmind/pulsar">官网</a></li>
<li>diesel：基于Greenlet 的事件 I/O 框架。<a href="https://github.com/dieseldev/diesel">官网</a></li>
<li>pyzmq：一个 ZeroMQ 消息库的 Python 封装。<a href="http://zeromq.github.io/pyzmq/">官网</a></li>
<li>txZMQ：基于 Twisted 的 ZeroMQ 消息库的 Python 封装。<a href="https://github.com/smira/txZMQ">官网</a></li>
</ul>
<h3><a id="user-content-websocket" class="anchor" href="#websocket" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>WebSocket</h3>
<p>帮助使用WebSocket的库。</p>
<ul>
<li>AutobahnPython：给 Python 、使用的 WebSocket &amp; WAMP 基于 Twisted 和 <a href="https://docs.python.org/3/library/asyncio.html">asyncio</a>。<a href="https://github.com/crossbario/autobahn-python">官网</a></li>
<li>Crossbar：开源统一应用路由(Websocket &amp; WAMP for Python on Autobahn).<a href="https://github.com/crossbario/crossbar/">官网</a></li>
<li>django-socketio：给 Django 用的 WebSockets。<a href="https://github.com/stephenmcd/django-socketio">官网</a></li>
<li>WebSocket-for-Python：为Python2/3 以及 PyPy 编写的 WebSocket 客户端和服务器库。<a href="https://github.com/Lawouach/WebSocket-for-Python">官网</a></li>
</ul>
<h3><a id="user-content-wsgi-服务器" class="anchor" href="#wsgi-服务器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>WSGI 服务器</h3>
<p>兼容 WSGI 的 web 服务器</p>
<ul>
<li>gunicorn：Pre-forked, 部分是由 C 语言编写的。<a href="https://pypi.python.org/pypi/gunicorn">官网</a></li>
<li>uwsgi：uwsgi 项目的目的是开发一组全栈工具，用来建立托管服务， 由 C 语言编写。<a href="https://uwsgi-docs.readthedocs.org/en/latest/">官网</a></li>
<li><a href="http://hao.jobbole.com/bjoern/">bjoern</a>：异步，非常快速，由 C 语言编写。<a href="https://pypi.python.org/pypi/bjoern">官网</a></li>
<li>fapws3：异步 (仅对于网络端)，由 C 语言编写。<a href="http://www.fapws.org/">官网</a></li>
<li>meinheld：异步，部分是由 C 语言编写的。<a href="https://pypi.python.org/pypi/meinheld">官网</a></li>
<li>netius：异步，非常快速。<a href="https://github.com/hivesolutions/netius">官网</a></li>
<li>paste：多线程，稳定，久经考验。<a href="http://pythonpaste.org/">官网</a></li>
<li>rocket：多线程。<a href="https://pypi.python.org/pypi/rocket">官网</a></li>
<li>waitress：多线程, 是它驱动着 Pyramid 框架。<a href="https://waitress.readthedocs.org/en/latest/">官网</a></li>
<li>Werkzeug：一个 WSGI 工具库，驱动着 Flask ，而且可以很方便大嵌入到你的项目中去。<a href="http://werkzeug.pocoo.org/">官网</a></li>
</ul>
<h3><a id="user-content-rpc-服务器" class="anchor" href="#rpc-服务器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>RPC 服务器</h3>
<p>兼容 RPC 的服务器。</p>
<ul>
<li>SimpleJSONRPCServer：这个库是 JSON-RPC 规范的一个实现。<a href="https://github.com/joshmarshall/jsonrpclib/">官网</a></li>
<li>SimpleXMLRPCServer：(Python 标准库) 简单的 XML-RPC 服务器实现，单线程。<a href="https://docs.python.org/2/library/simplexmlrpcserver.html">官网</a></li>
<li>zeroRPC：zerorpc 是一个灵活的 RPC 实现，基于 ZeroMQ 和 MessagePack。<a href="https://github.com/0rpc/zerorpc-python">官网</a></li>
</ul>
<h3><a id="user-content-密码学" class="anchor" href="#密码学" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>密码学</h3>
<ul>
<li>cryptography：这个软件包意在提供密码学基本内容和方法提供给 Python 开发者。<a href="https://cryptography.io/en/latest/">官网</a></li>
<li>hashids：在 Python 中实现 <a href="http://hashids.org/">hashids</a> 。<a href="https://github.com/davidaurelio/hashids-python">官网</a></li>
<li>Paramiko：SSHv2 协议的 Python (2.6+, 3.3+) ，提供客户端和服务端的功能。<a href="http://www.paramiko.org/">官网</a></li>
<li>Passlib：安全密码存储／哈希库，<a href="https://pythonhosted.org/passlib/">官网</a></li>
<li>PyCrypto：Python 密码学工具箱。<a href="https://www.dlitz.net/software/pycrypto/">官网</a></li>
<li>PyNacl：网络和密码学(NaCl) 库的 Python 绑定。<a href="https://github.com/pyca/pynacl">官网</a></li>
</ul>
<h3><a id="user-content-图形用户界面" class="anchor" href="#图形用户界面" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>图形用户界面</h3>
<p>用来创建图形用户界面程序的库。</p>
<ul>
<li>curses：内建的 <a href="http://www.gnu.org/software/ncurses/">ncurses</a> 封装，用来创建终端图形用户界面。<a href="https://docs.python.org/2/library/curses.html#module-curses">官网</a></li>
<li>enaml：使用类似 QML 的Declaratic语法来创建美观的用户界面。<a href="https://github.com/nucleic/enaml">官网</a></li>
<li><a href="http://hao.jobbole.com/kivy/">kivy</a>：一个用来创建自然用户交互（NUI）应用程序的库，可以运行在 Windows, Linux, Mac OS X, Android 以及 iOS平台上。<a href="https://kivy.org/">官网</a></li>
<li>pyglet：一个Python 的跨平台窗口及多媒体库。<a href="https://bitbucket.org/pyglet/pyglet/wiki/Home">官网</a></li>
<li>PyQt：跨平台用户界面框架 <a href="http://www.qt.io/">Qt</a> 的 Python 绑定 ，支持Qt v4 和 Qt v5。<a href="https://riverbankcomputing.com/software/pyqt/intro">官网</a></li>
<li>PySide：P跨平台用户界面框架 <a href="http://www.qt.io/">Qt</a> 的 Python 绑定 ，支持Qt v4。<a href="https://wiki.qt.io/PySide">官网</a></li>
<li>Tkinter：Tkinter 是 Python GUI 的一个事实标准库。<a href="https://wiki.python.org/moin/TkInter">官网</a></li>
<li>Toga：一个 Python 原生的, 操作系统原生的 GUI 工具包。<a href="https://github.com/pybee/toga">官网</a></li>
<li>urwid：一个用来创建终端 GUI 应用的库，支持组件，事件和丰富的色彩等。<a href="http://urwid.org/">官网</a></li>
<li>wxPython：wxPython 是 wxWidgets C++ 类库和 Python 语言混合的产物。<a href="http://wxpython.org/">官网</a></li>
<li>PyGObject：GLib/GObject/GIO/GTK+ (GTK+3) 的 Python 绑定<a href="https://wiki.gnome.org/Projects/PyGObject">官网</a></li>
<li>Flexx：Flexx 是一个纯 Python 语言编写的用来创建 GUI 程序的工具集，它使用 web 技术进行界面的展示。<a href="https://github.com/zoofIO/flexx">官网</a></li>
</ul>
<h3><a id="user-content-游戏开发" class="anchor" href="#游戏开发" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>游戏开发</h3>
<p>超赞的游戏开发库。</p>
<ul>
<li>Cocos2d：cocos2d 是一个用来开发 2D 游戏， 示例和其他图形/交互应用的框架。基于 pyglet。<a href="http://cocos2d.org/">官网</a></li>
<li>Panda3D：由迪士尼开发的 3D 游戏引擎，并由卡内基梅陇娱乐技术中心负责维护。使用C++编写, 针对 Python 进行了完全的封装。<a href="https://www.panda3d.org/">官网</a></li>
<li>Pygame：Pygame 是一组 Python 模块，用来编写游戏。<a href="http://www.pygame.org/news.html">官网</a></li>
<li>PyOgre：Ogre 3D 渲染引擎的 Python 绑定，可以用来开发游戏和仿真程序等任何 3D 应用。<a href="http://www.ogre3d.org/tikiwiki/PyOgre">官网</a></li>
<li>PyOpenGL：OpenGL 的 Python 绑定及其相关 APIs。<a href="http://pyopengl.sourceforge.net/">官网</a></li>
<li>PySDL2：SDL2 库的封装，基于 ctypes。<a href="http://pysdl2.readthedocs.org/en/latest/">官网</a></li>
<li>RenPy：一个视觉小说（visual novel）引擎。<a href="https://www.renpy.org/">官网</a></li>
</ul>
<h3><a id="user-content-日志" class="anchor" href="#日志" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>日志</h3>
<p>用来生成和操作日志的库。</p>
<ul>
<li>logging：(Python 标准库) 为 Python 提供日志功能。<a href="https://docs.python.org/2/library/logging.html">官网</a></li>
<li>logbook：Logging 库的替代品。<a href="http://pythonhosted.org/Logbook/">官网</a></li>
<li>Eliot：为复杂的和分布式系统创建日志。<a href="https://eliot.readthedocs.org/en/latest/">官网</a></li>
<li>Raven：Sentry的 Python 客户端。<a href="http://raven.readthedocs.org/en/latest/">官网</a></li>
<li>Sentry：实时记录和收集日志的服务器。<a href="https://pypi.python.org/pypi/sentry">官网</a></li>
</ul>
<h3><a id="user-content-testing" class="anchor" href="#testing" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Testing</h3>
<p>进行代码库测试和生成测试数据的库。</p>
<ul>
<li>测试框架
<ul>
<li>unittest：(Python 标准库) 单元测试框架。<a href="https://docs.python.org/2/library/unittest.html">官网</a></li>
<li>nose：nose 扩展了 unittest 的功能。<a href="https://nose.readthedocs.org/en/latest/">官网</a></li>
<li>contexts：一个 Python 3.3+ 的 BDD 框架。受到C# – Machine.Specifications的启发。<a href="https://github.com/benjamin-hodgson/Contexts">官网</a></li>
<li>hypothesis：Hypothesis 是一个基于先进的 Quickcheck 风格特性的测试库。<a href="https://github.com/DRMacIver/hypothesis">官网</a></li>
<li>mamba：Python 的终极测试工具， 拥护BDD。<a href="http://nestorsalceda.github.io/mamba/">官网</a></li>
<li>PyAutoGUI：PyAutoGUI 是一个人性化的跨平台 GUI 自动测试模块。<a href="https://github.com/asweigart/pyautogui">官网</a></li>
<li>pyshould：Should 风格的断言，基于 <a href="https://github.com/hamcrest/PyHamcrest">PyHamcrest</a>。<a href="https://github.com/drslump/pyshould">官网</a></li>
<li>pytest：一个成熟的全功能 Python 测试工具。<a href="http://pytest.org/latest/">官网</a></li>
<li>green：干净，多彩的测试工具。<a href="https://github.com/CleanCut/green">官网</a></li>
<li>pyvows：BDD 风格的测试工具，受Vows.js的启发。<a href="http://heynemann.github.io/pyvows/">官网</a>-</li>
<li>Robot Framework：一个通用的自动化测试框架。<a href="https://github.com/robotframework/robotframework">官网</a></li>
</ul>
</li>
<li>Web 测试
<ul>
<li>Selenium：<a href="http://www.seleniumhq.org/">Selenium</a> WebDriver 的 Python 绑定。<a href="https://pypi.python.org/pypi/selenium">官网</a></li>
<li>locust：使用 Python 编写的，可扩展的用户加载测试工具。<a href="https://github.com/locustio/locust">官网</a></li>
<li>sixpack：一个和语言无关的 A/B 测试框架。<a href="https://github.com/seatgeek/sixpack">官网</a></li>
<li>splinter：开源的 web 应用测试工具。<a href="https://splinter.readthedocs.org/en/latest/">官网</a></li>
</ul>
</li>
<li>Mock测试
<ul>
<li>mock：(Python 标准库) 一个用于伪造测试的库。<a href="https://docs.python.org/3/library/unittest.mock.html">官网</a></li>
<li>doublex：Python 的一个功能强大的 doubles  测试框架。<a href="https://pypi.python.org/pypi/doublex">官网</a></li>
<li>freezegun：通过伪造日期模块来生成不同的时间。<a href="https://github.com/spulec/freezegun">官网</a></li>
<li>httmock：针对 Python 2.6+ 和 3.2+ 生成 伪造请求的库。<a href="https://github.com/patrys/httmock">官网</a></li>
<li>httpretty：Python 的 HTTP 请求 mock 工具。<a href="http://falcao.it/HTTPretty/">官网</a></li>
<li>responses：伪造 Python 中的 requests 库的一个通用库。<a href="https://github.com/getsentry/responses">官网</a></li>
<li>VCR.py：在你的测试中记录和重放 HTTP 交互。<a href="https://github.com/kevin1024/vcrpy">官网</a></li>
</ul>
</li>
<li>对象工厂
<ul>
<li>factoryboy：一个 Python 用的测试固件 (test fixtures) 替代库。<a href="https://github.com/rbarrois/factoryboy">官网</a></li>
<li>mixer：另外一个测试固件 (test fixtures) 替代库，支持 Django, Flask, SQLAlchemy, Peewee 等。<a href="https://github.com/klen/mixer">官网</a></li>
<li>modelmommy：为 Django 测试创建随机固件<a href="https://github.com/vandersonmota/modelmommy">官网</a></li>
</ul>
</li>
<li>代码覆盖率
<ul>
<li>coverage：代码覆盖率测量。<a href="https://pypi.python.org/pypi/coverage">官网</a></li>
</ul>
</li>
<li>伪数据
<ul>
<li>faker：一个 Python 库，用来生成伪数据。<a href="http://www.joke2k.net/faker/">官网</a></li>
<li>fake2db：伪数据库生成器。<a href="https://github.com/emirozer/fake2db">官网</a></li>
<li>radar：生成随机的日期/时间。<a href="https://pypi.python.org/pypi/radar">官网</a></li>
</ul>
</li>
<li>错误处理
<ul>
<li>FuckIt.py：FuckIt.py 使用最先进的技术来保证你的 Python 代码无论对错都能继续运行。<a href="https://github.com/ajalt/fuckitpy">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-代码分析和lint工具" class="anchor" href="#代码分析和lint工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>代码分析和Lint工具</h3>
<p>进行代码分析，解析和操作代码库的库和工具。</p>
<ul>
<li>代码分析
<ul>
<li>coala：语言独立和易于扩展的代码分析应用程序。<a href="http://coala-analyzer.org/">官网</a></li>
<li>code2flow：把你的 Python 和 JavaScript 代码转换为流程图。<a href="https://github.com/scottrogowski/code2flow">官网</a></li>
<li>pycallgraph：这个库可以把你的Python 应用的流程(调用图)进行可视化。<a href="https://github.com/gak/pycallgraph">官网</a></li>
<li>pysonar2：Python 类型推断和检索工具。<a href="https://github.com/yinwang0/pysonar2">官网</a></li>
</ul>
</li>
<li>Lint工具
<ul>
<li>Flake8：模块化源码检查工具: pep8, pyflakes 以及 co。<a href="https://pypi.python.org/pypi/flake8">官网</a></li>
<li>Pylint：一个完全可定制的源码分析器。<a href="https://www.pylint.org/">官网</a></li>
<li>YAPF: Google的Python代码格式化工具。<a href="https://github.com/google/yapf">官网</a></li>
<li>pylama：Python 和 JavaScript 的代码审查工具。<a href="https://pylama.readthedocs.org/en/latest/">官网</a></li>
</ul>
</li>
<li>代码格式化
<ul>
<li>autopep8：自动格式化 Python 代码，以使其符合 PEP8 规范。<a href="https://github.com/hhatto/autopep8">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-debugging-tools" class="anchor" href="#debugging-tools" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Debugging Tools</h3>
<p>用来进行代码调试的库。</p>
<ul>
<li>调试器
<ul>
<li>ipdb：IPython 启用的 <a href="https://docs.python.org/2/library/pdb.html">pdb</a>。<a href="https://pypi.python.org/pypi/ipdb">官网</a></li>
<li>pudb：全屏，基于控制台的 Python 调试器。<a href="https://pypi.python.org/pypi/pudb">官网</a></li>
<li>pyringe：可以在 Python 进程中附加和注入代码的调试器。<a href="https://github.com/google/pyringe">官网</a></li>
<li>wdb：一个奇异的 web 调试器，通过 WebSockets 工作。<a href="https://github.com/Kozea/wdb">官网</a></li>
<li>winpdb：一个具有图形用户界面的 Python 调试器，可以进行远程调试，基于 rpdb2。<a href="http://winpdb.org/">官网</a></li>
<li>django-debug-toolbar：为 Django 显示各种调试信息。<a href="https://github.com/django-debug-toolbar/django-debug-toolbar">官网</a></li>
<li>django-devserver：一个 Django 运行服务器的替代品。<a href="https://github.com/dcramer/django-devserver">官网</a></li>
<li>flask-debugtoolbar：django-debug-toolbar 的 flask 版。<a href="https://github.com/mgood/flask-debugtoolbar">官网</a></li>
</ul>
</li>
<li>性能分析器
<ul>
<li>lineprofiler：逐行性能分析。<a href="https://github.com/rkern/lineprofiler">官网</a></li>
<li><a href="http://hao.jobbole.com/memory_profiler/">Memory Profiler</a>：监控 Python 代码的内存使用。<a href="http://pypi.python.org/pypi/memory_profiler">官网</a>、<a href="https://github.com/fabianp/memoryprofiler">内存</a></li>
<li>profiling：一个交互式 Python 性能分析工具。<a href="https://github.com/what-studio/profiling">官网</a></li>
</ul>
</li>
<li>其他
<ul>
<li>pyelftools：解析和分析 ELF 文件以及 DWARF 调试信息。<a href="https://github.com/eliben/pyelftools">官网</a></li>
<li>python-statsd：<a href="https://github.com/etsy/statsd/">statsd</a> 服务器的 Python 客户端。<a href="https://github.com/WoLpH/python-statsd">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-science-and-data-analysis" class="anchor" href="#science-and-data-analysis" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Science and Data Analysis</h3>
<p>用来进行科学计算和数据分析的库。</p>
<ul>
<li>astropy：一个天文学 Python 库。<a href="http://www.astropy.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/bcbio-nextgen/">bcbio-nextgen</a>：这个工具箱为全自动高通量测序分析提供符合最佳实践的处理流程。<a href="https://github.com/chapmanb/bcbio-nextgen">官网</a></li>
<li>bccb：生物分析相关代码集合<a href="https://github.com/chapmanb/bcbb">官网</a></li>
<li>Biopython：Biopython 是一组可以免费使用的用来进行生物计算的工具。<a href="http://biopython.org/wiki/MainPage">官网</a></li>
<li><a href="http://hao.jobbole.com/blaze/">blaze</a>：NumPy 和 Pandas 的大数据接口。<a href="http://blaze.readthedocs.org/en/latest/index.html">官网</a></li>
<li><a href="http://hao.jobbole.com/cclib/">cclib</a>：一个用来解析和解释计算化学软件包输出结果的库。<a href="http://cclib.github.io/">官网</a></li>
<li>NetworkX：一个为复杂网络设计的高性能软件。<a href="https://networkx.github.io/">官网</a></li>
<li>Neupy：执行和测试各种不同的人工神经网络算法。<a href="http://neupy.com/pages/home.html">官网</a></li>
<li>Numba：Python JIT (just in time) 编译器，针对科学用的 Python ，由Cython 和 NumPy 的开发者开发。<a href="http://numba.pydata.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/numpy/">NumPy</a>：使用 Python 进行科学计算的基础包。<a href="http://www.numpy.org/">官网</a></li>
<li>Open Babel：一个化学工具箱，用来描述多种化学数据。<a href="http://openbabel.org/wiki/MainPage">官网</a></li>
<li><a href="http://hao.jobbole.com/open-mining/">Open Mining</a>：使用 Python 挖掘商业情报 (BI) (Pandas web 接口)。<a href="https://github.com/mining/mining">官网</a></li>
<li><a href="http://hao.jobbole.com/orange/">orange</a>：通过可视化编程或 Python 脚本进行数据挖掘，数据可视化，分析和机器学习。<a href="http://orange.biolab.si/">官网</a></li>
<li>Pandas：提供高性能，易用的数据结构和数据分析工具。<a href="http://pandas.pydata.org/">官网</a></li>
<li>PyDy：PyDy 是 Python Dynamics 的缩写，用来为动力学运动建模工作流程提供帮助， 基于 NumPy, SciPy, IPython 和 matplotlib。<a href="http://www.pydy.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/pymc/">PyMC</a>：马尔科夫链蒙特卡洛采样工具。<a href="https://github.com/pymc-devs/pymc3">官网</a></li>
<li>RDKit：化学信息学和机器学习软件。<a href="http://www.rdkit.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/scipy/">SciPy</a>：由一些基于 Python ，用于数学，科学和工程的开源软件构成的生态系统。<a href="http://www.scipy.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/statsmodels/">statsmodels</a>：统计建模和计量经济学。<a href="https://github.com/statsmodels/statsmodels">官网</a></li>
<li>SymPy：一个用于符号数学的 Python 库。<a href="https://github.com/sympy/sympy">官网</a></li>
<li>zipline：一个 Python 算法交易库。<a href="https://github.com/quantopian/zipline">官网</a></li>
<li><a href="http://hao.jobbole.com/bayesian-belief-networks/">Bayesian-belief-networks</a>：优雅的贝叶斯信念网络框架。<a href="https://github.com/eBay/bayesian-belief-networks">官网</a></li>
<li>keras: 以tensorflow或者theano为后端的深度学习封装库，快速上手神经网络<a href="https://keras.io/">官网</a></li>
</ul>
<h3><a id="user-content-数据可视化" class="anchor" href="#数据可视化" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据可视化</h3>
<p>进行数据可视化的库。 参见: <a href="https://github.com/sorrycc/awesome-javascript#data-visualization">awesome-javascript</a>。</p>
<ul>
<li>matplotlib：一个 Python 2D 绘图库。<a href="http://matplotlib.org/">官网</a></li>
<li>bokeh：用 Python 进行交互式 web 绘图。<a href="https://github.com/bokeh/bokeh">官网</a></li>
<li>ggplot：ggplot2 给 R 提供的 API 的 Python 版本。<a href="https://github.com/yhat/ggplot">官网</a></li>
<li>plotly：协同 Python 和 matplotlib 工作的 web 绘图库。<a href="https://plot.ly/python/">官网</a></li>
<li>pygal：一个 Python SVG 图表创建工具。<a href="http://www.pygal.org/en/latest/">官网</a></li>
<li>pygraphviz：Graphviz 的 Python 接口。<a href="https://pypi.python.org/pypi/pygraphviz">官网</a></li>
<li>PyQtGraph：交互式实时2D/3D/图像绘制及科学/工程学组件。<a href="http://www.pyqtgraph.org/">官网</a></li>
<li>SnakeViz：一个基于浏览器的 Python's cProfile 模块输出结果查看工具。<a href="http://jiffyclub.github.io/snakeviz/">官网</a></li>
<li>vincent：把 Python 转换为 Vega 语法的转换工具。<a href="https://github.com/wrobstory/vincent">官网</a></li>
<li>VisPy：基于 OpenGL 的高性能科学可视化工具。<a href="http://vispy.org/">官网</a></li>
</ul>
<h3><a id="user-content-计算机视觉" class="anchor" href="#计算机视觉" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>计算机视觉</h3>
<p>计算机视觉库。</p>
<ul>
<li>OpenCV：开源计算机视觉库。<a href="http://opencv.org/">官网</a></li>
<li>  pyocr：Tesseract和Cuneiform的包装库。<a href="https://github.com/jflesch/pyocr">官网</a></li>
<li>  pytesseract：<a href="https://github.com/tesseract-ocr">Google Tesseract OCR</a>的另一包装库。<a href="https://github.com/madmaze/pytesseract">官网</a></li>
<li><a href="http://hao.jobbole.com/simplecv/">SimpleCV</a>：一个用来创建计算机视觉应用的开源框架。<a href="http://simplecv.org/">官网</a></li>
</ul>
<h3><a id="user-content-机器学习" class="anchor" href="#机器学习" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>机器学习</h3>
<p>机器学习库。 参见: <a href="https://github.com/josephmisiti/awesome-machine-learning#python">awesome-machine-learning</a>.</p>
<ul>
<li>Crab：灵活、快速的推荐引擎。<a href="https://github.com/muricoca/crab">官网</a></li>
<li>gensim：人性化的话题建模库。<a href="https://github.com/piskvorky/gensim">官网</a></li>
<li>hebel：GPU 加速的深度学习库。<a href="https://github.com/hannes-brt/hebel">官网</a></li>
<li>NuPIC：智能计算 Numenta 平台。<a href="https://github.com/numenta/nupic">官网</a></li>
<li>pattern：Python 网络挖掘模块。<a href="https://github.com/clips/pattern">官网</a></li>
<li><a href="http://hao.jobbole.com/pybrain/">PyBrain</a>：另一个 Python 机器学习库。<a href="https://github.com/pybrain/pybrain">官网</a></li>
<li><a href="http://hao.jobbole.com/pylearn2/">Pylearn2</a>：一个基于 <a href="https://github.com/Theano/Theano">Theano</a> 的机器学习库。<a href="https://github.com/lisa-lab/pylearn2">官网</a></li>
<li><a href="http://hao.jobbole.com/python-recsys/">python-recsys</a>：一个用来实现推荐系统的 Python 库。<a href="https://github.com/ocelma/python-recsys">官网</a></li>
<li>scikit-learn：基于 SciPy 构建的机器学习 Python 模块。<a href="http://scikit-learn.org/">官网</a></li>
<li>pydeep：Python 深度学习库。<a href="https://github.com/andersbll/deeppy">官网</a></li>
<li>vowpalporpoise：轻量级 <a href="https://github.com/JohnLangford/vowpalwabbit/">Vowpal Wabbit</a> 的 Python 封装。<a href="https://github.com/josephreisinger/vowpalporpoise">官网</a></li>
<li>skflow：一个 <a href="https://github.com/tensorflow/tensorflow">TensorFlow</a> 的简化接口(模仿 scikit-learn)。<a href="https://github.com/tensorflow/skflow">官网</a></li>
<li>Caffe: 一个<a href="https://github.com/BVLC/caffe">Caffe</a>的python接口。<a href="http://caffe.berkeleyvision.org">官网</a></li>
</ul>
<h3><a id="user-content-mapreduce" class="anchor" href="#mapreduce" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>MapReduce</h3>
<p>MapReduce 框架和库。</p>
<ul>
<li><a href="http://hao.jobbole.com/dpark/">dpark</a>：Spark 的 Python 克隆版，一个类似 MapReduce 的框架。<a href="https://github.com/douban/dpark">官网</a></li>
<li>dumbo：这个 Python 模块可以让人轻松的编写和运行 Hadoop 程序。<a href="https://github.com/klbostee/dumbo">官网</a></li>
<li>luigi：这个模块帮你构建批处理作业的复杂流水线。<a href="https://github.com/spotify/luigi">官网</a></li>
<li>mrjob：在 Hadoop 或 Amazon Web Services 上运行 MapReduce 任务。<a href="https://github.com/Yelp/mrjob">官网</a></li>
<li>PySpark：Spark 的 Python API 。<a href="http://spark.apache.org/docs/latest/programming-guide.html">官网</a></li>
<li>streamparse：运行针对事实数据流的 Python 代码。集成了<a href="http://storm.apache.org/">Apache Storm</a>。<a href="https://github.com/Parsely/streamparse">官网</a></li>
</ul>
<h3><a id="user-content-函数式编程" class="anchor" href="#函数式编程" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>函数式编程</h3>
<p>使用 Python 进行函数式编程。</p>
<ul>
<li>CyToolz：Toolz 的 Cython 实现 : 高性能函数式工具。<a href="https://github.com/pytoolz/cytoolz/">官网</a></li>
<li>fn.py：在 Python 中进行函数式编程 : 实现了一些享受函数式编程缺失的功能。<a href="https://github.com/kachayev/fn.py">官网</a></li>
<li>funcy：炫酷又实用的函数式工具。<a href="https://github.com/Suor/funcy">官网</a></li>
<li>Toolz：一组用于迭代器，函数和字典的函数式编程工具。<a href="https://github.com/pytoolz/toolz">官网</a></li>
</ul>
<h3><a id="user-content-第三方-api" class="anchor" href="#第三方-api" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>第三方 API</h3>
<p>用来访问第三方 API的库。 参见： <a href="https://github.com/realpython/list-of-python-api-wrappers">List of Python API Wrappers and Libraries</a>。</p>
<ul>
<li>apache-libcloud：一个为各种云设计的 Python 库。<a href="https://libcloud.apache.org/">官网</a></li>
<li>boto：Amazon Web Services 的 Python 接口。<a href="https://github.com/boto/boto">官网</a></li>
<li>django-wordpress：WordPress models and views for Django.<a href="https://github.com/sunlightlabs/django-wordpress/">官网</a></li>
<li>facebook-sdk：Facebook 平台的 Python SDK.<a href="https://github.com/mobolic/facebook-sdk">官网</a></li>
<li>facepy：Facepy 让和 Facebook's Graph API 的交互变得更容易。<a href="https://github.com/jgorset/facepy">官网</a></li>
<li>gmail：Gmail 的 Python 接口。<a href="https://github.com/charlierguo/gmail">官网</a></li>
<li>google-api-python-client：Python 用的 Google APIs 客户端库。<a href="https://github.com/google/google-api-python-client">官网</a></li>
<li>gspread：Google 电子表格的 Python API.<a href="https://github.com/burnash/gspread">官网</a></li>
<li>twython：Twitter API 的封装。<a href="https://github.com/ryanmcgrath/twython">官网</a></li>
</ul>
<h3><a id="user-content-devops-工具" class="anchor" href="#devops-工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>DevOps 工具</h3>
<p>用于 DevOps 的软件和库。</p>
<ul>
<li>Ansible：一个非常简单的 IT 自动化平台。<a href="https://github.com/ansible/ansible">官网</a></li>
<li>SaltStack：基础设施自动化和管理系统。<a href="https://github.com/saltstack/salt">官网</a></li>
<li>OpenStack：用于构建私有和公有云的开源软件。<a href="http://www.openstack.org/">官网</a></li>
<li>Docker Compose：快速，分离的开发环境，使用 Docker。<a href="https://docs.docker.com/compose/">官网</a></li>
<li>Fabric：一个简单的，Python 风格的工具，用来进行远程执行和部署。<a href="http://www.fabfile.org/">官网</a></li>
<li>cuisine：为 Fabric 提供一系列高级函数。<a href="https://github.com/sebastien/cuisine">官网</a></li>
<li>Fabtools：一个用来编写超赞的 Fabric 文件的工具。<a href="https://github.com/ronnix/fabtools">官网</a></li>
<li>gitapi：Git 的纯 Python API。<a href="https://bitbucket.org/haard/gitapi">官网</a></li>
<li>hgapi：Mercurial 的纯 Python API。<a href="https://bitbucket.org/haard/hgapi">官网</a></li>
<li>honcho：<a href="https://github.com/ddollar/foreman">Foreman</a>的 Python 克隆版，用来管理基于<a href="https://devcenter.heroku.com/articles/procfile">Procfile</a>的应用。<a href="https://github.com/nickstenning/honcho">官网</a></li>
<li>pexpect：Controlling interactive programs in a pseudo-terminal like 在一个伪终端中控制交互程序，就像 GNU expect 一样。<a href="https://github.com/pexpect/pexpect">官网</a></li>
<li>psutil：一个跨平台进程和系统工具模块。<a href="https://github.com/giampaolo/psutil">官网</a></li>
<li>supervisor：UNIX 的进程控制系统。<a href="https://github.com/Supervisor/supervisor">官网</a></li>
</ul>
<h3><a id="user-content-任务调度" class="anchor" href="#任务调度" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>任务调度</h3>
<p>任务调度库。</p>
<ul>
<li>APScheduler：轻巧但强大的进程内任务调度，使你可以调度函数。<a href="http://apscheduler.readthedocs.org/en/latest/">官网</a></li>
<li>django-schedule：一个 Django 排程应用。<a href="https://github.com/thauber/django-schedule">官网</a></li>
<li>doit：一个任务执行和构建工具。<a href="http://pydoit.org/">官网</a></li>
<li>gunnery：分布式系统使用的多用途任务执行工具 ，具有 web 交互界面。<a href="https://github.com/gunnery/gunnery">官网</a></li>
<li>Joblib：一组为 Python 提供轻量级作业流水线的工具。<a href="http://pythonhosted.org/joblib/index.html">官网</a></li>
<li>Plan：如有神助地编写 crontab 文件。<a href="https://github.com/fengsp/plan">官网</a></li>
<li>schedule：人性化的 Python 任务调度库。<a href="https://github.com/dbader/schedule">官网</a></li>
<li>Spiff：使用纯 Python 实现的强大的工作流引擎。<a href="https://github.com/knipknap/SpiffWorkflow">官网</a></li>
<li>TaskFlow：一个可以让你方便执行任务的 Python 库，一致并且可靠。<a href="http://docs.openstack.org/developer/taskflow/">官网</a></li>
</ul>
<h3><a id="user-content-外来函数接口" class="anchor" href="#外来函数接口" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>外来函数接口</h3>
<p>使用外来函数接口的库。</p>
<ul>
<li>cffi：用来调用 C 代码的外来函数接口。<a href="https://pypi.python.org/pypi/cffi">官网</a></li>
<li><a href="http://hao.jobbole.com/ctypes/">ctypes</a>：(Python 标准库) 用来调用 C 代码的外来函数接口。<a href="https://docs.python.org/2/library/ctypes.html">官网</a></li>
<li>PyCUDA：Nvidia CUDA API 的封装。<a href="https://mathema.tician.de/software/pycuda/">官网</a></li>
<li>SWIG：简化的封装和接口生成器。<a href="http://www.swig.org/Doc1.3/Python.html">官网</a></li>
</ul>
<h3><a id="user-content-高性能" class="anchor" href="#高性能" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>高性能</h3>
<p>让 Python 更快的库。</p>
<ul>
<li>Cython：优化的 Python 静态编译器。使用类型混合使 Python 编译成 C 或 C++ 模块来获得性能的极大提升。<a href="http://cython.org/">官网</a></li>
<li>PeachPy：嵌入 Python 的 x86-64 汇编器。可以被用作 Python 内联的汇编器或者是独立的汇编器，用于 Windows, Linux, OS X, Native Client 或者 Go 。<a href="https://github.com/Maratyszcza/PeachPy">官网</a></li>
<li>PyPy：使用 Python 实现的 Python。解释器使用黑魔法加快 Python 运行速度且不需要加入额外的类型信息。<a href="http://pypy.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/pyston-llvm-jit/">Pyston</a>：使用 LLVM 和现代 JIT 技术构建的 Python 实现，目标是为了获得很好的性能。<a href="https://github.com/dropbox/pyston">官网</a></li>
<li>Stackless Python：一个强化版的 Python。<a href="https://bitbucket.org/stackless-dev/stackless/overview">官网</a></li>
</ul>
<h3><a id="user-content-微软的-windows平台" class="anchor" href="#微软的-windows平台" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>微软的 Windows平台</h3>
<p>在 Windows 平台上进行 Python 编程。</p>
<ul>
<li>Python(x,y)：面向科学应用的 Python 发行版，基于 Qt 和 Spyder。<a href="http://python-xy.github.io/">官网</a></li>
<li>pythonlibs：非官方的 Windows 平台 Python 扩展二进制包。<a href="http://www.lfd.uci.edu/%7Egohlke/pythonlibs/">官网</a></li>
<li>PythonNet：Python 与 .NET 公共语言运行库 (CLR)的集成。<a href="https://github.com/pythonnet/pythonnet">官网</a></li>
<li>PyWin32：针对 Windows 的Python 扩展。<a href="https://sourceforge.net/projects/pywin32/">官网</a></li>
<li>WinPython：Windows 7/8 系统下便携式开发环境。<a href="https://winpython.github.io/">官网</a></li>
</ul>
<h3><a id="user-content-网络可视化和sdn" class="anchor" href="#网络可视化和sdn" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>网络可视化和SDN</h3>
<p>用来进行网络可视化和SDN(软件定义网络)的工具和库。</p>
<ul>
<li>Mininet：一款流行的网络模拟器以及用 Python 编写的 API。<a href="http://mininet.org/">官网</a></li>
<li>POX：一个针对基于 Python 的软件定义网络应用（例如 OpenFlow SDN 控制器）的开源开发平台。<a href="https://github.com/noxrepo/pox">官网</a></li>
<li>Pyretic：火热的 SDN 编程语言中的一员，为网络交换机和模拟器提供强大的抽象能力。<a href="http://frenetic-lang.org/pyretic/">官网</a></li>
<li>SDX Platform：基于 SDN 的 IXP 实现，影响了 Mininet, POX 和 Pyretic。<a href="https://github.com/sdn-ixp/internet2award">官网</a></li>
</ul>
<h3><a id="user-content-硬件" class="anchor" href="#硬件" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>硬件</h3>
<p>用来对硬件进行编程的库。</p>
<ul>
<li>ino：操作<a href="https://www.arduino.cc/">Arduino</a>的命令行工具。<a href="http://inotool.org/">官网</a></li>
<li>Pyro：Python 机器人编程库。<a href="http://pyrorobotics.com/">官网</a></li>
<li>PyUserInput：跨平台的，控制鼠标和键盘的模块。<a href="https://github.com/SavinaRoja/PyUserInput">官网</a></li>
<li>scapy：一个非常棒的操作数据包的库。<a href="https://github.com/secdev/scapy">官网</a></li>
<li>wifi：一个 Python 库和命令行工具用来在 Linux 平台上操作WiFi。<a href="https://wifi.readthedocs.org/en/latest/">官网</a></li>
<li>Pingo：Pingo 为类似Raspberry Pi，pcDuino， Intel Galileo等设备提供统一的API用以编程。<a href="http://www.pingo.io/">官网</a></li>
</ul>
<h3><a id="user-content-兼容性" class="anchor" href="#兼容性" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>兼容性</h3>
<p>帮助从 Python 2 向 Python 3迁移的库。</p>
<ul>
<li>Python-Future：这就是 Python 2 和 Python 3 之间丢失的那个兼容性层。<a href="http://python-future.org/index.html">官网</a></li>
<li>Python-Modernize：使 Python 代码更加现代化以便最终迁移到 Python 3。<a href="https://github.com/mitsuhiko/python-modernize">官网</a></li>
<li>Six：Python 2 和 3 的兼容性工具。<a href="https://pypi.python.org/pypi/six">官网</a></li>
</ul>
<h3><a id="user-content-杂项" class="anchor" href="#杂项" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>杂项</h3>
<p>不属于上面任何一个类别，但是非常有用的库。</p>
<ul>
<li>blinker：一个快速的 Python 进程内信号/事件分发系统。<a href="https://github.com/jek/blinker">官网</a></li>
<li>itsdangerous：一系列辅助工具用来将可信的数据传入不可信的环境。<a href="https://github.com/pallets/itsdangerous">官网</a></li>
<li>pluginbase：一个简单但是非常灵活的 Python 插件系统。<a href="https://github.com/mitsuhiko/pluginbase">官网</a></li>
<li>Pychievements：一个用来创建和追踪成就的 Python 框架。<a href="https://github.com/PacketPerception/pychievements">官网</a></li>
<li><a href="http://hao.jobbole.com/tryton/">Tryton</a>：一个通用商务框架。<a href="http://www.tryton.org/">官网</a></li>
</ul>
<h3><a id="user-content-算法和设计模式" class="anchor" href="#算法和设计模式" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>算法和设计模式</h3>
<p>Python 实现的算法和设计模式。</p>
<ul>
<li><a href="http://hao.jobbole.com/algorithms/">algorithms</a>：一个 Python 算法模块。<a href="https://github.com/nryoung/algorithms">官网</a></li>
<li>python-patterns：Python 设计模式的集合。<a href="https://github.com/faif/python-patterns">官网</a></li>
<li>sortedcontainers：快速，纯 Python 实现的SortedList，SortedDict 和 SortedSet 类型。<a href="http://www.grantjenks.com/docs/sortedcontainers/">官网</a></li>
</ul>
<h3><a id="user-content-编辑器插件" class="anchor" href="#编辑器插件" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>编辑器插件</h3>
<p>编辑器和 IDE 的插件</p>
<ul>
<li>Emacs
<ul>
<li>Elpy：Emacs Python 开发环境。<a href="https://github.com/jorgenschaefer/elpy">官网</a></li>
</ul>
</li>
<li>Sublime Text
<ul>
<li>SublimeJEDI：一个 Sublime Text 插件，用来使用超赞的自动补全库 Jedi。<a href="https://github.com/srusskih/SublimeJEDI">官网</a></li>
<li>Anaconda：Anaconda 把你的 Sublime Text 3 变成一个功能齐全的 Python IDE。<a href="https://github.com/DamnWidget/anaconda">官网</a></li>
</ul>
</li>
<li>Vim
<ul>
<li><a href="http://hao.jobbole.com/youcompleteme/">YouCompleteMe</a>：引入基于 <a href="https://github.com/davidhalter/jedi">Jedi</a> 的 Python 自动补全引擎。<a href="https://github.com/Valloric/YouCompleteMe">官网</a></li>
<li>Jedi-vim：绑定 Vim 和 Jedi 自动补全库对 Python 进行自动补全。<a href="https://github.com/davidhalter/jedi-vim">官网</a></li>
<li>Python-mode：将 Vim 变成 Python IDE 的一款多合一插件。<a href="https://github.com/klen/python-mode">官网</a></li>
</ul>
</li>
<li>Visual Studio
<ul>
<li>PTVS：Visual Studio 的 Python 工具<a href="https://github.com/Microsoft/PTVS">官网</a></li>
</ul>
</li>
</ul>
<h3><a id="user-content-集成开发环境" class="anchor" href="#集成开发环境" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>集成开发环境</h3>
<p>流行的 Python 集成开发环境。</p>
<ul>
<li>PyCharm：商业化的 Python IDE ，由 JetBrains 开发。也有免费的社区版提供。<a href="https://www.jetbrains.com/pycharm/">官网</a></li>
<li>LiClipse：基于 Eclipse 的免费多语言 IDE 。使用 PyDev 来支持 Python 。<a href="http://www.liclipse.com/">官网</a></li>
<li>Spyder：开源 Python IDE。<a href="https://github.com/spyder-ide/spyder">官网</a></li>
</ul>
<h3><a id="user-content-自动聊天工具" class="anchor" href="#自动聊天工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>自动聊天工具</h3>
<p>用于开发聊天机器人的库</p>
<ul>
<li>  Errbot：最简单和最流行的聊天机器人用来实现自动聊天工具。<a href="http://errbot.io/en/latest/">官网</a></li>
</ul>
<h2><a id="user-content-服务" class="anchor" href="#服务" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>服务</h2>
<p>在线工具和简化开发的 API 。</p>
<h3><a id="user-content-持续集成" class="anchor" href="#持续集成" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>持续集成</h3>
<p>参见: <a href="https://github.com/ciandcd/awesome-ciandcd#online-build-system">awesome-CIandCD</a>.</p>
<ul>
<li>Travis CI：一个流行的工具，为你的开源和<a href="https://travis-ci.com/">私人</a>项目提供持续集成服务。(仅支持 GitHub)<a href="https://travis-ci.org/">官网</a></li>
<li>CircleCI：一个持续集成工具，可以非常快速的进行并行测试。 (仅支持 GitHub)<a href="https://circleci.com/">官网</a></li>
<li>Vexor CI：一个为私人 app 提供持续集成的工具，支持按分钟付费。<a href="https://vexor.io/">官网</a></li>
<li>Wercker：基于 Docker 平台，用来构建和部署微服务。<a href="http://wercker.com/">官网</a></li>
</ul>
<h3><a id="user-content-代码质量" class="anchor" href="#代码质量" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>代码质量</h3>
<ul>
<li>Codacy：自动化代码审查，更加快速的发布高质量代码。对于开源项目是免费的。<a href="https://www.codacy.com/">官网</a></li>
<li>QuantifiedCode：一个数据驱动、自动、持续的代码审查工具。<a href="https://www.quantifiedcode.com/">官网</a></li>
</ul>

## 二、Java

<h2 id="user-content-ancients"><a id="user-content-古董级工具" class="anchor" href="#古董级工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>古董级工具</h2>
<p><em>这些工具伴随着Java一起出现，在各自辉煌之后还在一直使用。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/apache-ant/">Apache Ant</a>：基于XML的构建管理工具。<a href="http://ant.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/cglib/">cglib</a>：字节码生成库。<a href="https://github.com/cglib/cglib">官网</a></li>
<li><a href="http://hao.jobbole.com/glassfish/">GlassFish</a>：应用服务器，由Oracle赞助支持的Java EE参考实现。<a href="https://glassfish.java.net/">官网</a></li>
<li><a href="http://hao.jobbole.com/hudson/">Hudson</a>：持续集成服务器，目前仍在活跃开发。<a href="http://hudson-ci.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/javaserver-faces/">JavaServer Faces</a>：Mojarra是JSF标准的一个开源实现，由Oracle开发。<a href="https://javaserverfaces.java.net/">官网</a></li>
<li><a href="http://hao.jobbole.com/javaserver-pages/">JavaServer Pages</a>：支持自定义标签库的网站通用模板库。<a href="https://jsp.java.net/">官网</a></li>
<li><a href="http://hao.jobbole.com/liquibase/">Liquibase</a>：与具体数据库独立的追踪、管理和应用数据库Scheme变化的工具。<a href="http://www.liquibase.org/">官网</a></li>
</ul>
<h3 id="user-content-build"><a id="user-content-构建工具" class="anchor" href="#构建工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>构建工具</h3>
<p><em>构建及应用依赖关系处理工具。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/maven/">Apache Maven</a>：Maven是一款声明式构建及依赖管理工具，采用约定优于配置方式进行管理。相对Apache Ant更推荐使用Maven，前者采用了过程式管理，维护相对困难。<a href="http://maven.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/bazel/">Bazel</a>：来自Google的构建工具，可以快速、可靠地构建代码。<a href="http://bazel.io">官网</a></li>
<li><a href="http://hao.jobbole.com/gradle/">Gradle</a>：使用Groovy（非XML）进行增量构建，可以很好地与Maven依赖管理配合工作。<a href="http://gradle.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/buck/">Buck</a>：Facebook构建工具。<a href="https://buckbuild.com/">官网</a></li>
</ul>
<h3 id="user-content-bytecode-manipulation"><a id="user-content-字节码操作" class="anchor" href="#字节码操作" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>字节码操作</h3>
<p><em>编程方式操作字节码的开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/asm/">ASM</a>：通用底层字节码操作和分析开发库。<a href="http://asm.ow2.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/byte-buddy/">Byte Buddy</a>：使用流式API进一步简化字节码生成。<a href="http://bytebuddy.net/">官网</a></li>
<li><a href="http://hao.jobbole.com/byteman/">Byteman</a>：在运行时通过DSL（规则）操作字节码进行测试和故障排除。<a href="http://byteman.jboss.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/javassist/">Javassist</a>：一个简化字节码编辑尝试。<a href="http://jboss-javassist.github.io/javassist">官网</a></li>
</ul>
<h3 id="user-content-cluster-management"><a id="user-content-集群管理" class="anchor" href="#集群管理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>集群管理</h3>
<p><em>在集群内动态管理应用程序的框架。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/apache-aurora/">Apache Aurora</a>：Apache Aurora是一个Mesos框架，用于长时间运行服务和定时任务（cron job）。<a href="http://aurora.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/singularity/">Singularity</a>：Singularity是一个Mesos框架，方便部署和操作。它支持Web Service、后台运行、调度作业和一次性任务。<a href="http://getsingularity.com/">官网</a></li>
</ul>
<h3 id="user-content-code-analysis"><a id="user-content-代码分析" class="anchor" href="#代码分析" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>代码分析</h3>
<p><em>测量代码指标和质量工具。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/checkstyle/">Checkstyle</a>：代码编写规范和标准静态分析工具。<a href="https://github.com/checkstyle/checkstyle">官网</a></li>
<li><a href="http://hao.jobbole.com/error-prone/">Error Prone</a>：将常见编程错误作为运行时错误报告。<a href="https://github.com/google/error-prone">官网</a></li>
<li>FindBugs：通过字节码静态分析查找隐藏bug。<a href="http://findbugs.sourceforge.net/">官网</a></li>
<li><a href="http://hao.jobbole.com/jqassistant/">jQAssistant</a>：使用基于Neo4J查询语言进行代码静态分析。<a href="http://jqassistant.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/pmd/">PMD</a>：对源代码分析查找不良的编程习惯。<a href="https://github.com/pmd/pmd">官网</a></li>
<li><a href="http://hao.jobbole.com/sonarqube/">SonarQube</a>：通过插件集成其它分析组件，对过去一段时间内的数据进行统计。<a href="http://www.sonarqube.org/">官网</a></li>
</ul>
<h3 id="user-content-compiler-compiler"><a id="user-content-编译器生成工具" class="anchor" href="#编译器生成工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>编译器生成工具</h3>
<p><em>用来创建解析器、解释器或编译器的框架。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/antlr/">ANTLR</a>：复杂的全功能自顶向下解析框架。<a href="http://www.antlr.org/">官网</a></li>
<li><a href="/jobbole/awesome-java-cn/blob/master/JavaCC%EF%BC%9AJava%E8%AF%AD%E6%B3%95%E8%A7%A3%E6%9E%90%E5%99%A8%E7%94%9F%E6%88%90%E5%B7%A5%E5%85%B7">JavaCC</a>：JavaCC是更加专门的轻量级工具，易于上手且支持语法超前预测。<a href="https://javacc.java.net/">官网</a></li>
</ul>
<h3 id="user-content-configuration"><a id="user-content-外部配置工具" class="anchor" href="#外部配置工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>外部配置工具</h3>
<p><em>支持外部配置的开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/config/">config</a>：针对JVM语言的配置库。<a href="https://github.com/typesafehub/config">官网</a></li>
<li><a href="http://hao.jobbole.com/owner/">owner</a>：减少冗余配置属性。<a href="https://github.com/lviggiano/owner">官网</a></li>
</ul>
<h3 id="user-content-constraint-satisfaction-problem-solver"><a id="user-content-约束满足问题求解程序" class="anchor" href="#约束满足问题求解程序" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>约束满足问题求解程序</h3>
<p><em>帮助解决约束满足问题的开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/choco/">Choco</a>：可直接使用的约束满足问题求解程序，使用了约束规划技术。<a href="http://choco-solver.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/jacop/">JaCoP</a>：为FlatZinc语言提供了一个接口，可以执行MiniZinc模型。<a href="https://github.com/radsz/jacop/">官网</a></li>
<li><a href="http://hao.jobbole.com/optaplanner/">OptaPlanner</a>：业务规划与资源调度优化求解程序。<a href="http://www.optaplanner.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/sat4j/">Sat4J</a>：逻辑代数与优化问题最先进的求解程序。<a href="http://www.sat4j.org/">官网</a></li>
</ul>
<h3 id="user-content-continuous-integration"><a id="user-content-持续集成" class="anchor" href="#持续集成" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>持续集成</h3>
<ul>
<li><a href="http://hao.jobbole.com/bamboo/">Bamboo</a>：Atlassian解决方案，可以很好地集成Atlassian的其他产品。可以选择开源许可，也可以购买商业版。<a href="https://www.atlassian.com/software/bamboo">官网</a></li>
<li>CircleCI：提供托管服务，可以免费试用。<a href="https://circleci.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/codeship/">Codeship</a>：提供托管服务，提供有限的免费模式。<a href="https://codeship.com/features">官网</a></li>
<li><a href="/jobbole/awesome-java-cn/blob/master/hao.jobbole.com/fabric8">fabric8</a>：容器集成平台。<a href="http://fabric8.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/go/">Go</a>：ThoughtWork开源解决方案。<a href="https://www.gocd.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/jenkins/">Jenkins</a>：支持基于服务器的部署服务。<a href="http://jenkins-ci.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/teamcity/">TeamCity</a>：JetBrain的持续集成解决方案，有免费版。<a href="http://www.jetbrains.com/teamcity/">官网</a></li>
<li><a href="http://hao.jobbole.com/travis/">Travis</a>：通常用作开源项目的托管服务。<a href="https://travis-ci.org">官网</a></li>
<li><a href="http://hao.jobbole.com/buildkite/">Buildkite</a>: 持续集成工具，用简单的脚本就能设置pipeline，而且能快速构建，可以免费试用。<a href="https://buildkite.com/">官网</a></li>
</ul>
<h3 id="user-content-csv"><a id="user-content-csv解析" class="anchor" href="#csv解析" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>CSV解析</h3>
<p><em>简化CSV数据读写的框架与开发库</em></p>
<ul>
<li><a href="http://hao.jobbole.com/univocity-parsers/">uniVocity-parsers</a>：速度最快功能最全的CSV开发库之一，同时支持TSV与固定宽度记录的读写。<a href="https://github.com/uniVocity/univocity-parsers">官网</a></li>
</ul>
<h3 id="user-content-database"><a id="user-content-数据库" class="anchor" href="#数据库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据库</h3>
<p><em>简化数据库交互的相关工具。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/apache-phoenix/">Apache Phoenix</a>：HBase针对低延时应用程序的高性能关系数据库层。<a href="http://phoenix.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/crate/">Crate</a>：实现了数据同步、分片、缩放、复制的分布式数据存储。除此之外还可以使用基于SQL的语法跨集群查询。<a href="https://crate.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/flyway/">Flyway</a>：简单的数据库迁移工具。<a href="http://flywaydb.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/h2/">H2</a>：小型SQL数据库，以可以作为内存数据库使用著称。<a href="http://h2database.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/hikaricp/">HikariCP</a>：高性能JDBC连接工具。<a href="https://github.com/brettwooldridge/HikariCP">官网</a></li>
<li><a href="http://hao.jobbole.com/jdbi/">JDBI</a>：便捷的JDBC抽象。<a href="http://jdbi.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/jooq/">jOOQ</a>：为SQL schema生成typesafe代码。<a href="http://www.jooq.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/mapdb/">MapDB</a>：以磁盘或堆内存中并发集合为基础的嵌入式数据库引擎。<a href="http://www.mapdb.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/presto/">Presto</a>：针对大数据的分布式SQL查询引擎。<a href="https://github.com/facebook/presto">官网</a></li>
<li><a href="http://hao.jobbole.com/querydsl/">Querydsl</a>：Typesafe统一查询。<a href="http://www.querydsl.com/">官网</a></li>
</ul>
<h3 id="user-content-data-structures"><a id="user-content-数据结构" class="anchor" href="#数据结构" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据结构</h3>
<ul>
<li><a href="http://hao.jobbole.com/apache-parquet/">Apache Parquet</a>：Google Dremel论文中发布的基于组装算法的列式（Columnar）存储格式。<a href="http://parquet.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/protobuf/">Protobuf</a>：Google数据交换格式。<a href="https://github.com/google/protobuf">官网</a></li>
<li><a href="http://hao.jobbole.com/sbe/">SBE</a>：简单二进制编码，是最快速的消息格式之一。<a href="https://github.com/real-logic/simple-binary-encoding">官网</a></li>
<li><a href="http://hao.jobbole.com/wire/">Wire</a>：整洁轻量级协议缓存。<a href="https://github.com/square/wire">官网</a></li>
</ul>
<h3 id="user-content-date-and-time"><a id="user-content-时间日期工具库" class="anchor" href="#时间日期工具库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>时间日期工具库</h3>
<p><em>处理时间和日期的开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/joda-time/">Joda-Time</a>：在Java 8发布前，Joda-Time是实际使用的时间日期库标准。<a href="http://www.joda.org/joda-time/">官网</a></li>
<li><a href="http://hao.jobbole.com/time4j/">Time4J</a>：高级时间和日期库。<a href="https://github.com/MenoData/Time4J">官网</a></li>
<li><a href="http://hao.jobbole.com/ThreeTen/">ThreeTen</a>：JSR-310实现，为JDK提供更具特点的时间和日期API。<a href="http://www.threeten.org">官网</a></li>
</ul>
<h3 id="user-content-dependency-injection"><a id="user-content-依赖注入" class="anchor" href="#依赖注入" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>依赖注入</h3>
<p><em>帮实现依赖翻转范式的开发库。</em> <a href="https://en.wikipedia.org/wiki/Inversion_of_control">官网</a></p>
<ul>
<li><a href="http://hao.jobbole.com/apache-deltaspike/">Apache DeltaSpike</a>：CDI扩展框架。<a href="https://deltaspike.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/dagger2/">Dagger2</a>：编译时注入框架，不需要使用反射。<a href="http://google.github.io/dagger/">官网</a></li>
<li><a href="http://hao.jobbole.com/guice/">Guice</a>：可以匹敌Dagger的轻量级注入框架。<a href="https://github.com/google/guice">官网</a></li>
<li><a href="http://hao.jobbole.com/hk2/">HK2</a>：轻量级动态依赖注入框架。<a href="https://hk2.java.net">官网</a></li>
</ul>
<h3 id="user-content-development"><a id="user-content-开发流程增强工具" class="anchor" href="#开发流程增强工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>开发流程增强工具</h3>
<p><em>从最基本的层面增强开发流程。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/adt4j/">ADT4J</a>：针对代数数据类型的JSR-269代码生成器。<a href="https://github.com/sviperll/adt4j">官网</a></li>
<li><a href="http://hao.jobbole.com/aspectj/">AspectJ</a>：面向切面编程（AOP）的无缝扩展。<a href="https://eclipse.org/aspectj/">官网</a></li>
<li><a href="http://hao.jobbole.com/auto/">Auto</a>：源代码生成器集合。<a href="https://github.com/google/auto">官网</a></li>
<li><a href="http://hao.jobbole.com/dcevm/">DCEVM</a>：通过修改JVM在运行时支持对已加载的类进行无限次重定义。<a href="http://dcevm.github.io/">官网</a></li>
<li>HotswapAgent：支持无限次重定义运行时类与资源。<a href="https://github.com/HotswapProjects/HotswapAgent">官网</a></li>
<li>Immutables：类似Scala的条件类。<a href="http://immutables.github.io/">官网</a></li>
<li>JHipster：基于Spring Boot与AngularJS应用程序的Yeoman源代码生成器。<a href="https://github.com/jhipster/generator-jhipster">官网</a></li>
<li><a href="http://hao.jobbole.com/jrebel/">JRebel</a>：无需重新部署，可以即时重新加载代码与配置的商业软件。<a href="http://zeroturnaround.com/software/jrebel/">官网</a></li>
<li>Lombok：减少冗余的代码生成器。<a href="https://projectlombok.org/">官网</a></li>
<li>Spring Loaded：类重载代理。<a href="https://github.com/spring-projects/spring-loaded">官网</a></li>
<li><a href="http://hao.jobbole.com/vert-x/">vert.x</a>：多语言事件驱动应用框架。<a href="http://vertx.io/">官网</a></li>
</ul>
<h3 id="user-content-distributed-applications"><a id="user-content-分布式应用" class="anchor" href="#分布式应用" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>分布式应用</h3>
<p><em>用来编写分布式容错应用的开发库和框架。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/akka/">Akka</a>：用来编写分布式容错并发事件驱动应用程序的工具和运行时。<a href="http://akka.io">官网</a></li>
<li><a href="http://hao.jobbole.com/storm/">Apache Storm</a>：实时计算系统。<a href="http://storm.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/zookeeper/">Apache ZooKeeper</a>：针对大型分布式系统的协调服务，支持分布式配置、同步和名称注册。<a href="http://zookeeper.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/Hazelcast/">Hazelcast</a>：高可扩展内存数据网格。<a href="http://hazelcast.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/hystrix/">Hystrix</a>：提供延迟和容错。<a href="https://github.com/Netflix/Hystrix">官网</a></li>
<li><a href="http://hao.jobbole.com/jgroups/">JGroups</a>：提供可靠的消息传递和集群创建的工具。<a href="http://www.jgroups.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/orbit/">Orbit</a>：支持虚拟角色（Actor），在传统角色的基础上增加了另外一层抽象。<a href="http://orbit.bioware.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/quasar/">Quasar</a>：为JVM提供轻量级线程和角色。<a href="http://www.paralleluniverse.co/quasar/">官网</a></li>
</ul>
<h3 id="user-content-distributed-databases"><a id="user-content-分布式数据库" class="anchor" href="#分布式数据库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>分布式数据库</h3>
<p><em>对应用程序而言，在分布式系统中的数据库看起来就像是只有一个数据源。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/cassandra/">Apache Cassandra</a>：列式数据库，可用性高且没有单点故障。<a href="http://cassandra.apache.org">官网</a></li>
<li><a href="http://hao.jobbole.com/hbase/">Apache HBase</a>：针对大数据的Hadoop数据库。<a href="http://hbase.apache.org">官网</a></li>
<li><a href="http://hao.jobbole.com/druid/">Druid</a>：实时和历史OLAP数据存储，在聚集查询和近似查询方面表现不俗。<a href="http://druid.io">官网</a></li>
<li><a href="http://hao.jobbole.com/infinispan/">Infinispan</a>：针对缓存的高并发键值对数据存储。<a href="http://infinispan.org/">官网</a></li>
</ul>
<h3 id="user-content-distribution"><a id="user-content-发布" class="anchor" href="#发布" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>发布</h3>
<p><em>以本机格式发布应用程序的工具。</em></p>
<ul>
<li>Bintray：发布二进制文件版本控制工具。可以于Maven或Gradle一起配合使用。提供开源免费版本和几种商业收费版本。<a href="https://bintray.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/central-repository/">Central Repository</a>：最大的二进制组件仓库，面向开源社区提供免费服务。Apache Maven默认使用Central <a href="http://search.maven.org/">官网</a>Repository，也可以在所有其他构建工具中使用。</li>
<li>IzPack：为跨平台部署建立创作工具（Authoring Tool）。<a href="http://izpack.org/">官网</a></li>
<li>JitPack：打包GitHub仓库的便捷工具。可根据需要构建Maven、Gradle项目，发布可立即使用的组件。<a href="https://jitpack.io/">官网</a></li>
<li>Launch4j：将JAR包装为轻量级本机Windows可执行程序。<a href="http://launch4j.sourceforge.net/">官网</a></li>
<li>Nexus：支持代理和缓存功能的二进制管理工具。<a href="http://www.sonatype.com/nexus">官网</a></li>
<li>packr：将JAR、资源和JVM打包成Windows、Linux和Mac OS X本地发布文件。<a href="https://github.com/libgdx/packr/">官网</a></li>
</ul>
<h3 id="user-content-document-processing"><a id="user-content-文档处理工具" class="anchor" href="#文档处理工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>文档处理工具</h3>
<p><em>处理Office文档的开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/poi/">Apache POI</a>：支持OOXML规范（XLSX、DOCX、PPTX）以及OLE2规范（XLS、DOC、PPT）。<a href="http://poi.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/documents4j/">documents4j</a>：使用第三方转换器进行文档格式转换，转成类似MS Word这样的格式。<a href="http://documents4j.com">官网</a></li>
<li><a href="http://hao.jobbole.com/jopendocument/">jOpenDocument</a>：处理OpenDocument格式（由Sun公司提出基于XML的文档格式）。<a href="http://www.jopendocument.org/">官网</a></li>
</ul>
<h3 id="user-content-functional-programming"><a id="user-content-函数式编程" class="anchor" href="#函数式编程" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>函数式编程</h3>
<p><em>函数式编程支持库。</em></p>
<ul>
<li>Cyclops：支持一元（Monad）操作和流操作工具类、comprehension（List语法）、模式匹配、trampoline等特性。<a href="https://github.com/aol/cyclops">官网</a></li>
<li>Fugue：Guava的函数式编程扩展。<a href="https://bitbucket.org/atlassian/fugue">官网</a></li>
<li>Functional Java：实现了多种基础和高级编程抽象，用来辅助面向组合开发（composition-oriented development）。<a href="http://www.functionaljava.org">官网</a></li>
<li>Javaslang：一个函数式组件库，提供持久化数据类型和函数式控制结构。<a href="http://javaslang.com">官网</a></li>
<li>jOOλ：旨在填补Java 8 lambda差距的扩展，提供了众多缺失的类型和一组丰富的顺序流API。<a href="https://github.com/jOOQ/jOOL">官网</a></li>
</ul>
<h3 id="user-content-game-development"><a id="user-content-游戏开发" class="anchor" href="#游戏开发" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>游戏开发</h3>
<p><em>游戏开发框架。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/jmonkeyengine/">jMonkeyEngine</a>：现代3D游戏开发引擎。<a href="http://jmonkeyengine.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/libgdx/">libGDX</a>：全面的跨平台高级框架。<a href="https://libgdx.badlogicgames.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/lwjgl/">LWJGL</a>：对OpenGL/CL/AL等技术进行抽象的健壮框架。<a href="https://www.lwjgl.org/">官网</a></li>
</ul>
<h3 id="user-content-gui"><a id="user-content-gui" class="anchor" href="#gui" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>GUI</h3>
<p><em>现代图形化用户界面开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/javafx/">JavaFX</a>：Swing的后继者。<a href="http://www.oracle.com/technetwork/java/javase/overview/javafx-overview-2158620.html">官网</a></li>
<li><a href="http://hao.jobbole.com/scene_builder/">Scene Builder</a>：开发JavaFX应用的可视化布局工具。<a href="http://docs.oracle.com/javase/8/scene-builder-2/get-started-tutorial/overview.htm#JSBGS164">官网</a></li>
</ul>
<h3 id="user-content-high-performance"><a id="user-content-高性能计算" class="anchor" href="#高性能计算" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>高性能计算</h3>
<p><em>涵盖了从集合到特定开发库的高性能计算相关工具。</em></p>
<ul>
<li>Agrona：高性能应用中常见的数据结构和工具方法。<a href="https://github.com/real-logic/Agrona">官网</a></li>
<li>Disruptor：线程间消息传递开发库。<a href="http://lmax-exchange.github.io/disruptor/">官网</a></li>
<li>fastutil：快速紧凑的特定类型集合（Collection）。<a href="http://fastutil.di.unimi.it/">官网</a></li>
<li>GS Collections：受Smalltalk启发的集合框架。<a href="https://github.com/goldmansachs/gs-collections">官网</a></li>
<li><a href="http://hao.jobbole.com/hppc/">HPPC</a>：基础类型集合。<a href="http://labs.carrotsearch.com/hppc.html">官网</a></li>
<li>Javolution：实时和嵌入式系统的开发库。<a href="http://javolution.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/jctools/">JCTools</a>：JDK中缺失的并发工具。<a href="https://github.com/JCTools/JCTools">官网</a></li>
<li><a href="http://hao.jobbole.com/koloboke/">Koloboke</a>：Hash set和hash map。<a href="https://github.com/OpenHFT/Koloboke">官网</a></li>
<li>Trove：基础类型集合。<a href="http://trove.starlight-systems.com/">官网</a></li>
<li>High-scale-lib:Cliff Click 个人开发的高性能并发库<a href="https://github.com/stephenc/high-scale-lib">官网</a></li>
</ul>
<h3 id="user-content-ide"><a id="user-content-ide" class="anchor" href="#ide" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>IDE</h3>
<p><em>简化开发的集成开发环境。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/eclipse/">Eclipse</a>：老牌开源项目，支持多种插件和编程语言。<a href="http://www.eclipse.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/intellij-idea/">IntelliJ IDEA</a>：支持众多JVM语言，是安卓开发者好的选择。商业版主要针对企业客户。<a href="http://www.jetbrains.com/idea/">官网</a></li>
<li><a href="http://hao.jobbole.com/netbeans/">NetBeans</a>：为多种技术提供集成化支持，包括Java SE、Java EE、数据库访问、HTML5等。<a href="https://netbeans.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/scala-ide/">Scala IDE</a>：一款基于Eclipse开源平台打造的Scala集成开发环境。<a href="http://scala-ide.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/springsource-tool-suite/">SpringSource Tool Suite（STS）</a>:一款基于Eclipse开源平台打造的Spring应用开发环境。<a href="http://spring.io/tools/sts/">官网</a></li>
</ul>
<h3 id="user-content-imagery"><a id="user-content-图像处理" class="anchor" href="#图像处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>图像处理</h3>
<p><em>创建、评价和操作图片的支持库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/imgscalr/">Imgscalr</a>：纯Java 2D实现，简单、高效、支持硬件加速的图像缩放开发库。<a href="https://github.com/thebuzzmedia/imgscalr">官网</a></li>
<li><a href="http://hao.jobbole.com/picasso/">Picasso</a>：安卓图片下载和图片缓存开发库。<a href="http://square.github.io/picasso/">官网</a></li>
<li><a href="http://hao.jobbole.com/thumbnailator/">Thumbnailator</a>：Thumbnailator是一个高质量Java缩略图开发库。<a href="https://github.com/coobird/thumbnailator">官网</a></li>
<li><a href="http://hao.jobbole.com/zxing/">ZXing</a>：支持多种格式的一维、二维条形码图片处理开发库。<a href="https://github.com/zxing/zxing">官网</a></li>
<li><a href="http://hao.jobbole.com/im4java/">im4java</a>: 基于ImageMagick或GraphicsMagick命令行的图片处理开发库，基本上ImageMagick能够支持的图片格式和处理方式都能够处理。<a href="http://im4java.sourceforge.net/">官网</a></li>
<li>Apache Batik：在Java应用中程序以SVG格式显示、生成及处理图像的工具集，包括SVG解析器、SVG生成器、SVG DOM等模块，可以集成使用也可以单独使用，还可以扩展自定义的SVG标签。<a href="http://xmlgraphics.apache.org/batik/">官网</a></li>
</ul>
<h3 id="user-content-json"><a id="user-content-json" class="anchor" href="#json" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>JSON</h3>
<p><em>简化JSON处理的开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/genson/">Genson</a>：强大且易于使用的Java到JSON转换开发库。<a href="http://owlike.github.io/genson">官网</a></li>
<li><a href="http://hao.jobbole.com/gson/">Gson</a>：谷歌官方推出的JSON处理库，支持在对象与JSON之间双向序列化，性能良好且可以实时调用。<a href="https://github.com/google/gson">官网</a></li>
<li><a href="http://hao.jobbole.com/jackson/">Jackson</a>：与GSON类似，在频繁使用时性能更佳。<a href="http://wiki.fasterxml.com/JacksonHome">官网</a></li>
<li><a href="http://hao.jobbole.com/logansquare/">LoganSquare</a>：基于Jackson流式API，提供对JSON解析和序列化。比GSON与Jackson组合方式效果更好。<a href="https://github.com/bluelinelabs/LoganSquare">官网</a></li>
<li><a href="http://hao.jobbole.com/fastjson/">Fastjson</a>：一个Java语言编写的高性能功能完善的JSON库。<a href="https://github.com/Alibaba/fastjson">官网</a></li>
<li>Kyro：快速、高效、自动化的Java对象序列化和克隆库。<a href="https://github.com/EsotericSoftware/kryo">官网</a></li>
</ul>
<h3 id="user-content-jvm-and-jdk"><a id="user-content-jvm与jdk" class="anchor" href="#jvm与jdk" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>JVM与JDK</h3>
<p><em>目前的JVM和JDK实现。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/jdk-9/">JDK 9</a>：JDK 9的早期访问版本。<a href="https://jdk9.java.net/">官网</a></li>
<li><a href="http://hao.jobbole.com/openjdk/">OpenJDK</a>：JDK开源实现。<a href="http://openjdk.java.net/">官网</a></li>
</ul>
<h3 id="user-content-languages"><a id="user-content-基于jvm的语言" class="anchor" href="#基于jvm的语言" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>基于JVM的语言</h3>
<p><em>除Java外，可以用来编写JVM应用程序的编程语言。</em></p>
<ul>
<li>Scala：融合了面向对象和函数式编程思想的静态类型编程语言。<a href="http://www.scala-lang.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/groovy/">Groovy</a>：类型可选（Optionally typed）的动态语言，支持静态类型和静态编译。目前是一个Apache孵化器项目。<a href="http://www.groovy-lang.org/">官网</a></li>
<li>Clojure：可看做现代版Lisp的动态类型语言。<a href="http://clojure.org/">官网</a></li>
<li>Ceylon：RedHat开发的面向对象静态类型编程语言。<a href="http://ceylon-lang.org/">官网</a></li>
<li>Kotlin：JetBrain针对JVM、安卓和浏览器提供的静态类型编程语言。<a href="http://kotlinlang.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/xtend/">Xtend</a>：一种静态编程语言，能够将其代码转换为简洁高效的Java代码，并基于JVM运行。<a href="http://www.eclipse.org/xtend/">官网</a></li>
</ul>
<h3 id="user-content-logging"><a id="user-content-日志" class="anchor" href="#日志" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>日志</h3>
<p><em>记录应用程序行为日志的开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/log4j2/">Apache Log4j 2</a>：使用强大的插件和配置架构进行完全重写。<a href="http://logging.apache.org/log4j/">官网</a></li>
<li><a href="http://hao.jobbole.com/kibana/">kibana</a>：分析及可视化日志文件。<a href="https://www.elastic.co/products/kibana">官网</a></li>
<li><a href="http://hao.jobbole.com/logback/">Logback</a>：强健的日期开发库，通过Groovy提供很多有趣的选项。<a href="http://logback.qos.ch/">官网</a></li>
<li><a href="http://hao.jobbole.com/logstash/">logstash</a>：日志文件管理工具。<a href="https://www.elastic.co/products/logstash">官网</a></li>
<li><a href="http://hao.jobbole.com/metrics/">Metrics</a>：通过JMX或HTTP发布参数，并且支持存储到数据库。<a href="https://github.com/dropwizard/metrics">官网</a></li>
<li><a href="http://hao.jobbole.com/slf4j/">SLF4J</a>：日志抽象层，需要与具体的实现配合使用。<a href="http://www.slf4j.org/">官网</a></li>
</ul>
<h3 id="user-content-machine-learning"><a id="user-content-机器学习" class="anchor" href="#机器学习" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>机器学习</h3>
<p><em>提供具体统计算法的工具。其算法可从数据中学习。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/apache-flink/">Apache Flink</a>：快速、可靠的大规模数据处理引擎。<a href="https://flink.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/apache-hadoop/">Apache Hadoop</a>：在商用硬件集群上用来进行大规模数据存储的开源软件框架。<a href="http://hadoop.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/apache-mahout/">Apache Mahout</a>：专注协同过滤、聚类和分类的可扩展算法。<a href="https://mahout.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/apache-spark/">Apache Spark</a>：开源数据分析集群计算框架。<a href="http://spark.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/deepdive/">DeepDive</a>：从非结构化数据建立结构化信息并集成到已有数据库的工具。<a href="http://deepdive.stanford.edu">官网</a></li>
<li><a href="http://hao.jobbole.com/deeplearning4j/">Deeplearning4j</a>：分布式多线程深度学习开发库。<a href="http://deeplearning4j.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/h2o/">H2O</a>：用作大数据统计的分析引擎。<a href="http://h2o.ai/">官网</a></li>
<li><a href="http://hao.jobbole.com/weka/">Weka</a>：用作数据挖掘的算法集合，包括从预处理到可视化的各个层次。<a href="http://www.cs.waikato.ac.nz/ml/weka/">官网</a></li>
<li><a href="http://hao.jobbole.com/quickml/">QuickML</a>：高效机器学习库。<a href="http://quickml.org/">官网</a>、<a href="https://github.com/sanity/quickml">GitHub</a></li>
</ul>
<h3 id="user-content-messaging"><a id="user-content-消息传递" class="anchor" href="#消息传递" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>消息传递</h3>
<p><em>在客户端之间进行消息传递，确保协议独立性的工具。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/aeron/">Aeron</a>：高效可扩展的单播、多播消息传递工具。<a href="https://github.com/real-logic/Aeron">官网</a></li>
<li><a href="http://hao.jobbole.com/activemq/">Apache ActiveMQ</a>：实现JMS的开源消息代理（broker），可将同步通讯转为异步通讯。<a href="http://activemq.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/apache-camel/">Apache Camel</a>：通过企业级整合模式（Enterprise Integration Pattern EIP）将不同的消息传输API整合在一起。<a href="http://camel.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/kafka/">Apache Kafka</a>：高吞吐量分布式消息系统。<a href="http://kafka.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/hermes/">Hermes</a>：快速、可靠的消息代理（Broker），基于Kafka构建。<a href="http://hermes.allegro.tech">官网</a></li>
<li>JBoss HornetQ：清晰、准确、模块化，可以方便嵌入的消息工具。<a href="http://hornetq.jboss.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/jeromq/">JeroMQ</a>：ZeroMQ的纯Java实现。<a href="https://github.com/zeromq/jeromq">官网</a></li>
<li><a href="http://hao.jobbole.com/smack/">Smack</a>：跨平台XMPP客户端函数库。<a href="https://github.com/igniterealtime/Smack/">官网</a></li>
<li>Openfire：是开源的、基于XMPP、采用Java编程语言开发的实时协作服务器。 Openfire安装和使用都非常简单，并可利用Web界面进行管理。 <a href="http://www.igniterealtime.org/projects/openfire/index.jsp">官网</a> <a href="https://github.com/igniterealtime/Openfire">GitHub</a></li>
<li>Spark：是一个开源，跨平台IM客户端。它的特性支持集组聊天，电话集成和强大安全性能。如果企业内部部署IM使用Openfire+Spark是最佳的组合。 <a href="http://www.igniterealtime.org/projects/spark/index.jsp">官网</a> <a href="https://github.com/igniterealtime/Spark">GitHub</a></li>
<li>Tigase： 是一个轻量级的可伸缩的 Jabber/XMPP 服务器。无需其他第三方库支持，可以处理非常高的复杂和大量的用户数，可以根据需要进行水平扩展。 <a href="http://www.tigase.net">官网</a></li>
</ul>
<h3 id="user-content-miscellaneous"><a id="user-content-杂项" class="anchor" href="#杂项" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>杂项</h3>
<p><em>未分类其它资源。</em></p>
<ul>
<li>Design Patterns：实现并解释了最常见的设计模式。<a href="https://github.com/iluwatar/java-design-patterns">官网</a></li>
<li>Jimfs：内存文件系统。<a href="https://github.com/google/jimfs">官网</a></li>
<li>Lanterna：类似curses的简单console文本GUI函数库。<a href="https://code.google.com/p/lanterna/">官网</a></li>
<li>LightAdmin：可插入式CRUD UI函数库，可用来快速应用开发。<a href="http://lightadmin.org/">官网</a></li>
<li>OpenRefine：用来处理混乱数据的工具，包括清理、转换、使用Web Service进行扩展并将其关联到数据库。<a href="http://openrefine.org/">官网</a></li>
<li>RoboVM：Java编写原生iOS应用。<a href="https://robovm.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/quartz/">Quartz</a>：强大的任务调度库.<a href="http://www.quartz-scheduler.org/">官网</a></li>
</ul>
<h3 id="user-content-monitoring"><a id="user-content-应用监控工具" class="anchor" href="#应用监控工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>应用监控工具</h3>
<p><em>监控生产环境中应用程序的工具。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/appdynamics/">AppDynamics</a>：性能监测商业工具。<a href="http://www.appdynamics.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/javamelody/">JavaMelody</a>：性能监测和分析工具。<a href="https://github.com/javamelody/javamelody">官网</a></li>
<li><a href="http://hao.jobbole.com/Kamon/">Kamon</a>：Kamon用来监测在JVM上运行的应用程序。<a href="http://www.kamon.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/new-relic/">New Relic</a>：性能监测商业工具。<a href="http://newrelic.com/">官网</a></li>
<li>SPM：支持对JVM应用程序进行分布式事务追踪的性能监测商业工具。<a href="https://sematext.com/spm/">官网</a></li>
<li><a href="http://hao.jobbole.com/overops_takipi/">OverOps(Takipi)</a>：产品运行时错误监测及调试商业工具。<a href="https://www.takipi.com/">官网</a></li>
</ul>
<h3 id="user-content-native"><a id="user-content-原生开发库" class="anchor" href="#原生开发库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>原生开发库</h3>
<p><em>用来进行特定平台开发的原生开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/jna/">JNA</a>：不使用JNI就可以使用原生开发库。此外，还为常见系统函数提供了接口。<a href="https://github.com/java-native-access/jna">官网</a></li>
</ul>
<h3 id="user-content-natural-language-processing"><a id="user-content-自然语言处理" class="anchor" href="#自然语言处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>自然语言处理</h3>
<p><em>用来专门处理文本的函数库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/apache-opennlp/">Apache OpenNLP</a>：处理类似分词等常见任务的工具。<a href="https://opennlp.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/stanford_corenlp/">CoreNLP</a>：斯坦佛CoreNLP提供了一组基础工具，可以处理类似标签、实体名识别和情感分析这样的任务。<a href="http://nlp.stanford.edu/software/coenlp.shtml">官网</a></li>
<li><a href="http://hao.jobbole.com/lingpipe/">LingPipe</a>：一组可以处理各种任务的工具集，支持POS标签、情感分析等。<a href="http://alias-i.com/lingpipe/">官网</a></li>
<li><a href="http://hao.jobbole.com/mallet/">Mallet</a>：统计学自然语言处理、文档分类、聚类、主题建模等。<a href="http://mallet.cs.umass.edu/">官网</a></li>
</ul>
<h3 id="user-content-networking"><a id="user-content-网络" class="anchor" href="#网络" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>网络</h3>
<p><em>网络编程函数库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/async-http-client/">Async Http Client</a>：异步HTTP和WebSocket客户端函数库。<a href="https://github.com/AsyncHttpClient/async-http-client">官网</a></li>
<li><a href="http://hao.jobbole.com/grizzly/">Grizzly</a>：NIO框架，在Glassfish中作为网络层使用。<a href="https://grizzly.java.net/">官网</a></li>
<li><a href="http://hao.jobbole.com/netty/">Netty</a>：构建高性能网络应用程序开发框架。<a href="http://netty.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/okhttp/">OkHttp</a>：一个Android和Java应用的HTTP+SPDY客户端。<a href="http://square.github.io/okhttp/">官网</a></li>
<li>Undertow：基于NIO实现了阻塞和非阻塞API的Web服务器，在WildFly中作为网络层使用。<a href="http://undertow.io/">官网</a></li>
</ul>
<h3 id="user-content-orm"><a id="user-content-orm" class="anchor" href="#orm" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>ORM</h3>
<p><em>处理对象持久化的API。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/ebean/">Ebean</a>：支持快速数据访问和编码的ORM框架。<a href="http://ebean-orm.github.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/eclipselink/">EclipseLink</a>：支持许多持久化标准，JPA、JAXB、JCA和SDO。<a href="https://www.eclipse.org/eclipselink/">官网</a></li>
<li><a href="http://hao.jobbole.com/hibernate/">Hibernate</a>：广泛使用、强健的持久化框架。Hibernate的技术社区非常活跃。<a href="http://hibernate.org/orm/">官网</a></li>
<li><a href="http://hao.jobbole.com/mybatis/">MyBatis</a>：带有存储过程或者SQL语句的耦合对象（Couples object）。<a href="http://mybatis.github.io/mybatis-3/">官网</a></li>
<li><a href="http://hao.jobbole.com/ormlite/">OrmLite</a>：轻量级开发包，免除了其它ORM产品中的复杂性和开销。<a href="http://ormlite.com/">官网</a></li>
<li>Nutz：另一个SSH。<a href="http://nutzam.com/">官网</a>，<a href="https://github.com/nutzam/nutz">Github</a></li>
<li>JFinal：JAVA WEB + ORM框架。<a href="http://www.jfinal.com">官网</a>，<a href="https://github.com/jfinal/jfinal">Github</a></li>
<li><a href="http://openjpa.apache.org/">Apache OpenJPA</a>: 实现了 EJB 3.0 中的 JPA 标准,为开发者提供功能强大、使用简单的持久化数据管理框架。 <a href="http://openjpa.apache.org/">官网</a></li>
</ul>
<h3 id="user-content-pdf"><a id="user-content-pdf" class="anchor" href="#pdf" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>PDF</h3>
<p><em>用来帮助创建PDF文件的资源。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/apache_fop/">Apache FOP</a>：从XSL-FO创建PDF。<a href="http://xmlgraphics.apache.org/fop/">官网</a></li>
<li><a href="http://hao.jobbole.com/apache-pdfbox/">Apache PDFBox</a>：用来创建和操作PDF的工具集。<a href="http://pdfbox.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/dynamicreports/">DynamicReports</a>：JasperReports的精简版。<a href="http://dynamicreports.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/flyingsaucer/">flyingsaucer</a>：XML/XHTML和CSS 2.1渲染器。<a href="https://github.com/flyingsaucerproject/flyingsaucer">官网</a></li>
<li><a href="http://hao.jobbole.com/itext/">iText</a>：一个易于使用的PDF函数库，用来编程创建PDF文件。注意，用于商业用途时需要许可证。<a href="http://itextpdf.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/jasperreports/">JasperReports</a>：一个复杂的报表引擎。<a href="http://community.jaspersoft.com/project/jasperreports-library">官网</a></li>
</ul>
<h3 id="user-content-performance-analysis"><a id="user-content-性能分析" class="anchor" href="#性能分析" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>性能分析</h3>
<p><em>性能分析、性能剖析及基准测试工具。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/jhiccup/">jHiccup</a>：提供平台中JVM暂停的日志和记录。<a href="https://github.com/giltene/jHiccup">官网</a></li>
<li><a href="http://hao.jobbole.com/jmh/">JMH</a>：JVM基准测试工具。<a href="http://openjdk.java.net/projects/code-tools/jmh/">官网</a></li>
<li><a href="http://hao.jobbole.com/jprofiler/">JProfiler</a>：商业分析器。<a href="https://www.ej-technologies.com/products/jprofiler/overview.html">官网</a></li>
<li><a href="http://hao.jobbole.com/latencyutils/">LatencyUtils</a>：测量和报告延迟的工具。<a href="https://github.com/LatencyUtils/LatencyUtils">官网</a></li>
<li><a href="http://hao.jobbole.com/visualvm/">VisualVM</a>：对运行中的应用程序信息提供了可视化界面。<a href="http://visualvm.java.net/">官网</a></li>
<li><a href="http://hao.jobbole.com/yourkit-java-profiler/">YourKit Java Profiler</a>：商业分析器。<a href="https://www.yourkit.com/features/">官网</a></li>
</ul>
<h3 id="user-content-reactive-libraries"><a id="user-content-响应式开发库" class="anchor" href="#响应式开发库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>响应式开发库</h3>
<p><em>用来开发响应式应用程序的开发库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/reactive-streams/">Reactive Streams</a>：异步流处理标准，支持非阻塞式反向压力（backpressure）。<a href="https://github.com/reactive-streams/reactive-streams-jv/">官网</a></li>
<li><a href="http://hao.jobbole.com/reactor/">Reactor</a>：构建响应式快速数据（fast-data）应用程序的开发库。<a href="http://projectreactor.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/rxjava/">RxJava</a>：通过JVM可观察序列（observable sequence）构建异步和基于事件的程序。<a href="https://github.com/ReactiveX/RxJava">官网</a></li>
</ul>
<h3 id="user-content-rest-frameworks"><a id="user-content-rest框架" class="anchor" href="#rest框架" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>REST框架</h3>
<p><em>用来创建RESTful 服务的框架。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/dropwizard/">Dropwizard</a>：偏向于自己使用的Web框架。用来构建Web应用程序，使用了Jetty、Jackson、Jersey和Metrics。<a href="https://dropwizard.github.io/drpwizard/">官网</a></li>
<li><a href="http://hao.jobbole.com/feign/">Feign</a>：受Retrofit、JAXRS-2.0和WebSocket启发的HTTP客户端连接器（binder）。<a href="https://github.com/Netflix/feign">官网</a></li>
<li>Jersey：JAX-RS参考实现。<a href="https://jersey.java.net/">官网</a></li>
<li><a href="http://hao.jobbole.com/resteasy/">RESTEasy</a>：经过JAX-RS规范完全认证的可移植实现。<a href="http://resteasy.jboss.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/restexpress/">RestExpress</a>：一个Java类型安全的REST客户端。<a href="https://github.com/RestExpress/RestExpress">官网</a></li>
<li><a href="http://hao.jobbole.com/restx/">RestX</a>：基于注解处理和编译时源码生成的框架。<a href="http://restx.io">官网</a></li>
<li><a href="http://hao.jobbole.com/retrofit/">Retrofit</a>：类型安全的REST客户端。<a href="http://square.github.io/retrofit/">官网</a></li>
<li><a href="http://hao.jobbole.com/sparkjava/">Spark</a>：受到Sinatra启发的Java REST框架。<a href="http://sparkjava.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/swagger/">Swagger</a>：Swagger是一个规范且完整的框架，提供描述、生产、消费和可视化RESTful Web Service。<a href="http://swagger.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/bladejava/">Blade</a>：国人开发的一个轻量级的MVC框架. 它拥有简洁的代码，优雅的设计。<a href="https://github.com/biezhi/blade">官网</a></li>
</ul>
<h3 id="user-content-science"><a id="user-content-科学计算与分析" class="anchor" href="#科学计算与分析" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>科学计算与分析</h3>
<p><em>用于科学计算和分析的函数库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/datamelt/">DataMelt</a>：用于科学计算、数据分析及数据可视化的开发环境。<a href="http://jwork.org/dmelt/">官网</a></li>
<li><a href="http://hao.jobbole.com/jgrapht/">JGraphT</a>：支持数学图论对象和算法的图形库。<a href="https://github.com/jgrapht/jgrapht">官网</a></li>
<li><a href="http://hao.jobbole.com/jscience/">JScience</a>：用来进行科学测量和单位的一组类。<a href="http://jscience.org/">官网</a></li>
</ul>
<h3 id="user-content-search"><a id="user-content-搜索引擎" class="anchor" href="#搜索引擎" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>搜索引擎</h3>
<p><em>文档索引引擎，用于搜索和分析。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/solr/">Apache Solr</a>：一个完全的企业搜索引擎。为高吞吐量通信进行了优化。<a href="http://lucene.apache.org/solr/">官网</a></li>
<li>Elasticsearch：一个分布式、支持多租户（multitenant）全文本搜索引擎。提供了RESTful Web接口和无schema的JSON文档。<a href="http://www.elsticsearch.org/">官网</a></li>
<li>Apache Lucene：是一个开放源代码的全文检索引擎工具包，是一个全文检索引擎的架构，提供了完整的查询引擎和索引引擎，部分文本分析引擎。<a href="http://lucene.apache.org/">官网</a></li>
</ul>
<h3 id="user-content-security"><a id="user-content-安全" class="anchor" href="#安全" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>安全</h3>
<p><em>用于处理安全、认证、授权或会话管理的函数库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/shiro/">Apache Shiro</a>：执行认证、授权、加密和会话管理。<a href="http://shiro.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/bouncy-castle/">Bouncy Castle</a>，涵盖了从基础的帮助函数到PGP/SMIME操作。<a href="https://www.bouncycastle.org/java.html">官网</a>：多途加密开发库。支持JCA提供者（JCA provider)</li>
<li><a href="http://hao.jobbole.com/cryptomator/">Cryptomator</a>：在云上进行客户端跨平台透明加密。<a href="https://cryptomator.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/keycloak/">Keycloak</a>：为浏览器应用和RESTful Web Service集成SSO和IDM。目前还处于beta版本，但是看起来非常有前途。<a href="http://keycloak.jboss.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/picketlink/">PicketLink</a>：PicketLink是一个针对Java应用进行安全和身份认证管理的大型项目（Umbrella Project）。<a href="http://picketlink.org/">官网</a></li>
</ul>
<h3 id="user-content-serialization"><a id="user-content-序列化" class="anchor" href="#序列化" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>序列化</h3>
<p><em>用来高效处理序列化的函数库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/flatbuffers/">FlatBuffers</a>：高效利用内存的序列化函数库，无需解包和解析即可高效访问序列化数据。<a href="https://github.com/google/flatbuffers">官网</a></li>
<li><a href="http://hao.jobbole.com/kryo/">Kryo</a>：快速、高效的对象图形序列化框架。<a href="https://github.com/EsotericSoftware/kryo">官网</a></li>
<li><a href="http://hao.jobbole.com/fst/">FST</a>：提供兼容JDK的高性能对象图形序列化。<a href="https://github.com/RuedigerMoeller/fast-serialization">官网</a></li>
<li><a href="http://hao.jobbole.com/messagepack/">MessagePack</a>：一种高效的二进制序列化格式。<a href="https://github.com/msgpack/msgpack-java">官网</a></li>
</ul>
<h3 id="user-content-server"><a id="user-content-应用服务器" class="anchor" href="#应用服务器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>应用服务器</h3>
<p><em>用来部署应用程序的服务器。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/apache-tomcat/">Apache Tomcat</a>：针对Servlet和JSP的应用服务器，健壮性好且适用性强。<a href="http://tomcat.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/tomee/">Apache TomEE</a>：Tomcat加Java EE。<a href="http://tomee.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/jetty/">Jetty</a>：轻量级、小巧的应用服务器，通常会嵌入到项目中。<a href="http://www.eclipse.org/jetty/">官网</a></li>
<li><a href="http://hao.jobbole.com/websphere-liberty/">WebSphere Liberty</a>：轻量级、模块化应用服务器，由IBM开发。<a href="https://developer.ibm.com/wasdev/">官网</a></li>
<li><a href="http://hao.jobbole.com/wildfly/">WildFly</a>：之前被称作JBoss，由Red Hat开发。支持很多Java EE功能。<a href="http://www.wildfly.org/">官网</a></li>
</ul>
<h3 id="user-content-template-engine"><a id="user-content-模板引擎" class="anchor" href="#模板引擎" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>模板引擎</h3>
<p><em>在模板中替换表达式的工具。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/velocity/">Apache Velocity</a>：提供HTML页面模板、email模板和通用开源代码生成器模板。<a href="http://velocity.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/freemarker/">FreeMarker</a>：通用模板引擎，不需要任何重量级或自己使用的依赖关系。<a href="http://freemarker.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/handlebars-java/">Handlebars.java</a>：使用Java编写的模板引擎，逻辑简单，支持语义扩展（semantic Mustache）。<a href="http://jknack.github.io/handlebars.java/">官网</a></li>
<li><a href="http://hao.jobbole.com/thymeleaf/">Thymeleaf</a>：旨在替换JSP，支持XML文件的工具。<a href="http://www.thymeleaf.org/">官网</a></li>
</ul>
<h3 id="user-content-testing"><a id="user-content-测试" class="anchor" href="#测试" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>测试</h3>
<p><em>测试内容从对象到接口，涵盖性能测试和基准测试工具。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/jmeter/">Apache JMeter</a>：功能性测试和性能评测。<a href="http://jmeter.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/arquillian/">Arquillian</a>：集成测试和功能行测试平台，集成Java EE容器。<a href="http://arquillian.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/assertj/">AssertJ</a>：支持流式断言提高测试的可读性。<a href="http://joel-costigliola.github.io/assertj/">官网</a></li>
<li><a href="http://hao.jobbole.com/awaitility/">Awaitility</a>：用来同步异步操作的DSL。<a href="https://github.com/jayway/awaitility">官网</a></li>
<li><a href="http://hao.jobbole.com/cucumber-jvm/">Cucumber</a>：BDD测试框架。<a href="https://github.com/cucumber/cucumber-jvm">官网</a></li>
<li>Gatling：设计为易于使用、可维护的和高性能负载测试工具。<a href="http://gatling.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/hamcrest/">Hamcrest</a>：可用来灵活创建意图（intent）表达式的匹配器。<a href="http://hamcrest.org/JavaHamcrest/">官网</a></li>
<li>JMockit：用来模拟静态、final方法等。<a href="http://jmockit.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/junit/">JUnit</a>：通用测试框架。<a href="http://junit.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/mockito/">Mockito</a>：在自动化单元测试中创建测试对象，为TDD或BDD提供支持。<a href="https://github.com/mockito/mockito">官网</a></li>
<li><a href="http://hao.jobbole.com/powermock/">PowerMock</a>： 支持模拟静态方法、构造函数、final类和方法、私有方法以及移除静态初始化器的模拟工具。<a href="https://github.com/jayway/powermock">官网</a></li>
<li><a href="http://hao.jobbole.com/rest-assured/">REST Assured</a>：为REST/HTTP服务提供方便测试的Java DSL。<a href="https://github.com/jayway/rest-assured">官网</a></li>
<li><a href="http://hao.jobbole.com/selenide/">Selenide</a>：为Selenium提供精准的周边API，用来编写稳定且可读的UI测试。<a href="http://selenide.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/selenium/">Selenium</a>：为Web应用程序提供可移植软件测试框架。<a href="http://docs.seleniumhq.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/spock/">Spock</a>：JUnit-compatible framework featuring an expressive Groovy-derived specification language.<a href="http://docs.spockframework.org/">官网</a>兼容JUnit框架，支持衍生的Groovy范的语言。</li>
<li><a href="http://hao.jobbole.com/testng/">TestNG</a>：测试框架。<a href="http://testng.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/truth/">Truth</a>：Google的断言和命题（proposition）框架。<a href="https://github.com/google/truth">官网</a></li>
<li><a href="http://hao.jobbole.com/unitils/">Unitils</a>：模块化测试函数库，支持单元测试和集成测试。<a href="http://www.unitils.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/wiremock/">WireMock</a>：Web Service测试桩（Stub）和模拟函数。<a href="http://wiremock.org/">官网</a></li>
</ul>
<h3 id="user-content-utility"><a id="user-content-通用工具库" class="anchor" href="#通用工具库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>通用工具库</h3>
<p><em>通用工具类函数库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/apache-commons/">Apache Commons</a>：提供各种用途的函数，比如配置、验证、集合、文件上传或XML处理等。<a href="http://commons.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/args4j/">args4j</a>：命令行参数解析器。<a href="http://args4j.kohsuke.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/crash/">CRaSH</a>：为运行进行提供CLI。<a href="http://www.crashub.org">官网</a></li>
<li><a href="http://hao.jobbole.com/gephi/">Gephi</a>：可视化跨平台网络图形化操作程序。<a href="https://github.com/gephi/gephi/">官网</a></li>
<li><a href="http://hao.jobbole.com/guava/">Guava</a>：集合、缓存、支持基本类型、并发函数库、通用注解、字符串处理、I/O等。<a href="https://github.com/google/guava">官网</a></li>
<li><a href="http://hao.jobbole.com/jade/">JADE</a>：构建、调试多租户系统的框架和环境。<a href="http://jade.tilab.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/javatuples/">javatuples</a>：正如名字表示的那样，提供tuple支持。尽管目前tuple的概念还有留有争议。<a href="http://www.javatuples.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/jcommander/">JCommander</a>：命令行参数解析器。<a href="http://jcommander.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/protege/">Protégé</a>：提供存在论（ontology）编辑器以及构建知识系统的框架。<a href="http://protege.stanford.edu/">官网</a></li>
</ul>
<h3 id="user-content-web-crawling"><a id="user-content-网络爬虫" class="anchor" href="#网络爬虫" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>网络爬虫</h3>
<p><em>用于分析网站内容的函数库。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/nutch/">Apache Nutch</a>：可用于生产环境的高度可扩展、可伸缩的网络爬虫。<a href="http://nutch.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/crawler4j/">Crawler4j</a>：简单的轻量级网络爬虫。<a href="https://github.com/yasserg/crawler4j">官网</a></li>
<li><a href="http://hao.jobbole.com/jsoup/">JSoup</a>：刮取、解析、操作和清理HTML。<a href="http://jsoup.org/">官网</a></li>
<li><a href="https://github.com/code4craft/webmagic/">webmagic</a>：一个可扩展的Java爬虫框架，架构类似Python的Scrapy。</li>
</ul>
<h3 id="user-content-web-frameworks"><a id="user-content-web框架" class="anchor" href="#web框架" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Web框架</h3>
<p><em>用于处理Web应用程序不同层次间通讯的框架。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/apache-tapestry/">Apache Tapestry</a>：基于组件的框架，使用Java创建动态、强健的、高度可扩展的Web应用程序。<a href="http://tapestry.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/apache-wicket/">Apache Wicket</a>：基于组件的Web应用框架，与Tapestry类似带有状态显示GUI。<a href="http://wicket.apache.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/gwt/">Google Web Toolkit</a>：一组Web开发工具集，包含在客户端将Java代码转为JavaScript的编译器、XML解析器、RCP <a href="http://www.gwtproject.org/">官网</a>API、JUnit集成、国际化支持和GUI控件。</li>
<li><a href="http://hao.jobbole.com/grails/">Grails</a>：Groovy框架，旨在提供一个高效开发环境，使用约定而非配置、没有XML并支持混入（mixin）。<a href="https://grails.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/ninja/">Ninja</a>：Java全栈Web开发框架。非常稳固、快速和高效。<a href="http://www.ninjaframework.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/pippo/">Pippo</a>：小型、高度模块化的类Sinatra框架。<a href="http://www.pippo.ro/">官网</a></li>
<li><a href="http://hao.jobbole.com/play-framework/">Play</a>：使用约定而非配置，支持代码热加载并在浏览器中显示错误。<a href="https://www.playframework.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/primefaces/">PrimeFaces</a>：JSF框架，提供免费和带支持的商业版本。包括若干前端组件。<a href="http://primefaces.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/ratpack/">Ratpack</a>：一组Java开发函数库，用于构建快速、高效、可扩展且测试完备的HTTP应用程序。<a href="https://ratpack.io/">官网</a></li>
<li><a href="http://hao.jobbole.com/spring-boot/">Spring Boot</a>：微框架，简化了Spring新程序的开发过程。<a href="http://projects.spring.io/spring-boot/">官网</a></li>
<li><a href="http://hao.jobbole.com/spring-framework/">Spring</a>：旨在简化Java EE的开发过程，提供依赖注入相关组件并支持面向切面编程。<a href="http://projects.spring.io/spring-framework/">官网</a></li>
<li><a href="http://hao.jobbole.com/vaadin/">Vaadin</a>：基于GWT构建的事件驱动框架。使用服务端架构，客户端使用Ajax。<a href="https://vaadin.com/">官网</a></li>
<li>Blade：国人开发的一个轻量级的MVC框架. 它拥有简洁的代码，优雅的设计。<a href="https://github.com/biezhi/blade">官网</a></li>
</ul>
<h3 id="user-content-Business-Process-Management"><a id="user-content-业务流程管理套件" class="anchor" href="#业务流程管理套件" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>业务流程管理套件</h3>
<p><em>流程驱动的软件系统构建。</em></p>
<ul>
<li><a href="http://hao.jobbole.com/jbpm/">jBPM</a>：非常灵活的业务流程管理框架，致力于构建开发与业务分析人员之间的桥梁。<a href="http://www.jbpm.org/">官网</a></li>
<li>Activity：轻量级工作流和业务流程管理框架。<a href="http://www.activiti.org/">官网</a> <a href="https://github.com/Activiti/Activiti">github</a></li>
</ul>

## 三、JS

<hr>
<h2 id="user-content-package-managers"><a id="user-content-包管理器" class="anchor" href="#包管理器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>包管理器</h2>
<p>管理着 JavaScript 库，并提供读取和打包它们的工具。</p>
<ul>
<li>npm：npm 是 JavaScript 的包管理器。<a href="https://www.npmjs.com/">官网</a></li>
<li>Bower：一个 web 应用的包管理器。<a href="https://github.com/bower/bower">官网</a></li>
<li>component：能构建更好 web 应用的客户端包管理器。<a href="https://github.com/componentjs/component">官网</a></li>
<li>spm：全新的静态包管理器。<a href="https://github.com/spmjs/spm">官网</a></li>
<li>jam：一个专注于浏览器端和兼容 RequireJS 的包管理器。<a href="https://github.com/caolan/jam">官网</a></li>
<li>jspm：流畅的浏览器包管理器。<a href="https://github.com/jspm/jspm-cli">官网</a></li>
<li>Ender：没有库文件的程序库。<a href="https://github.com/ender-js/Ender">官网</a></li>
<li>volo：以项目模板、添加依赖项与自动化生成的方式创建前端项目。<a href="https://github.com/volojs/volo">官网</a> </li>
<li>Duo：一个整合 Component、Browserify 和 Go <a href="https://github.com/duojs/duo">官网</a>的最佳思想，使开发者能快速方便地组织和编写前端代码的下一代包管理器。</li>
</ul>
<h2 id="user-content-loaders"><a id="user-content-加载器" class="anchor" href="#加载器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>加载器</h2>
<p>JavaScript 的模块或加载系统。</p>
<ul>
<li>RequireJS：JavaScript 文件和模块的加载器。<a href="https://github.com/jrburke/requirejs">官网</a></li>
<li>browserify：在浏览器端以 node.js 的方式 require()。<a href="https://github.com/substack/node-browserify">官网</a></li>
<li>SeaJS：用于 Web 的模块加载器。<a href="https://github.com/seajs/seajs">官网</a></li>
<li>HeadJS：HEAD 的唯一脚本。<a href="https://github.com/headjs/headjs">官网</a></li>
<li>curl：小巧、快速且易扩展的模块加载器，它能处理 AMD、CommonJS Modules/1.1、CSS、HTML/text 和历史脚本。<a href="https://github.com/cujojs/curl">官网</a></li>
<li>lazyload：小巧且无依赖的异步 JavaScript 和 CSS 加载器。<a href="https://github.com/rgrove/lazyload/">官网</a></li>
<li>script.js：异步 JavaScript 加载器和依赖管理器。<a href="https://github.com/ded/script.js">官网</a></li>
<li>systemjs：AMD、CJS（commonJS） 和符合 ES6 规范的模块加载器。<a href="https://github.com/systemjs/systemjs">官网</a></li>
<li>LodJS：基于 AMD 的模块加载器。<a href="https://github.com/yanhaijing/lodjs">官网</a></li>
<li>ESL：浏览器端的模块加载器，支持延迟定义和 AMD。<a href="https://github.com/ecomfe/esl">官网</a></li>
<li>modulejs：轻量的 JavaScript 模块系统。<a href="https://github.com/lrsjng/modulejs">官网</a></li>
</ul>
<h2 id="user-content-bundlers"><a id="user-content-打包工具" class="anchor" href="#打包工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>打包工具</h2>
<ul>
<li>browserify ：Browserify 让你能在浏览器端使用 require('modules') ，打包所有依赖。<a href="https://github.com/substack/node-browserify">官网</a></li>
<li>webpack：为浏览器打包 CommonJs/AMD 模块。<a href="https://github.com/webpack/webpack">官网</a></li>
<li>gulp：用自动化构建工具增强你的工作流程！<a href="http://gulpjs.com/">官网</a></li>
</ul>
<h2 id="user-content-testing-frameworks"><a id="user-content-测试框架" class="anchor" href="#测试框架" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>测试框架</h2>
<h3><a id="user-content-框架" class="anchor" href="#框架" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>框架</h3>
<ul>
<li>mocha：适用于 node.js 和浏览器、简易、灵活、有趣的 JavaScript 测试框架。<a href="https://github.com/mochajs/mocha">官网</a></li>
<li>jasmine：简单无 DOM 的 JavaScript 测试框架。<a href="https://github.com/jasmine/jasmine">官网</a></li>
<li>qunit：一个易于使用的 JavaScript 单元测试框架。<a href="https://github.com/jquery/qunit">官网</a></li>
<li>jest：简单的 JavaScript 单元测试框架。<a href="https://github.com/facebook/jest">官网</a></li>
<li>prova：基于 Tape 和 Browserify 的测试运行器，它适用于 Node &amp; 浏览器。<a href="https://github.com/azer/prova">官网</a></li>
<li>DalekJS：自动化且跨浏览器的 JavaScript 功能测试框架。<a href="https://github.com/dalekjs/dalek">官网</a></li>
</ul>
<h3><a id="user-content-断言" class="anchor" href="#断言" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>断言</h3>
<ul>
<li>chai：适用于 node.js 和浏览器的 BDD / TDD 断言框架，并能搭配其它测试框架使用。<a href="https://github.com/chaijs/chai">官网</a></li>
<li>Sinon.JS：对 JavaScript 进行 spies、stubs 和 mock 测试。<a href="https://github.com/sinonjs/sinon">官网</a></li>
<li>expect.js：简约的、适用于 Node.js 和浏览器端的 BDD 式断言工具。<a href="https://github.com/Automattic/expect.js">官网</a></li>
<li>should.js：适用于 Node.js 的 BDD 式断言工具。<a href="https://github.com/tj/should.js">官网</a></li>
</ul>
<h3><a id="user-content-覆盖率" class="anchor" href="#覆盖率" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>覆盖率</h3>
<ul>
<li>istanbul：另一个 JS 代码覆盖率检测工具。<a href="https://github.com/gotwarlost/istanbul">官网</a></li>
<li>blanket：一个简单的代码覆盖率检测库。它的设计理念是易于安装和使用，且可用于浏览器端和 node.js。<a href="https://github.com/alex-seville/blanket">官网</a></li>
<li>JSCover：JSCover 是一个检测 JavaScript 程序代码覆盖率的工具。<a href="https://github.com/tntim96/JSCover">官网</a></li>
</ul>
<h3><a id="user-content-运行器" class="anchor" href="#运行器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>运行器</h3>
<ul>
<li>phantomjs：脚本化的 Headless WebKit。<a href="https://github.com/ariya/phantomjs">官网</a></li>
<li>slimerjs：一个内核为 Gecko 的类似 PhantomJS 工具。<a href="https://github.com/laurentj/slimerjs">官网</a></li>
<li>casperjs：基于 PhantomJS 和 Slimer JS 的导航脚本和测试工具。<a href="https://github.com/n1k0/casperjs">官网</a> </li>
<li>zombie：基于 node.js 、快速、全栈且无图形界面的浏览器的测试工具。<a href="https://github.com/assaf/zombie">官网</a></li>
<li>totoro：一个简单可靠且能跨浏览器运行的测试工具。<a href="https://github.com/totorojs/totoro">官网</a></li>
<li>karma：一个优秀的的 JavaScript 测试运行器。<a href="https://github.com/karma-runner/karma">官网</a></li>
<li>nightwatch：基于 node.js 和 selenium webdriver 的图形界面自动化测试框架。<a href="https://github.com/nightwatchjs/nightwatch">官网</a></li>
<li>intern：下一代 JavaScript 代码测试栈。<a href="https://github.com/theintern/intern">官网</a></li>
<li>yolpo：在浏览器逐句执行的 JavaScript 解释器。<a href="http://www.yolpo.com/">官网</a></li>
</ul>
<h2 id="user-content-qa-tools"><a id="user-content-qa-工具" class="anchor" href="#qa-工具" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>QA 工具</h2>
<ul>
<li>JSHint：JSHint 是一个有助于发现 JavaScript 代码错误和潜在问题的工具。<a href="https://github.com/jshint/jshint/">官网</a></li>
<li>jscs：JavaScript 代码风格检测工具。<a href="https://github.com/jscs-dev/node-jscs">官网</a></li>
<li>jsfmt：格式化、搜索和改写 JavaScript。<a href="https://github.com/rdio/jsfmt">官网</a></li>
<li>jsinspect：检测复制粘贴和结构类似的代码。<a href="https://github.com/danielstjules/jsinspect">官网</a></li>
<li>buddy.js：发现 JavaScript 代码里的 <a href="https://zh.wikipedia.org/wiki/%E9%AD%94%E8%A1%93%E6%95%B8%E5%AD%97">魔术数字</a>。<a href="https://github.com/danielstjules/buddy.js">官网</a></li>
<li>ESLint：完全插件化的工具，能在 JavaScript 中识别和记录模式。<a href="https://github.com/eslint/eslint">官网</a></li>
<li>JSLint ：高标准、严格和固执的代码质量工具，旨在只保持语言的优良部分。<a href="https://github.com/douglascrockford/JSLint">官网</a></li>
</ul>
<h2 id="user-content-mvc-frameworks-and-libraries"><a id="user-content-mvc-框架和库" class="anchor" href="#mvc-框架和库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>MVC 框架和库</h2>
<ul>
<li><a href="http://hao.jobbole.com/angularjs/">angular.js</a>：为网络应用增强 HTML。<a href="https://github.com/angular/angular.js">官网</a></li>
<li>aurelia：一个适用于移动设备、桌面电脑和 web 的客户端 JavaScript 框架。<a href="http://aurelia.io/">官网</a></li>
<li>backbone：给你的 JS 应用加入带有 Models、Views、Collections 和 Events 的 Backbone。<a href="https://github.com/jashkenas/backbone">官网</a></li>
<li>batman.js：最适合 Rails 开发者的 JavaScript 框架。<a href="http://batmanjs.org/">官网</a></li>
<li>ember.js：一个旨在创建非凡 web 应用的 JavaScript 框架。<a href="https://github.com/emberjs/ember.js">官网</a></li>
<li>meteor：一个超简单的、数据库无处不在的、只传输数据的纯 JavaScript web 框架。<a href="https://github.com/meteor/meteor">官网</a></li>
<li>ractive：新一代 DOM 操作。<a href="https://github.com/ractivejs/ractive">官网</a></li>
<li>vue：一个用于构建可交互界面的、直观快速和可组合的 MVVM 框架。<a href="https://github.com/vuejs/vue">官网</a> </li>
<li>knockout：Knockout 用 JavaScript 让创建响应式的富 UI 更加容易。<a href="https://github.com/knockout/knockout">官网</a> </li>
<li>spine：构建 JavaScript 应用的轻量 MVC 库。<a href="https://github.com/spine/spine">官网</a></li>
<li>espresso.js：一个极小的、用于制作用户界面的 JavaScript 库。<a href="https://github.com/techlayer/espresso.js">官网</a></li>
<li>canjs：让 JS 更好、更快、更简单。<a href="https://github.com/canjs/canjs">官网</a></li>
<li>react：用于建构用户界面的库。它是声明式的、高效的和极度灵活的，并使用虚拟 DOM 作为其不同的实现。<a href="https://facebook.github.io/react/">官网</a></li>
<li>react-native：一个用 React 构建原生应用的框架。<a href="https://github.com/facebook/react-native">官网</a></li>
<li>riot：类 React 库，但很轻量。<a href="https://github.com/riot/riot">官网</a></li>
<li>thorax：加强你的 Backbone。<a href="https://github.com/walmartlabs/thorax">官网</a></li>
<li>chaplin：使用 Backbone.js 库的 JavaScript 应用架构。<a href="https://github.com/chaplinjs/chaplin">官网</a></li>
<li>marionette：一个 Backbone.js 的复合应用程序库，旨在简化大型 JavaScript 应用结构。<a href="https://github.com/marionettejs/backbone.marionette">官网</a></li>
<li>ripple：一个小巧的、用于构建响应界面的基础框架。<a href="https://github.com/ripplejs/ripple">官网</a></li>
<li>rivets：轻量却拥有强大的数据绑定和模板解决方案<a href="https://github.com/mikeric/rivets">官网</a></li>
<li>derby：让编写实时和协同应用更简单的 MVC 框架，能够在 Node.js 和浏览器同时运行。<a href="https://github.com/derbyjs/derby">官网</a>
<ul>
<li>derby-awesome：很棒的 derby 组件集合。<a href="https://github.com/russll/awesome-derby">官网</a></li>
</ul>
</li>
<li><a href="http://hao.jobbole.com/way-js/">way.js</a>：简单、轻量、持久化的双向数据绑定。<a href="https://github.com/gwendall/way.js">官网</a></li>
<li>mithril.js：Mithril 是一个客户端 MVC 框架（轻量、强大和快速）<a href="https://github.com/lhorie/mithril.js">官网</a></li>
<li>jsblocks：jsblocks 是一个更好的 MV-ish 框架。<a href="https://github.com/astoilkov/jsblocks">官网</a></li>
<li>LiquidLava：易懂的、用于构建用户界面的 MVC 框架。<a href="http://www.lava-framework.com/">官网</a></li>
<li><a href="http://hao.jobbole.com/electron/">Electron</a>：用Html、CSS和JavaScript构建跨平台的客户端应用程序。<a href="http://electron.atom.io/">官网</a>、<a href="https://github.com/electron/electron">GitHub</a></li>
</ul>
<h2 id="user-content-node-powered-cms-frameworks"><a id="user-content-基于-node-的-cms-框架" class="anchor" href="#基于-node-的-cms-框架" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>基于 Node 的 CMS 框架</h2>
<ul>
<li>KeystoneJS：强大的 CMS 和 web 应用框架。<a href="https://github.com/keystonejs/keystone">官网</a></li>
<li>Reaction Commerce：拥有实时的架构和设计的响应式（reactive） CMS。<a href="https://github.com/reactioncommerce/reaction">官网</a></li>
<li>Ghost：简单、强大的发布平台。<a href="https://github.com/tryghost/Ghost">官网</a></li>
<li>Apostrophe：提供内容编辑和基本服务的 CMS。<a href="https://github.com/punkave/apostrophe">官网</a></li>
<li>We.js：适用于实时应用、网站或博客的框架。<a href="https://github.com/wejs/we/">官网</a></li>
<li>Hatch.js：拥有社交特性的 CMS 平台。<a href="https://github.com/inventures/hatchjs">官网</a></li>
<li>TaracotJS：拥有快速、极简风格特点且基于Node.js 的 CMS。<a href="https://github.com/xtremespb/taracotjs-generator/">官网</a></li>
<li>Nodizecms：为 CoffeeScript 爱好者准备的 CMS。<a href="https://github.com/nodize/nodizecms">官网</a></li>
<li>Cody：拥有所见即所得的编辑器的 CMS。<a href="https://github.com/jcoppieters/cody">官网</a></li>
<li>PencilBlue：CMS 和博客平台。<a href="https://github.com/pencilblue/pencilblue/">官网</a></li>
</ul>
<h2 id="user-content-templating-engines"><a id="user-content-模板引擎" class="anchor" href="#模板引擎" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>模板引擎</h2>
<p>模板引擎允许您执行字符串插值。</p>
<ul>
<li>mustache.js：是 JavaScript 中带有 {{mustaches}} 的最简模板。<a href="https://github.com/janl/mustache.js">官网</a></li>
<li>handlebars.js：是 Mustache 模板语言的扩展。<a href="https://github.com/wycats/handlebars.js/">官网</a></li>
<li>hogan.js：是 Mustache 模板语言的编译器。<a href="https://github.com/twitter/hogan.js">官网</a></li>
<li>doT：最快速简洁的 JavaScript 模板引擎，适用于 nodejs 和浏览器。<a href="https://github.com/olado/doT">官网</a></li>
<li>dustjs：适用于浏览器和 node.js 的异步模板。<a href="https://github.com/linkedin/dustjs/">官网</a></li>
<li>eco：嵌入式的 CoffeeScript 模板。<a href="https://github.com/sstephenson/eco/">官网</a></li>
<li>JavaScript-Templates：轻量（小于 1KB）、快速且无依赖的强大 JavaScript 模版引擎。<a href="https://github.com/blueimp/JavaScript-Templates">官网</a></li>
<li>t.js：小巧的 JavaScript 模板框架，压缩后约为 400 字节。<a href="https://github.com/jasonmoo/t.js">官网</a></li>
<li>Jade：健壮的、优雅且功能丰富的 nodejs 模板引擎。<a href="https://github.com/pugjs/jade">官网</a></li>
<li>EJS：高效的 JavaScript 模板。<a href="https://github.com/mde/ejs">官网</a></li>
<li>xtemplate：可扩展的模板引擎，适用于 node 和浏览器。<a href="https://github.com/xtemplate/xtemplate">官网</a></li>
<li>marko：快速轻量且基于 HTML 的模板引擎，支持异步、流、自定义标签和 CommonJS 模编译后输出。适用于 Node.js <a href="https://github.com/marko-js/marko">官网</a>和浏览器。</li>
</ul>
<h2 id="user-content-data-flow"><a id="user-content-flux" class="anchor" href="#flux" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Flux</h2>
<p>Flux是Facebook用来构建客户端Web应用的应用架构</p>
<ul>
<li>Reflux是根据React的flux创建的单向数据流类库。<a href="https://github.com/reflux/refluxjs">官网</a></li>
<li>Redux是可预测javascript应用程序状态的容器。<a href="http://redux.js.org/">官网</a></li>
<li>Mobx是通过透明的函数响应式编程实现简单，可扩展的状态管理库。<a href="https://mobx.js.org/">官网</a></li>
<li>Dva是基于Redux, Redux-saga 和 <a href="mailto:react-router@2.x">react-router@2.x</a>的轻量级的框架。<a href="https://github.com/dvajs/dva">官网</a></li>
</ul>
<h2 id="user-content-data visualization"><a id="user-content-数据可视化" class="anchor" href="#数据可视化" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据可视化</h2>
<p>Web 数据可视化工具</p>
<ul>
<li>d3：一个对 HTML 和 SVG 进行可视化的 JavaScript 库。<a href="https://github.com/mbostock/d3">官网</a></li>
<li>metrics-graphics：更简洁和拥有更规范的数据图表布局优化算法的库。<a href="https://github.com/mozilla/metrics-graphics">官网</a></li>
<li>pykcharts.js：经过精心设计后，去除 d3.js 复杂性的 d3.js 图表库。<a href="https://github.com/pykih/PykCharts.js">官网</a></li>
<li><a href="http://hao.jobbole.com/three-js/">three.js</a>：JavaScript 3D 库。<a href="https://github.com/mrdoob/three.js">官网</a></li>
<li>Chart.js：简单的、基于 canvas 标签的 HTML5 图表库。<a href="https://github.com/nnnick/Chart.js">官网</a></li>
<li>paper.js：是矢量图形脚本中的瑞士军刀 —— 使用 HTML5 Canvas 将 Scriptographer  移植到 JavaScript <a href="https://github.com/paperjs/paper.js">官网</a>和浏览器。</li>
<li>fabric.js：JavaScript Canvas 库，SVG 与 Canvas 可以相互解析。<a href="https://github.com/kangax/fabric.js">官网</a></li>
<li>peity：进度条、线状和饼状图。<a href="https://github.com/benpickles/peity">官网</a></li>
<li>raphael：JavaScript 矢量库。<a href="https://github.com/DmitryBaranovskiy/raphael">官网</a></li>
<li>echarts：商业产品图表。<a href="https://github.com/ecomfe/echarts">官网</a></li>
<li>vis：动态的、基于浏览器的可视化库。<a href="https://github.com/almende/vis">官网</a></li>
<li>two.js：一个渲染器无关的适用于 web 的二维绘图 api 。<a href="https://github.com/jonobr1/two.js">官网</a></li>
<li>g.raphael：基于 Raphaël 图表库。<a href="https://github.com/DmitryBaranovskiy/g.raphael">官网</a></li>
<li>sigma.js：一个致力于图形绘画的 JavaScript 库。<a href="https://github.com/jacomyal/sigma.js">官网</a></li>
<li>arbor：一个使用 web workers 和 jQuery 的图形可视化库。<a href="https://github.com/samizdatco/arbor">官网</a></li>
<li>cubism：可视化时间序列的 D3 插件。<a href="https://github.com/square/cubism">官网</a></li>
<li>dc.js：与 crossfilter 无缝合作的多维图表绘制库，使用 d3.js 渲染。<a href="https://github.com/dc-js/dc.js">官网</a></li>
<li>vega：一套可视化语法。<a href="https://github.com/trifacta/vega">官网</a></li>
<li>processing.js：Processing.js 基于 Web 标准使数据可视化，而无需任何插件。<a href="http://processingjs.org/">官网</a></li>
<li>envisionjs：动态的 HTML5 可视化。<a href="https://github.com/HumbleSoftware/envisionjs">官网</a></li>
<li>rickshaw：用于构建交互式实时图表的 JavaScript 工具包。<a href="https://github.com/shutterstock/rickshaw">官网</a></li>
<li>flot：吸引人的、基于 jQuery 的 JavaScript 图表库。<a href="https://github.com/flot/flot">官网</a></li>
<li>morris.js：漂亮的时间序列线框图。<a href="https://github.com/morrisjs/morris.js">官网</a></li>
<li>nvd3：一个为 D3.js 构建可复用图表和图表组件的库。<a href="https://github.com/novus/nvd3">官网</a></li>
<li>svg.js：一个轻量的、用于操作和添加 SVG 动画的库。<a href="https://github.com/wout/svg.js">官网</a></li>
<li>heatmap.js：基于 HTML5 canvas 的热力图 JavaScript 库。<a href="https://github.com/pa7/heatmap.js">官网</a></li>
<li>jquery.sparkline：一个直接在浏览器端生成小型走势图的 jQuery 插件。<a href="https://github.com/gwatts/jquery.sparkline">官网</a></li>
<li>xCharts：一个基于 D3、用于构建自定义图表和图形的库。<a href="https://github.com/tenxer/xCharts">官网</a></li>
<li>trianglify：基于 d3.js 的低多边形（low poly）风格背景图片生成器。<a href="https://github.com/qrohlf/trianglify">官网</a></li>
<li>d3-cloud：创建词云（word cloud）效果的 JavaScript 库。<a href="https://github.com/jasondavies/d3-cloud">官网</a></li>
<li>d4：一个基于 D3 、友好、可复用的 DSL 图表库 。<a href="https://github.com/heavysixer/d4">官网</a></li>
<li>dimple.js：基于 d3 的简易商业分析图表库。<a href="http://dimplejs.org/">官网</a></li>
<li>chartist-js：简单的响应式图表。<a href="https://github.com/gionkunz/chartist-js">官网</a></li>
<li>epoch：一个通用的实时图表库。<a href="https://github.com/epochjs/epoch">官网</a></li>
<li>c3：基于 D3 的可复用图表库。<a href="https://github.com/masayuki0812/c3">官网</a></li>
<li>BabylonJS：一个运用 HTML5 和 WebGL 构建 3D 游戏的框架。<a href="https://github.com/BabylonJS/Babylon.js">官网</a></li>
<li>jquery.raty.js：一个星级评分插件。<a href="https://github.com/wbotelhos/raty">官网</a></li>
</ul>
<p>也有一些很棒的收费库，如 <a href="https://www.amcharts.com/">amchart</a>、<a href="https://plot.ly/">plotly</a> 和 <a href="http://www.highcharts.com/">highchart</a>。</p>
<h3 id="user-content-timeline"><a id="user-content-时间轴" class="anchor" href="#时间轴" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>时间轴</h3>
<ul>
<li>TimelineJS： 一个用 JavaScript 编写的可叙事时间轴库。<a href="https://github.com/NUKnightLab/TimelineJS">官网</a></li>
<li>timesheet.js：用于构建简单的 HTML5 &amp; CSS3 时间表的 JavaScript 库。<a href="https://github.com/semu/timesheet.js">官网</a></li>
</ul>
<h2 id="user-content-editors"><a id="user-content-编辑器" class="anchor" href="#编辑器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>编辑器</h2>
<ul>
<li>ace：Ace（Ajax.org Cloud9 Editor）。<a href="https://github.com/ajaxorg/ace">官网</a></li>
<li>CodeMirror：浏览器端的代码编辑器。<a href="https://github.com/codemirror/CodeMirror">官网</a></li>
<li>esprima：用于综合分析的 ECMAScript 解析器。<a href="https://github.com/ariya/esprima">官网</a></li>
<li><a href="http://hao.jobbole.com/quill/">quill</a>：一个带有 API 的跨浏览器富文本编辑器。(<a href="http://quilljs.com/">官网</a>)</li>
<li>medium-editor：Medium.com 所见即所得编辑器的克隆版。<a href="https://github.com/yabwe/medium-editor">官网</a></li>
<li>pen：享受在线编辑（支持 markdown）。<a href="https://github.com/sofish/pen">官网</a></li>
<li>jquery-notebook：一个易用的、简洁优雅的文本编辑器。灵感来源于 Medium 的魅力。<a href="https://github.com/raphaelcruzeiro/jquery-notebook">官网</a></li>
<li>bootstrap-wysiwyg：小巧的、兼容 bootstrap 的所见即所得的富文本编辑器。<a href="https://github.com/mindmup/bootstrap-wysiwyg">官网</a></li>
<li>ckeditor-releases：适用于每个人的 web 文本编辑器。<a href="https://github.com/ckeditor/ckeditor-releases">官网</a></li>
<li>editor：一个 markdown 编辑器，但仍在开发中。<a href="https://github.com/lepture/editor">官网</a></li>
<li>EpicEditor：一个可嵌入的 JavaScript Markdown <a href="https://github.com/OscarGodson/EpicEditor">官网</a>的编辑器，拥有全屏编辑、即时预览、自动保存草稿和离线支持等功能。</li>
<li>jsoneditor：查看、编辑和格式化 JSON 的 web 工具。<a href="https://github.com/josdejong/jsoneditor">官网</a></li>
<li>vim.js： 拥有持久化 ~/.vimrc 的 Vim 编辑器的 JavaScript 移植版本。<a href="https://github.com/coolwanglu/vim.js">官网</a></li>
<li>Squire：HTML5 富文本编辑器。<a href="https://github.com/neilj/Squire">官网</a></li>
<li>TinyMCE：JavaScript 富文本编辑器。<a href="https://github.com/tinymce/tinymce">官网</a></li>
<li>trix：由 Basecamp 制作，适用于每天写作的富文本编辑器。<a href="https://github.com/basecamp/trix">官网</a></li>
</ul>
<h3 id="user-content-files"><a id="user-content-文件" class="anchor" href="#文件" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>文件</h3>
<p>处理文件的库。</p>
<ul>
<li>Papa Parse：一款强大的 CSV 库，支持解析 CSV 文件/字符串，也能导出 CSV。<a href="https://github.com/mholt/PapaParse">官网</a></li>
<li>jBinary：对用声明式语法描述文件类型和数据结构的二进制文件，进行高级 I/O（加载、解析、操作、序列化、存储）操作。<a href="https://github.com/jDataView/jBinary">官网</a></li>
</ul>
<h3 id="user-content-functional-programming"><a id="user-content-函数式编程" class="anchor" href="#函数式编程" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>函数式编程</h3>
<p>函数式编程库扩展了 JavaScript 的能力。</p>
<ul>
<li><a href="http://hao.jobbole.com/underscore/">underscore</a>：JavaScript 的实用工具。<a href="https://github.com/jashkenas/underscore">官网</a></li>
<li><a href="http://hao.jobbole.com/lodash/">lodash</a>：提供一致性、可定制、高性能和额外功能的实用库。<a href="https://github.com/lodash/lodash">官网</a></li>
<li>Sugar：一个扩展了原生对象功能的 JavaScript 库。<a href="https://github.com/andrewplummer/Sugar">官网</a></li>
<li>lazy.js：类似 Underscore，但性能更优越<a href="https://github.com/dtao/lazy.js">官网</a></li>
<li>ramda：一个针对 JavaScript 程序员的实用函数库。<a href="https://github.com/CrossEye/ramda">官网</a></li>
<li>mout：模块化的 JavaScript 工具库。<a href="https://github.com/mout/mout">官网</a></li>
<li>mesh：流数据同步工具。<a href="https://github.com/crcn/mesh.js">官网</a></li>
</ul>
<h3 id="user-content-reactive-programming"><a id="user-content-响应式编程" class="anchor" href="#响应式编程" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>响应式编程</h3>
<p>响应式程序库扩展了 JavaScript 的能力。</p>
<ul>
<li>RxJs：对 JavaScript 进行响应式扩展。<a href="https://github.com/Reactive-Extensions/RxJS">官网</a></li>
<li>Bacon：JavaScript 的 FPR（函数式响应式编程）库。<a href="https://github.com/baconjs/bacon.js">官网</a></li>
<li>Kefir：受 Bacon.js 和 RxJS 启发的 FRP 库，专注于高性能和低内存消耗。<a href="https://github.com/pozadi/kefir">官网</a></li>
<li>Highland：对 JavaScript 实用工具的重新思考，Highland 能轻易地管理同步和异步信息，而且仅使用标准 JavaScript 和类 Node 流。<a href="http://highlandjs.org/">官网</a></li>
<li>Most.js：高性能 FRP 库。<a href="https://github.com/cujojs/most">官网</a></li>
</ul>
<h3 id="user-content-data-structure"><a id="user-content-数据结构" class="anchor" href="#数据结构" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据结构</h3>
<p>数据结构库用于构建一个更复杂的应用。</p>
<ul>
<li>immutable-js：不可变的数据集合，包括 Sequence、Range、Repeat、Map、OrderedMap、Set 和 sparse Vector。<a href="https://github.com/facebook/immutable-js">官网</a></li>
<li>mori：使用 ClojureScript 持久化数据结构和支持原生 JavaScript API 的库。<a href="https://github.com/swannodette/mori">官网</a></li>
<li>buckets：完整的、经过充分测试和记录数据结构的 JavaScript 库。<a href="https://github.com/mauriciosantos/Buckets-JS">官网</a></li>
<li>hashmap：简单的 hashmap 实现，支持任何类型的键值。<a href="https://github.com/flesler/hashmap">官网</a></li>
</ul>
<h3 id="user-content-date"><a id="user-content-日期" class="anchor" href="#日期" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>日期</h3>
<p>日期库。</p>
<ul>
<li>moment：解析、验证、操作和显示日期。<a href="https://github.com/moment/moment">官网</a></li>
<li>moment-timezone：基于 moment.js 的时区库。<a href="https://github.com/moment/moment-timezone">官网</a></li>
<li>jquery-timeago：一款支持自动更新模糊时间戳的 jQuery 插件（如："4 分钟之前"）。<a href="https://github.com/rmm5t/jquery-timeago">官网</a></li>
<li>timezone-js：让 JavaScript Date 对象拥有时区功能。使用 Olson zoneinfo 文件记录着时区数据。<a href="https://github.com/mde/timezone-js">官网</a></li>
<li>date：拥有人性化的 Date() 方法。<a href="https://github.com/MatthewMueller/date">官网</a></li>
<li>ms.js：小巧的毫秒转换工具。<a href="https://github.com/rauchg/ms.js">官网</a></li>
<li>timeago.js：一个非常轻量级(~1.7 Kb)的用于将时间转化成<code>xxx时间前</code>格式，例如：8分钟前。<a href="http://timeago.org">官网</a></li>
</ul>
<h3 id="user-content-string"><a id="user-content-字符串" class="anchor" href="#字符串" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>字符串</h3>
<p>字符串库。</p>
<ul>
<li>selecting：一个允许你获取用户选定文本的库。<a href="https://github.com/EvandroLG/selecting">官网</a></li>
<li>underscore.string：扩展了 Underscore.js 的字符串操作。<a href="https://github.com/epeli/underscore.string">官网</a></li>
<li>string.js：额外的 JavaScript 字符串方法。<a href="https://github.com/jprichardson/string.js">官网</a></li>
<li>he：健壮的 HTML 实体编码/解码器。<a href="https://github.com/mathiasbynens/he">官网</a></li>
<li>multiline：多行字符串。<a href="https://github.com/sindresorhus/multiline">官网</a></li>
<li>query-string：解析和字符串化 URL 查询字符串。<a href="https://github.com/sindresorhus/query-string">官网</a></li>
<li>URI.js：URL 操作库。<a href="https://github.com/medialize/URI.js/">官网</a> </li>
<li>jsurl：轻量的 URL 操作库。<a href="https://github.com/Mikhus/jsurl">官网</a></li>
<li>sprintf.js：实现字符串格式化。<a href="https://github.com/alexei/sprintf.js">官网</a></li>
<li>url-pattern：让 url 和其它字符串进行比正则表达式匹配更简单。字符串和数据可相互转化。<a href="https://github.com/snd/url-pattern">官网</a></li>
</ul>
<h3 id="user-content-number"><a id="user-content-数字" class="anchor" href="#数字" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数字</h3>
<ul>
<li>Numeral-js：对数字进行格式化和操作的库。<a href="https://github.com/adamwdraper/Numeral-js">官网</a></li>
<li>odometer：流畅的数字过渡效果。<a href="https://github.com/HubSpot/odometer">官网</a></li>
<li>accounting.js：对数字、金钱、货币进行格式化的轻量库——完全本地化和无依赖。<a href="https://github.com/josscrowcroft/accounting.js">官网</a></li>
<li>money.js：一个小巧（1kb）的货币转换库，适用于 web 和 nodeJS。<a href="https://github.com/josscrowcroft/money.js">官网</a></li>
<li>Fraction.js：一个有理数库。<a href="https://github.com/infusion/Fraction.js">官网</a></li>
<li>Complex.js： 一个复数库。<a href="https://github.com/infusion/Complex.js">官网</a></li>
<li>Polynomial.js：一个多项式库。<a href="https://github.com/infusion/Polynomial.js">官网</a></li>
</ul>
<h3 id="user-content-storage"><a id="user-content-存储" class="anchor" href="#存储" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>存储</h3>
<ul>
<li>store.js：为所有浏览器封装了 LocalStorage，而没有使用 cookies 和 flash。隐秘地使用 localStorage、globalStorage 和用户数据。<a href="https://github.com/marcuswestin/store.js">官网</a></li>
<li>localForage：改善后的离线存储。其封装了 IndexedDB、WebSQL 和 localStorage，拥有操作简单和强大的 API。<a href="https://github.com/mozilla/localForage">官网</a></li>
<li>jStorage：jStorage 是一个简单的键值对数据库，用于在浏览器端存储数据。<a href="https://github.com/andris9/jStorage">官网</a></li>
<li>cross-storage：获得权限后，能跨域名本地存储。<a href="https://github.com/zendesk/cross-storage">官网</a></li>
<li>basket.js：用 localStorage 加载和缓存脚本的资源加载器。<a href="https://github.com/addyosmani/basket.js">官网</a></li>
<li>bag.js：可以缓存脚本和加载资源，与 basket.js 相似，但增加了键值对接口和对 localStorage / websql / <a href="https://github.com/nodeca/bag.js">官网</a>undexedDB 的支持。</li>
<li>basil.js：智能的 JavaScript 数据持久层库。<a href="https://github.com/Wisembly/basil.js">官网</a></li>
<li>jquery-cookie：轻量简单的、用于读取、编辑和删除 cookie 的 jQuery 插件。<a href="https://github.com/carhartl/jquery-cookie">官网</a></li>
<li>Cookies：客户端 Cookie 操作库。<a href="https://github.com/ScottHamper/Cookies">官网</a></li>
<li>DB.js：基于 Promise 的、封装了 IndexedDB 的库。<a href="https://github.com/aaronpowell/db.js/">官网</a></li>
<li>lawnchair.js：简单的客户端 JSON 存储。<a href="https://github.com/brianleroux/lawnchair/">官网</a></li>
</ul>
<h3 id="user-content-color"><a id="user-content-颜色" class="anchor" href="#颜色" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>颜色</h3>
<ul>
<li>randomColor：JavaScript 颜色生成器。<a href="https://github.com/davidmerfield/randomColor">官网</a></li>
<li>chroma.js：拥有各种各样颜色操作的 JavaScript 库。<a href="https://github.com/gka/chroma.js">官网</a></li>
<li>color：JavaScript 颜色转换和操作库。<a href="https://github.com/MoOx/color">官网</a></li>
<li>colors：更智能的默认 web 颜色。<a href="https://github.com/mrmrs/colors">官网</a></li>
<li>PleaseJS：随机创建出赏心悦目的颜色和配色方案。<a href="https://github.com/Fooidge/PleaseJS">官网</a></li>
<li>TinyColor：快速、轻巧的颜色操作和转换库。<a href="https://github.com/bgrins/TinyColor">官网</a></li>
<li>Vibrant.js：从图像提取主要颜色。<a href="https://github.com/jariz/vibrant.js/">官网</a></li>
</ul>
<h3 id="user-content-i18n-and-l10n"><a id="user-content-国际化和本地化i18n-and-l10n" class="anchor" href="#国际化和本地化i18n-and-l10n" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>国际化和本地化（I18n And L10n）</h3>
<p>本地化和国际化 JavaScript 库</p>
<ul>
<li>i18next：JavaScript 最简单的国际化（i18n）方法。<a href="https://github.com/i18next/i18next">官网</a></li>
<li>polyglot：小巧的国际化助手库。<a href="https://github.com/airbnb/polyglot.js">官网</a></li>
<li>babelfish：i18n 提供友好易懂的 API ，并且内置多种支持。<a href="https://github.com/nodeca/babelfish/">官网</a></li>
</ul>
<h3 id="user-content-class"><a id="user-content-类" class="anchor" href="#类" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>类</h3>
<ul>
<li>ClassManager：世界上最快、最方便的类系统之一。<a href="https://github.com/kogarashisan/ClassManager">官网</a></li>
<li>klass：用于创建极富表现力的类工具库。<a href="https://github.com/ded/klass">官网</a></li>
<li>augment：世界上最小且最快的一流 JavaScript 继承模式。<a href="https://github.com/javascript/augment">官网</a></li>
</ul>
<h3 id="user-content-control-flow"><a id="user-content-控制流" class="anchor" href="#控制流" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>控制流</h3>
<ul>
<li>async：适用于 node 和浏览器的异步工具库。<a href="https://github.com/caolan/async">官网</a></li>
<li>q：实现异步的 promise JavaScript 库。<a href="https://github.com/kriskowal/q">官网</a></li>
<li>step：让逻辑顺序合理化的异步控制流库。<a href="https://github.com/creationix/step/">官网</a></li>
<li>contra：利用函数风格实现的异步流控制。<a href="https://github.com/bevacqua/contra/">官网</a></li>
<li>Bluebird：专注于革新功能和性能的，功能齐全的 promoise 库。<a href="https://github.com/petkaantonov/bluebird/">官网</a></li>
<li>when：快速可靠的、Promises/A+ 规范的 when() 实现，而且拥有异步其它的优秀特性。<a href="https://github.com/cujojs/when">官网</a></li>
<li>ObjectEventTarget：提供增加了事件监听的原型（与 DOMElement 的 EventTarget 在浏览器行为一致）。<a href="https://github.com/gartz/ObjectEventTarget">官网</a></li>
</ul>
<h3 id="user-content-routing"><a id="user-content-路由" class="anchor" href="#路由" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>路由</h3>
<ul>
<li>director：一个小巧的、与 URL 同构的路由器。<a href="https://github.com/flatiron/director">官网</a></li>
<li>page.js：受 Express router 启发的小型客户端路由器（约为1200字节）。<a href="https://github.com/visionmedia/page.js">官网</a></li>
<li>pathjs：简单、轻量的 web 路由器。<a href="https://github.com/mtrpcic/pathjs">官网</a></li>
<li>crossroads：JavaScript 路由。<a href="https://github.com/millermedeiros/crossroads.js">官网</a></li>
<li>davis.js：使用 pushState、RESTful 风格和可降级的 JavaScript 路由器。<a href="https://github.com/olivernn/davis.js">官网</a></li>
<li><a href="http://hao.jobbole.com/angular-ui-router/">angular-ui-router</a>：基于AngularJS的可嵌套路由。<a href="http://angular-ui.github.io/ui-router/">官网</a></li>
</ul>
<h3 id="user-content-security"><a id="user-content-安全性" class="anchor" href="#安全性" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>安全性</h3>
<ul>
<li>DOMPurify：针对 HTML、MathML 和 SVG 的仅支持DOM、快速、高容错的 XSS 过滤器。<a href="https://github.com/cure53/DOMPurify">官网</a></li>
<li>js-xss：通过白名单配置，即可过滤不信任的 HTML（防止 XSS 攻击）。<a href="https://github.com/leizongmin/js-xss">官网</a></li>
</ul>
<h3 id="user-content-log"><a id="user-content-日志" class="anchor" href="#日志" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>日志</h3>
<ul>
<li>log：带有样式的 Console.log。<a href="https://github.com/adamschwartz/log">官网</a></li>
<li>Conzole：对 JavaScript 原生 console 对象方法和功能进行封装的 debug 面板，使其显示在页面内。<a href="https://github.com/Oaxoa/Conzole">官网</a></li>
<li>console.log-wrapper：将日志清晰地记录到 console，且兼容所有浏览器。<a href="https://github.com/patik/console.log-wrapper">官网</a></li>
<li>loglevel：最轻量的 JavaScript 日志记录工具库，向封装后可用的 console.log 方法增加可靠的日志等级。<a href="https://github.com/pimterry/loglevel">官网</a></li>
<li>minilog：轻量的、用流式 API 显示的、可用于客户端和服务器端的日志记录库。<a href="http://mixu.net/minilog/">官网</a></li>
</ul>
<h3 id="user-content-regexp"><a id="user-content-正则表达式" class="anchor" href="#正则表达式" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>正则表达式</h3>
<ul>
<li>RegEx101：在线的 JavaScript 正则表达式测试器和调试器。同时支持 Python、PHP 和 PCRE。<a href="https://regex101.com/#javascript">官网</a></li>
<li>RegExr：用于创建、测试和学习正则表达式的 HTML/JS  工具。<a href="http://regexr.com/">官网</a></li>
<li>RegExpBuilder：使用链式方法创建正则表达式。<a href="https://github.com/thebinarysearchtree/regexpbuilderjs">官网</a></li>
</ul>
<h3 id="user-content-media"><a id="user-content-媒体" class="anchor" href="#媒体" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>媒体</h3>
<ul>
<li>Ion.Sound：可用于任何网页上简单音频。<a href="https://github.com/IonDen/ion.sound">官网</a></li>
</ul>
<h3 id="user-content-voice-command"><a id="user-content-语音命令" class="anchor" href="#语音命令" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>语音命令</h3>
<ul>
<li>annyang：向网站添加语音命令的语音识别库。<a href="https://github.com/TalAter/annyang">官网</a></li>
<li>voix.js：向网站、app 或游戏添加语音命令的 JavaScript 库。<a href="https://github.com/pazguille/voix">官网</a></li>
</ul>
<h3 id="user-content-api"><a id="user-content-api" class="anchor" href="#api" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>API</h3>
<ul>
<li>bottleneck：强大的频率限制器，使调节流量变得更容易。<a href="https://github.com/SGrondin/bottleneck">官网</a></li>
<li>oauth-signature-js：适用于 node 和 浏览器的 OAuth 1.0a 签名生成器。<a href="https://github.com/bettiolo/oauth-signature-js">官网</a></li>
<li>amygdala：为 Web 应用提供 RESTful HTTP 客户端解决方案。<a href="https://github.com/lincolnloop/amygdala">官网</a></li>
<li>jquery.rest：一个让 RESTful API 更易使用的 jQuery 插件。<a href="https://github.com/jpillora/jquery.rest">官网</a></li>
</ul>
<h3 id="user-content-vision-detection"><a id="user-content-视觉检测" class="anchor" href="#视觉检测" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>视觉检测</h3>
<ul>
<li>tracking.js：在 web 上实现计算视觉的一种现代方法。<a href="https://github.com/eduardolundgren/tracking.js">官网</a></li>
<li>ocrad.js：通过 Emscripten 用 JavaScript 实现 OCR（光学字符识别）。<a href="https://github.com/antimatter15/ocrad.js">官网</a></li>
</ul>
<h3 id="user-content-browser-detection"><a id="user-content-浏览器检测" class="anchor" href="#浏览器检测" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>浏览器检测</h3>
<ul>
<li>bowser：一个浏览器检测器。<a href="https://github.com/ded/bowser">官网</a></li>
</ul>
<h3 id="user-content-performance-analysis"><a id="user-content-性能分析" class="anchor" href="#性能分析" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>性能分析</h3>
<ul>
<li>easy-monitor：一个轻量级实时 Node.js 项目的内核性能分析工具。<a href="http://www.easy-monitor.cn/document">官网</a></li>
</ul>
<h2><a id="user-content-ui" class="anchor" href="#ui" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>UI</h2>
<h3 id="user-content-code-highlighting"><a id="user-content-代码高亮" class="anchor" href="#代码高亮" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>代码高亮</h3>
<ul>
<li>Highlight.js：JavaScript 语法高亮器。<a href="https://github.com/isagalaev/highlight.js">官网</a></li>
<li>PrismJS：轻量、健壮和优雅的语法高亮器。<a href="https://github.com/PrismJS/prism">官网</a></li>
</ul>
<h3 id="user-content-loading-status"><a id="user-content-加载状态" class="anchor" href="#加载状态" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>加载状态</h3>
<p>指示加载状态的库。</p>
<ul>
<li>Mprogress.js：创建谷歌 Material 设计风格的线性进度条。<a href="https://github.com/lightningtgc/MProgress.js">官网</a></li>
<li>NProgress：在 Ajax'y 应用显示细长型进度条<a href="http://ricostacruz.com/nprogress/">官网</a></li>
<li>Spin.js：一个旋转的进度指示器。<a href="https://github.com/fgnass/spin.js">官网</a></li>
<li>progress.js：为页面任何对象创建和管理进度条。<a href="https://github.com/usablica/progress.js">官网</a></li>
<li>progressbar.js：用 SVG path 动画制作的、漂亮和响应式的进度条。<a href="https://github.com/kimmobrunfeldt/progressbar.js">官网</a></li>
<li>pace：自动向你的网站添加一个进度条。<a href="https://github.com/HubSpot/pace">官网</a></li>
<li>topbar：小巧漂亮的、与网站同宽的进度指示器。<a href="https://github.com/buunguyen/topbar">官网</a></li>
<li>nanobar：非常轻量的进度条。不依赖 jQuery。<a href="https://github.com/jacoborus/nanobar">官网</a></li>
<li>PageLoadingEffects：使用 SVG 动画展现新内容的现代方式。<a href="https://github.com/codrops/PageLoadingEffects">官网</a></li>
<li>SpinKit：运用 CSS 动画的加载指示器集合。<a href="https://github.com/tobiasahlin/SpinKit">官网</a></li>
<li>Ladda：内置在按钮的加载指示器。<a href="https://github.com/hakimel/Ladda">官网</a></li>
<li>css-loaders：运用 CSS 动画的旋转加载指示器的集合。<a href="https://github.com/lukehaas/css-loaders">官网</a></li>
</ul>
<p>除了上述这些库，还有收藏在 <a href="http://codepen.io/collection/HtAne/">Codepen</a> 的，另外还有 <a href="http://www.ajaxload.info/">Ajaxload</a>，<a href="http://preloaders.net/">Preloaders</a> 和 <a href="http://cssload.net/">CSSLoad</a> 这些生成器。</p>
<h3 id="user-content-validation"><a id="user-content-验证" class="anchor" href="#验证" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>验证</h3>
<ul>
<li>Parsley.js：不用写一行 JavaScript 代码即可在前端验证表单。<a href="https://github.com/guillaumepotier/Parsley.js">官网</a></li>
<li>jquery-validation：jQuery 验证插件。<a href="https://github.com/jzaefferer/jquery-validation">官网</a></li>
<li>validator.js：字符串验证和过滤（在使用用户输入之前清理用户输入中的有害或危险字符的操作）。<a href="https://github.com/chriso/validator.js">官网</a></li>
<li>validate.js：受 CodeIgniter 启发的轻量表单验证 JavaScript 库。<a href="https://github.com/rickharrison/validate.js">官网</a></li>
<li>validatr：跨浏览器的 HTML5 表单验证库。<a href="https://github.com/jaymorrow/validatr/">官网</a></li>
<li>BootstrapValidator：是验证表单域中最好的 jQuery 插件。要与 Bootstrap 3 一起使用。<a href="https://github.com/nghuuphuoc/bootstrapvalidator">官网</a></li>
<li><a href="http://hao.jobbole.com/is-js/">is.js</a>：检查类型、正则表达式、是否存在、时间等。<a href="https://github.com/arasatasaygin/is.js">官网</a></li>
<li>FieldVal：多用途验证库。同时支持同步和异步验证。<a href="https://github.com/FieldVal/fieldval-js">官网</a></li>
</ul>
<h3 id="user-content-keyboard-wrappers"><a id="user-content-键盘封装器" class="anchor" href="#键盘封装器" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>键盘封装器</h3>
<ul>
<li>mousetrap：处理键盘快捷键的 JavaScript 库。<a href="https://github.com/ccampbell/mousetrap">官网</a></li>
<li>keymaster：定义和调度键盘快捷键的小型库。<a href="https://github.com/madrobby/keymaster">官网</a></li>
<li>Keypress：键入捕捉工具库，任何键都可以成为一个修饰健。<a href="https://github.com/dmauro/Keypress">官网</a></li>
<li>KeyboardJS：一个用于绑定键盘组合的 JavaScript 库，让你脱离快捷键和快捷键组合冲突的痛苦。<a href="https://github.com/RobertWHurst/KeyboardJS">官网</a></li>
<li>jquery.hotkeys：jQuery Hotkeys 能让你在代码任何的地方监听键盘事件，并几乎支持所有按键组合。<a href="https://github.com/jeresig/jquery.hotkeys">官网</a></li>
<li>jwerty：令人惊叹的键盘事件处理库。<a href="https://github.com/keithamus/jwerty">官网</a></li>
</ul>
<h3 id="user-content-tours-and-guides"><a id="user-content-浏览和引导" class="anchor" href="#浏览和引导" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>浏览和引导</h3>
<ul>
<li>intro.js：这是一个介绍新功能的很好方式，能一步步地引导用户浏览你的网站和项目。<a href="https://github.com/usablica/intro.js">官网</a></li>
<li>shepherd：通过引导让用户浏览你的应用程序。<a href="https://github.com/HubSpot/shepherd">官网</a></li>
<li>bootstrap-tour：应用 Twitter Bootstrap 弹出框对产品进行快速简单的引导。<a href="https://github.com/sorich87/bootstrap-tour">官网</a></li>
<li>tourist：简单、灵活的应用引导介绍库。<a href="https://github.com/easelinc/tourist">官网</a></li>
<li>chardin.js：简单的应用遮罩层介绍。<a href="https://github.com/heelhook/chardin.js">官网</a></li>
<li>pageguide：使用 jQuery 和 CSS3 的 web 页面元素交互引导库。<a href="https://github.com/tracelytics/pageguide">官网</a></li>
<li>hopscotch：让开发者更容易向其页面产品添加引导的框架。<a href="https://github.com/linkedin/hopscotch">官网</a></li>
<li>joyride：基于 jQuery 的功能引导插件。<a href="https://github.com/zurb/joyride">官网</a></li>
<li>focusable：通过向页面其余部分添加遮罩层，使焦点聚集在特定 DOM 元素。<a href="https://github.com/zzarcon/focusable">官网</a></li>
</ul>
<h3 id="user-content-notifications"><a id="user-content-通知" class="anchor" href="#通知" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>通知</h3>
<ul>
<li>messenger：为你的应用添加 Growl-style 弹框和信息（Crowl 是 Mac OS X 下的一个通知系统）。<a href="https://github.com/HubSpot/messenger">官网</a></li>
<li>noty：jQuery 通知插件。<a href="https://github.com/needim/noty">官网</a></li>
<li>pnotify：适用于 Bootstrap、jQuery UI 和 Web Notifications Draft 的 JavaScript 通知库。<a href="https://github.com/sciactive/pnotify">官网</a></li>
<li>toastr：用来显示简单的，会自动到期的信息窗口）简单的弹出框通知（<a href="http://ux.stackexchange.com/questions/11998/what-is-a-toast-notification">toast notifications</a><a href="https://github.com/CodeSeven/toastr">官网</a></li>
<li>humane-js：一个简单、时髦的浏览器通知系统。<a href="https://github.com/wavded/humane-js">官网</a></li>
<li>smoke.js：与框架无关的、能够自定义样式的 JavaScript 弹框系统。<a href="https://github.com/hxgf/smoke.js">官网</a></li>
</ul>
<h3 id="user-content-sliders"><a id="user-content-幻灯片" class="anchor" href="#幻灯片" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>幻灯片</h3>
<ul>
<li>Swiper：使用硬件加速过渡的移动设备触控滑块框架。<a href="https://github.com/nolimits4web/Swiper">官网</a></li>
<li>slick：你所需要的最后一个轮播插件。<a href="https://github.com/kenwheeler/slick">官网</a></li>
<li>slidesJs：响应式的 jQuery（1.7.1+）幻灯片插件，具有触摸、 CSS3 过渡等特性。<a href="http://www.slidesjs.com/">官网</a></li>
<li>FlexSlider：一款令人惊叹的、全响应式的幻灯片 jQuery 插件。<a href="https://github.com/woothemes/FlexSlider">官网</a></li>
<li>unslider：最简单的幻灯片 jQuery 插件。<a href="https://github.com/idiot/unslider">官网</a></li>
<li>colorbox：轻量、可自定义的灯箱 jQuery 插件。<a href="https://github.com/jackmoore/colorbox">官网</a></li>
<li>fancyBox：提供了良好优雅的方式，为页面上的图片、html 内容和多媒体添加缩放功能的工具。<a href="https://github.com/fancyapps/fancyBox">官网</a></li>
<li>sly：基于项导航的、支持单向滚动的 JavaScript 库。<a href="https://github.com/darsain/sly">官网</a></li>
<li>vegas：向页面添加漂亮的全屏背景的 jQuery 插件，甚至允许幻灯片。<a href="https://github.com/jaysalvat/vegas">官网</a></li>
<li>Sequence：用于创建响应式的幻灯片、演示、旗帜广告和以步骤为基础的应用的 CSS 动画框架。<a href="https://github.com/IanLunn/Sequence">官网</a></li>
<li>baguetteBox.js：易于使用的、用纯 JavaScript 实现的遮罩层脚本。<a href="https://github.com/feimosi/baguetteBox.js">官网</a></li>
<li>reveal.js：用 HTML 创建漂亮演示控件的框架。<a href="https://github.com/hakimel/reveal.js">官网</a></li>
<li>PhotoSwipe：适用于移动设备和桌面电脑的、模块化和不无依赖框架的 JavaScript 画廊控件。<a href="https://github.com/dimsemenov/PhotoSwipe">官网</a></li>
<li>jcSlider：用 CSS 动画实现的响应式幻灯片 jQuery 插件。<a href="https://github.com/JoanClaret/jcSlider">官网</a></li>
<li>basic-jquery-slider：易于使用、指定主题和定制化。<a href="https://github.com/jcobb/basic-jquery-slider">官网</a></li>
<li>unslider： 这是最简单的幻灯片 jQuery 插件。<a href="https://github.com/idiot/unslider">官网</a></li>
<li>viewerjs：原生js实现的图片查看器。<a href="https://fengyuanchen.github.io/viewerjs/">官网</a></li>
<li>jQuery.adaptive-slider：带有自适应颜色标题和导航的幻灯片 jQuery 插件。<a href="https://github.com/creative-punch/jQuery.adaptive-slider/">官网</a></li>
<li>slidr：可添加一些幻灯片效果。<a href="https://github.com/bchanx/slidr">官网</a></li>
<li>Flickity：可触摸的、响应式的和可轻弹的画廊。<a href="https://github.com/metafizzy/flickity">官网</a></li>
</ul>
<h3 id="user-content-range-sliders"><a id="user-content-滑块控件" class="anchor" href="#滑块控件" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>滑块控件</h3>
<ul>
<li>Ion.RangeSlider：强大的、易于自定义的范围滑块选择库，支持很多配置和皮肤。<a href="https://github.com/IonDen/ion.rangeSlider">官网</a></li>
<li>jQRangeSlider：支持日期的滑块选择库。<a href="https://github.com/ghusse/jQRangeSlider">官网</a></li>
<li>noUiSlider：轻量无冗余的、高度定制化的滑块选择库。<a href="https://github.com/leongersen/noUiSlider">官网</a></li>
<li>rangeslider.js：HTML5  input 区域滑块元素。<a href="https://github.com/andreruffert/rangeslider.js">官网</a></li>
</ul>
<h3 id="user-content-form-widgets"><a id="user-content-表单组件" class="anchor" href="#表单组件" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>表单组件</h3>
<h3><a id="user-content-输入" class="anchor" href="#输入" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>输入</h3>
<ul>
<li>typeahead.js：快速的、功能齐全的自动补全库。<a href="https://github.com/twitter/typeahead.js">官网</a></li>
<li>tag-it：处理多标签字段以及标签建议/自动完成的 jQuery UI 插件。<a href="https://github.com/aehlke/tag-it">官网</a></li>
<li>At.js：向你的应用添加类似 Github 的自动完成提示功能。<a href="https://github.com/ichord/At.js">官网</a></li>
<li>Placeholders.js：JavaScript 补全 HTML5 占位符的属性。<a href="https://github.com/jamesallardice/Placeholders.js">官网</a></li>
<li>fancyInput：利用 CSS3 效果让输入更有趣。<a href="https://github.com/yairEO/fancyInput">官网</a></li>
<li>jQuery-Tags-Input：利用这个 jQuery 插件，可奇妙地将一个简单的文本输入转换成一个酷酷的标签列表。<a href="https://github.com/xoxco/jQuery-Tags-Input">官网</a></li>
<li>vanilla-masker：一个纯 JavaScript 实现的输入控制库。<a href="https://github.com/BankFacil/vanilla-masker">官网</a></li>
<li>Ion.CheckRadio：一个为复选框和单选按钮添加样式的 jQuery 库，支持多种皮肤。<a href="https://github.com/IonDen/ion.checkRadio">官网</a></li>
</ul>
<h3><a id="user-content-日历" class="anchor" href="#日历" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>日历</h3>
<ul>
<li>pickadate.js：对移动设备友好的、响应式的和轻量的 jQuery 日期 &amp; 时间输入选择器。<a href="https://github.com/amsul/pickadate.js">官网</a></li>
<li>bootstrap-datepicker：基于 bootstrap 的日历选择器。<a href="https://github.com/eternicode/bootstrap-datepicker">官网</a></li>
<li>Pikaday：一个崭新的 JavaScript 日期选择器 —— 轻量、无依赖和模块化的 CSS。<a href="https://github.com/dbushell/Pikaday">官网</a></li>
<li>fullcalendar：全尺寸、支持拖放事件的日历（jQuery 插件）。<a href="https://github.com/fullcalendar/fullcalendar">官网</a></li>
<li>rome：可定制的日期（和时间）选择器。无依赖，可选 UI。<a href="https://github.com/bevacqua/rome">官网</a></li>
<li>datedropper： datedropper 是一个 jQuery 插件，它提供了快速简易的方式去管理日期输入框。<a href="https://github.com/felicegattuso/datedropper">官网</a></li>
<li>flatpickr： flatpickr 是一个轻量、强大、无依赖的日历和时间选择器插件，支持移动端，并支持React、Ember、Angular和Vue。<a href="https://chmln.github.io/flatpickr/">官网</a></li>
</ul>
<h3><a id="user-content-选择" class="anchor" href="#选择" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>选择</h3>
<ul>
<li>selectize.js：Selectize 是文本框和选择框的混合体。它基于jQuery，拥有自动完成和键盘感应下拉列表功能，可用于标签、联系人列表等。<a href="https://github.com/brianreavis/selectize.js">官网</a></li>
<li>select2：它基于 jQuery，是选择框（select box）的替代品。支持搜索、远程数据集和无限滚动。<a href="https://github.com/select2/select2">官网</a></li>
<li>chosen：可以让冗长不便的选择框更友好的库。<a href="https://github.com/harvesthq/chosen">官网</a></li>
</ul>
<h3><a id="user-content-文件上传" class="anchor" href="#文件上传" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>文件上传</h3>
<ul>
<li>jQuery-File-Upload：File Upload 是一个支持多文件选择、文件拖放、进度条、验证和图片、音频、视频预览的 <a href="https://github.com/blueimp/jQuery-File-Upload">官网</a>jQuery 插件。</li>
<li>dropzone：Dropzone 是一个易于使用且支持多文件拖放的库。其支持图片预览并且拥有很好的进度条效果。<a href="https://github.com/enyo/dropzone">官网</a></li>
<li>flow.js：一个通过 HTML5 的 File API ，提供多个同时链接的、稳定的、容错的、可恢复的/可重新开始的文件上传库。<a href="https://github.com/flowjs/flow.js">官网</a></li>
<li>fine-uploader：一个带有进度条、拖放功能和支持直接上传到 S3 （Amazon Simple Storage Service，亚马逊简易存储服务）的多文件上传插件。<a href="https://github.com/FineUploader/fine-uploader">官网</a></li>
<li>FileAPI：JavaScript 文件工具集合。支持多文件上传、拖放和文件分块上传。对于图像，支持裁剪、调整大小和根据 <a href="http://baike.baidu.com/view/22006.htm">EXIF</a> 自动调整方向。<a href="https://github.com/mailru/FileAPI">官网</a></li>
<li>plupload：处理文件上传的 JavaScript <a href="https://github.com/moxiecode/plupload">官网</a>API，其支持多文件选择、文件类型过滤、分块请求、客户端图片缩放和根据不同的运行环境选择 HTML5、Silverlight 和 Flash。</li>
</ul>
<h3><a id="user-content-其它" class="anchor" href="#其它" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>其它</h3>
<ul>
<li>form：jQuery 表单插件。<a href="https://github.com/malsup/form">官网</a></li>
<li>Garlic.js：自动在本地保存表单文本和选择框的值，直到表单被提交。<a href="https://github.com/guillaumepotier/Garlic.js">官网</a></li>
<li>Countable：对某个 HTML 元素包含文本的段落数、单词数和字符数进行统计的 JavaScript 函数。<a href="https://github.com/RadLikeWhoa/Countable">官网</a></li>
<li>card：只需一行代码，让信用卡表单变得更友好。<a href="https://github.com/jessepollak/card">官网</a></li>
<li>stretchy：自适应大小的 form 元素，表单本应该是这样的。<a href="https://github.com/LeaVerou/stretchy">官网</a></li>
<li>list.js：向表格、列表等 HTML 元素添加搜索、排序、过滤和自适应功能的库。在已有 HTML 上增加可视化。<a href="http://www.listjs.com/">
</a><a href="https://github.com/javve/list.js">官网</a></li>
</ul>
<h3 id="user-content-tips"><a id="user-content-提示" class="anchor" href="#提示" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>提示</h3>
<ul>
<li>tipsy：基于 jQuery 的 Fackbook 风格的提示工具（tooltip）。<a href="https://github.com/jaz303/tipsy">官网</a></li>
<li>opentip：开源且基于 prototype 框架的 JavaScript 工具提示库。<a href="https://github.com/enyo/opentip">官网</a></li>
<li>qTip2：非常强大的工具提示库。<a href="https://github.com/qTip2/qTip2">官网</a></li>
<li>tooltipster：一个工具提示 jQuery 插件。<a href="https://github.com/iamceege/tooltipster">官网</a></li>
<li>simptip：用 Sass 制作的、简单的工具提示。<a href="https://github.com/arashmanteghi/simptip">官网</a></li>
<li>jquery-popup-overlay：是一个响应式的和可访问性强的模态框（modal）和工具提示框 jQuery 插件。<a href="https://github.com/vast-engineering/jquery-popup-overlay">官网</a></li>
</ul>
<h3 id="user-content-modals-and-popups"><a id="user-content-模态框和弹出框" class="anchor" href="#模态框和弹出框" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>模态框和弹出框</h3>
<ul>
<li>Magnific-Popup：专注于性能、轻量、响应式的灯箱（lightbox）脚本。<a href="https://github.com/dimsemenov/Magnific-Popup">官网</a></li>
<li>jquery-popbox：jQuery 提示框插件。<a href="https://github.com/gristmill/jquery-popbox">官网</a></li>
<li>jquery.avgrund.js：一种新的定于弹出的模态框 jQuery 插件。<a href="https://github.com/voronianski/jquery.avgrund.js">官网</a></li>
<li>vex：新的、拥有高度可配置和易于改变样式功能的对话框库。<a href="https://github.com/HubSpot/vex">官网</a></li>
<li>bootstrap-modal：对 Bootstrap 默认的模态框类进行扩展。其支持响应式、可堆叠和 ajax 等。<a href="https://github.com/jschr/bootstrap-modal">官网</a></li>
<li>css-modal：纯 CSS 打造的模态框。<a href="https://github.com/drublic/css-modal">官网</a></li>
<li>jquery-popup-overlay：是一个响应式的和可访问性强的模态框和工具提示框（tooltips）jQuery 插件。<a href="https://github.com/vast-engineering/jquery-popup-overlay">官网</a></li>
<li>layer：国内最多人使用的web弹层组件。<a href="https://github.com/sentsin/layer/">官网</a></li>
</ul>
<h3 id="user-content-scroll"><a id="user-content-滚动" class="anchor" href="#滚动" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>滚动</h3>
<ul>
<li>scrollMonitor：滚动发生时，可以监听元素的、简单、快速的 API。<a href="https://github.com/sakabako/scrollMonitor">官网</a></li>
<li>headroom：除非你需要显示页面头部（header），否则将隐藏它，以腾出页面头部空间。<a href="https://github.com/WickyNilliams/headroom.js">官网</a></li>
<li>onepage-scroll：创建一个类似 Apple 的单页面滚动网站（iPhone 5S  网站）。<a href="https://github.com/peachananr/onepage-scroll">官网</a></li>
<li>iscroll：高性能、轻量、无依赖、兼容多平台的 JavaScript 滚动组件。<a href="https://github.com/cubiq/iscroll">官网</a></li>
<li>skrollr：独立（不依赖 jQuery） 的视差滚动库，适用于移动设备（Android + iOS）和桌面电脑。<a href="https://github.com/Prinzhorn/skrollr">官网</a></li>
<li>parallax：面向智能设备的视差引擎。<a href="https://github.com/wagerfield/parallax">官网</a></li>
<li>stellar.js：让视差滚动变简单。<a href="https://github.com/markdalgleish/stellar.js">官网</a></li>
<li>plax：基于 jQuery 的视差库。<a href="https://github.com/cameronmcefee/plax">官网</a></li>
<li>jparallax：创建可交互视差效果的 jQuery 插件。<a href="https://github.com/stephband/jparallax">官网</a></li>
<li>fullPage：简单和易于使用的、用于创建全屏滚动网站的插件（也被称为单页面网站）。<a href="https://github.com/alvarotrigo/fullPage.js">官网</a></li>
<li>ScrollMenu：让老旧无聊的滚动条焕然一新。<a href="https://github.com/s-yadav/ScrollMenu">官网</a></li>
</ul>
<h3 id="user-content-menu"><a id="user-content-菜单" class="anchor" href="#菜单" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>菜单</h3>
<ul>
<li>jQuery-menu-aim：当用户光标放在特定下拉菜单项时触发事件。可制作响应式的、大数据量的下拉菜单，如 Amazon 的。<a href="https://github.com/kamens/jQuery-menu-aim">官网</a></li>
<li>jQuery contextMenu：右键菜单（contextMenu） 管理工具。<a href="https://github.com/swisnl/jQuery-contextMenu">官网</a></li>
<li>Slideout：为移动设备的 web 应用制作出响应式的、可触摸滑出的导航菜单。<a href="https://github.com/mango/slideout">官网</a></li>
<li>Slide and swipe：一个基于 touchSwipe 库的滑出菜单插件。<a href="https://github.com/JoanClaret/slide-and-swipe-menu">官网</a></li>
</ul>
<h3 id="user-content-table-grid"><a id="user-content-表格栅格" class="anchor" href="#表格栅格" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>表格/栅格</h3>
<ul>
<li>jTable：基于 CRUD 表创建 AJAX 的 jQuery 插件。<a href="https://github.com/hikalkan/jtable">官网</a></li>
<li>DataTables：这是一个非常灵活的工具，在渐进增强的基础上，将高级的交互效果加到 HTML 表格。（jQuery 插件）<a href="http://www.datatables.net/">官网</a> </li>
<li>floatThead：（jQuery 插件）锁定表格头部，只允许表格内容滚动。适用于任何表格，而且不需要额外的 html 或 css。<a href="https://github.com/mkoryak/floatThead">官网</a></li>
<li>Masonry：瀑布流式的网格布局库。<a href="http://masonry.desandro.com/">官网</a></li>
<li>Packery：使用装箱算法（bin-packing）的网格布局库。支持拖拽布局。<a href="http://packery.metafizzy.co/">官网</a></li>
<li>Isotope：可过滤和可排序的网格布局的库，它能实现 Masonry、Packery 等布局。<a href="http://isotope.metafizzy.co/">官网</a></li>
</ul>
<h3 id="user-content-frameworks-1"><a id="user-content-框架-1" class="anchor" href="#框架-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>框架</h3>
<ul>
<li>Semantic UI：拥有大量主题和元素的 UI 套件。<a href="http://semantic-ui.com/">官网</a></li>
</ul>
<h3 id="user-content-gesture"><a id="user-content-手势" class="anchor" href="#手势" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>手势</h3>
<ul>
<li>hammer.js：拥有多种触摸手势的 JavaScript 库。<a href="https://github.com/hammerjs/hammer.js">官网</a></li>
<li>touchemulator：在桌面电脑模仿触摸输入。<a href="https://github.com/hammerjs/touchemulator">官网</a></li>
<li>Dragula：超级易于使用的拖拽库。<a href="https://github.com/bevacqua/dragula/">官网</a></li>
</ul>
<h3 id="user-content-touch"><a id="user-content-触摸" class="anchor" href="#触摸" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>触摸</h3>
<ul>
<li>fastclick.js：去除触屏用户300ms点击延误。<a href="https://github.com/ftlabs/fastclick">官网</a></li>
<li>dropload.js：移动端下拉刷新，上拉加载更多。<a href="https://github.com/ximan/dropload">官网</a></li>
<li>touchslide.js：触屏滑动特效。<a href="http://www.superslide2.com/touchSlide/">官网</a></li>
</ul>
<h3 id="user-content-maps"><a id="user-content-地图" class="anchor" href="#地图" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>地图</h3>
<ul>
<li>Leaflet：对移动设备友好的、可交互的地图 JavaScript 库。<a href="https://github.com/Leaflet/Leaflet">官网</a></li>
<li>Cesium：开源的、基于 WebGL 实现的虚拟地球仪和地图引擎。<a href="https://github.com/AnalyticalGraphicsInc/cesium">官网</a></li>
<li>gmaps：以最简单的方式使用 Google 地图。<a href="https://github.com/HPNeo/gmaps">官网</a></li>
<li>polymaps：一个免费的、兼容现代 web 浏览器的、用于制作动态可交互的地图 JavaScript 库。<a href="https://github.com/simplegeo/polymaps">官网</a></li>
<li>kartograph.js：开源的 Kartograph SVG 地图渲染器。<a href="https://github.com/kartograph/kartograph.js">官网</a></li>
<li>mapbox.js：Mapbox 的 API，Leaflet 的插件。<a href="https://github.com/mapbox/mapbox.js">官网</a></li>
<li>jqvmap：矢量地图 jQuery 插件。<a href="https://github.com/manifestinteractive/jqvmap">官网</a></li>
<li>OpenLayers3：高性能的、功能丰富的库，能满足你对地图所有需求。<a href="http://openlayers.org/">官网</a></li>
</ul>
<h3 id="user-content-video-audio"><a id="user-content-视频音频" class="anchor" href="#视频音频" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>视频/音频</h3>
<ul>
<li>prettyembed.js：更完美地嵌入 YouTube —— 拥有很好的选项，如高分辨率的预览图、嵌入选项的高级定制和可选的 <a href="https://github.com/mike-zarandona/prettyembed.js">官网</a>FitVids 支持。</li>
<li><a href="http://hao.jobbole.com/html5media/">html5media</a>：能在所有主流浏览器播放多媒体标签中定义的多媒体文件。<a href="https://github.com/etianen/html5media">官网</a></li>
<li>Play-em JS：Play'em 是一个 JavaScript 组件，它能管理音乐/视频播放顺序，通过在一个 DIV 元素里嵌入几个播放器（Youtube、Soundcloud 和 Vimeo）来控制一系列歌曲的播放。<a href="https://github.com/adrienjoly/playemjs">官网</a></li>
<li>polyplayer：将 YouTube、Soundcloud 和 Vimeo 播放器的 API 统一成一套。<a href="https://github.com/Acconut/polyplayer">官网</a></li>
<li>flowplayer： HTML5 视频播放器 <a href="https://flowplayer.org/">官网</a>、<a href="https://github.com/flowplayer/flowplayer">Github</a></li>
<li>mediaelement：让 HTML5、 Flash 播放器和模仿 HTML5 媒介元素 API 的 Silverlight shim，在所有浏览器拥有一致的 UI。<a href="http://mediaelementjs.com/">官网</a>、<a href="https://github.com/johndyer/mediaelement">Github</a></li>
<li>SoundJS：让音频在 web 上运行更简单的库。它为不同浏览器提供了一致的 API。<a href="https://github.com/CreateJS/SoundJS">官网</a></li>
</ul>
<h3 id="user-content-animations"><a id="user-content-动画" class="anchor" href="#动画" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>动画</h3>
<ul>
<li><a href="http://hao.jobbole.com/velocity-js/">velocity</a>：加速 JavaScript 动画。<a href="https://github.com/julianshapiro/velocity">官网</a></li>
<li><a href="http://hao.jobbole.com/jquery-transit/">jquery.transit</a>：拥有超级流畅的 CSS3 变换和过渡的 jQuery 插件。<a href="https://github.com/rstacruz/jquery.transit">官网</a></li>
<li>impess.js：在 HTML 文档里，运用 CSS3 变换和过渡制作类似 Prezi 的展现效果。<a href="https://github.com/impress/impress.js">官网</a></li>
<li><a href="http://hao.jobbole.com/bounce-js/">bounce.js</a>：可以立刻创建有趣的 CSS3 动画。<a href="https://github.com/tictail/bounce.js">官网</a></li>
<li>GreenSock-JS：适用于所有主流浏览器的高性能 HTML5 动画。<a href="https://github.com/greensock/GreenSock-JS">官网</a></li>
<li>TransitionEnd：TransitionEnd 是一个运用 transitonend 事件的、跨浏览器的库。<a href="https://github.com/EvandroLG/transitionEnd">官网</a></li>
<li><a href="http://hao.jobbole.com/dynamics-js/">Dynamics.js</a>：用于创建基于物理知识的 CSS 动画库。<a href="https://github.com/michaelvillar/dynamics.js">官网</a></li>
</ul>
<h3 id="user-content-image-processing"><a id="user-content-图片处理" class="anchor" href="#图片处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>图片处理</h3>
<ul>
<li><a href="http://hao.jobbole.com/lena-js/">lena.js</a>：拥有滤镜和实用功能的图像处理库。<a href="https://github.com/davidsonfellipe/lena.js">官网</a></li>
<li><a href="http://hao.jobbole.com/pica/">pica</a>：高质量地调整图片大小（拥有快速的、纯 JS 实现的 Lanczos 滤镜算法）。<a href="https://github.com/nodeca/pica">官网</a></li>
<li>cropper：一个简单的图像裁剪 jQuery 插件。<a href="https://github.com/fengyuanchen/cropper">官网</a></li>
<li>AlloyImage：腾讯前端开源的基于HTML5的专业级图像处理开源引擎。<a href="https://github.com/AlloyTeam/AlloyImage">官网</a></li>
</ul>
<h3 id="user-content-es6"><a id="user-content-ecmascript-6" class="anchor" href="#ecmascript-6" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>ECMAScript 6</h3>
<ul>
<li><a href="http://hao.jobbole.com/ecmascript-6/">es6features</a>：ECMAScript 6 特性概述。<a href="https://github.com/lukehoban/es6features">官网</a></li>
<li>es6-features：ECMAScript 6:  特性概述和比较。<a href="https://github.com/rse/es6-features">官网</a></li>
<li>ECMAScript 6 compatibility table ：Compatibility tables 展示了各种平台上所有 ECMAScript 6 特性的支持程度。<a href="http://kangax.github.io/compat-table/es6/">官网</a></li>
<li>Babel (Formerly 6to5)：将 ES6+ 代码转换成纯 ES5。<a href="https://github.com/babel/babel">官网</a></li>
<li>Traceur compiler：ES6 特性转 ES5。包括 classes、generators、promises、destructuring <a href="https://github.com/google/traceur-compiler">官网</a>patterns、default parameters 等。</li>
</ul>
<h3 id="user-content-sdk"><a id="user-content-软件开发工具包sdk" class="anchor" href="#软件开发工具包sdk" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>软件开发工具包(SDK)</h3>
<ul>
<li>javascript-sdk-design：从工作和个人经验中提炼出来的 JavaScript SDK 设计指导。<a href="https://github.com/huei90/javascript-sdk-design">官网</a></li>
</ul>
<h3 id="user-content-misc"><a id="user-content-大杂烩" class="anchor" href="#大杂烩" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>大杂烩</h3>
<ul>
<li>echo：利用 data-* 属性延迟加载图片。<a href="https://github.com/toddmotto/echo">官网</a></li>
<li>picturefill：响应式图片显示插件，使浏览器支持 srcset、size 属性。<a href="https://github.com/scottjehl/picturefill">官网</a></li>
<li>platform.js：一个平台检测库，几乎适用于所有 JavaScript 平台。<a href="https://github.com/bestiejs/platform.js">官网</a></li>
<li><a href="http://hao.jobbole.com/json3/">json3</a>：一个现代 JSON 实现库，几乎兼容所有 JavaScript 平台。<a href="https://github.com/bestiejs/json3">官网</a></li>
<li>Logical Or Not：一个关于 JavaScript 特性的游戏。<a href="http://gabinaureche.com/logicalornot/">官网</a></li>
<li>BitSet.js：实现位向量的 JavaScript 库。<a href="https://github.com/infusion/BitSet.js">官网</a></li>
<li><a href="http://hao.jobbole.com/edge-js/">Edge.js</a>：运行在一个进程中运行.NET和Node.js代码。<a href="http://tjanczuk.github.io/edge/">官网</a>、<a href="https://github.com/tjanczuk/edge">GitHub</a></li>
</ul>

## 四、机器学习

<hr>
<h2><a id="user-content-c" class="anchor" href="#c" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#c"></a>C++</h2>
<h4><a id="user-content-计算机视觉" class="anchor" href="#计算机视觉" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#compute-vision"></a>计算机视觉</h4>
<ul>
<li><a href="http://hao.jobbole.com/ccv/">CCV</a>：基于C语言/提供缓存/核心的机器视觉库，新颖的机器视觉库。<a href="https://github.com/liuliu/ccv">官网</a></li>
<li><a href="http://hao.jobbole.com/opencv/">OpenCV</a>：它提供C++、C、Python、Java 以及 MATLAB接口。并支持Windows、Linux、Android 和 Mac OS操作系统。<a href="http://opencv.org/">官网</a></li>
</ul>
<h4><a id="user-content-通用机器学习" class="anchor" href="#通用机器学习" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning"></a>通用机器学习</h4>
<ul>
<li>MLPack：<a href="http://www.mlpack.org/">官网</a>。</li>
<li>DLib：<a href="http://dlib.net/ml.html">官网</a>。</li>
<li>ecogg：<a href="https://code.google.com/p/encog-cpp/">官网</a>。</li>
<li>shark：<a href="http://image.diku.dk/shark/sphinx_pages/build/html/index.html">官网</a>。</li>
</ul>
<h2><a id="user-content-closure" class="anchor" href="#closure" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#closure"></a>Closure</h2>
<h4><a id="user-content-通用机器学习-1" class="anchor" href="#通用机器学习-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>通用机器学习</h4>
<ul>
<li>Closure Toolbox：Clojure语言库与工具的分类目录。<a href="http://www.clojure-toolbox.com/">官网</a></li>
</ul>
<h2><a id="user-content-go" class="anchor" href="#go" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#go"></a>Go</h2>
<h4><a id="user-content-自然语言处理" class="anchor" href="#自然语言处理" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#natural-language-processing"></a>自然语言处理</h4>
<ul>
<li>go-porterstemmer：一个Porter词干提取算法的原生Go语言净室实现。<a href="https://github.com/reiver/go-porterstemmer">官网</a></li>
<li>paicehusk：Paice/Husk词干提取算法的Go语言实现。<a href="https://github.com/Rookii/paicehusk">官网</a></li>
<li>snowball：Go语言版的Snowball词干提取器。<a href="https://bitbucket.org/tebeka/snowball">官网</a></li>
</ul>
<h4><a id="user-content-通用机器学习-2" class="anchor" href="#通用机器学习-2" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning-2"></a>通用机器学习</h4>
<ul>
<li>Go Learn：Go语言机器学习库。<a href="https://github.com/sjwhitworth/golearn">官网</a></li>
<li>go-pr：Go语言机器学习包。<a href="https://github.com/daviddengcn/go-pr">官网</a></li>
<li>bayesian：Go语言朴素贝叶斯分类库。<a href="https://github.com/jbrukh/bayesian">官网</a></li>
<li>go-galib：Go语言遗传算法库。<a href="https://github.com/thoj/go-galib">官网</a></li>
</ul>
<h4><a id="user-content-数据分析数据可视化" class="anchor" href="#数据分析数据可视化" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#data-analysis--data-visualization"></a>数据分析/数据可视化</h4>
<ul>
<li>go-graph：Go语言图形库。<a href="https://github.com/StepLg/go-graph">官网</a></li>
<li>SVGo：Go语言的SVG生成库。<a href="http://www.svgopen.org/2011/papers/34-SVGo_a_Go_Library_for_SVG_generation/">官网</a></li>
</ul>
<h2><a id="user-content-java" class="anchor" href="#java" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#java"></a>Java</h2>
<h4><a id="user-content-自然语言处理-1" class="anchor" href="#自然语言处理-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#natural-language-processing-1"></a>自然语言处理</h4>
<ul>
<li>CoreNLP：斯坦福大学的CoreNLP提供一系列的自然语言处理工具，输入原始英语文本，可以给出单词的基本形式（下面Stanford开头的几个工具都包含其中)。<a href="http://nlp.stanford.edu/software/corenlp.shtml">官网</a></li>
<li>Stanford Parser：一个自然语言解析器。<a href="http://nlp.stanford.edu/software/lex-parser.shtml">官网</a></li>
<li>Stanford POS Tagger：一个词性分类器。<a href="http://nlp.stanford.edu/software/tagger.shtml">官网</a></li>
<li>Stanford Name Entity Recognizer：Java实现的名称识别器。<a href="http://nlp.stanford.edu/software/CRF-NER.shtml">官网</a></li>
<li>Stanford Word Segmenter：分词器，很多NLP工作中都要用到的标准预处理步骤。<a href="http://nlp.stanford.edu/software/segmenter.shtml">官网</a>。</li>
<li>Tregex、Tsurgeon与Semgrex：用来在树状数据结构中进行模式匹配，基于树关系以及节点匹配的正则表达式（名字是“tree regular expressions"的缩写）<a href="http://nlp.stanford.edu/software/tregex.shtml">官网</a></li>
<li>Stanford Phrasal：最新的基于统计短语的机器翻译系统，java编写。<a href="http://nlp.stanford.edu/software/phrasal/">官网</a></li>
<li>Stanford Tokens Regex：用以定义文本模式的框架。<a href="http://nlp.stanford.edu/software/tokensregex.shtml">官网</a></li>
<li>Stanford Temporal Tagger：SUTime是一个识别并标准化时间表达式的库。<a href="http://nlp.stanford.edu/software/sutime.shtml">官网</a></li>
<li>Stanford SPIED：在种子集上使用模式，以迭代方式从无标签文本中学习字符实体。<a href="http://nlp.stanford.edu/software/patternslearning.shtml">官网</a>。</li>
<li>Stanford Topic Modeling Toolbox：为社会科学家及其他希望分析数据集的人员提供的主题建模工具。<a href="http://nlp.stanford.edu/software/tmt/tmt-0.4/">官网</a></li>
<li>Twitter Text Java：Java实现的推特文本处理库。<a href="https://github.com/twitter/twitter-text-java">官网</a></li>
<li>MALLET：基于Java的统计自然语言处理、文档分类、聚类、主题建模、信息提取以及其他机器学习文本应用包。<a href="http://mallet.cs.umass.edu/">官网</a></li>
<li>OpenNLP：处理自然语言文本的机器学习工具包。<a href="http://hao.jobbole.com/apache-opennlp/">官网</a></li>
<li>LingPipe：使用计算机语言学处理文本的工具包。<a href="http://alias-i.com/lingpipe/index.html">官网</a></li>
</ul>
<h4><a id="user-content-通用机器学习-3" class="anchor" href="#通用机器学习-3" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning-3"></a>通用机器学习</h4>
<ul>
<li>MLlib in Apache Spark：Spark中的分布式机器学习程序库。<a href="http://spark.apache.org/docs/latest/mllib-guide.html">官网</a></li>
<li>Mahout：分布式的机器学习库。<a href="https://github.com/apache/mahout">官网</a></li>
<li>Stanford Classifier：斯坦福大学的分类器。<a href="http://nlp.stanford.edu/software/classifier.shtml">官网</a></li>
<li>Weka：Weka是数据挖掘方面的机器学习算法集。<a href="http://www.cs.waikato.ac.nz/ml/weka/">官网</a></li>
<li>ORYX：提供一个简单的大规模实时机器学习/预测分析基础架构。<a href="https://github.com/cloudera/oryx">官网</a></li>
</ul>
<h4><a id="user-content-数据分析数据可视化-1" class="anchor" href="#数据分析数据可视化-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#data-analysis--data-visualization-1"></a>数据分析/数据可视化</h4>
<ul>
<li>Hadoop：大数据分析平台。<a href="https://github.com/apache/hadoop-mapreduce">官网</a></li>
<li>Spark：快速通用的大规模数据处理引擎。<a href="https://github.com/apache/spark">官网</a></li>
<li>Impala：为Hadoop实现实时查询。<a href="https://github.com/cloudera/impala">官网</a></li>
</ul>
<h2><a id="user-content-javascript" class="anchor" href="#javascript" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#javascript"></a>Javascript</h2>
<h4><a id="user-content-自然语言处理-2" class="anchor" href="#自然语言处理-2" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#natural-language-processing-2"></a>自然语言处理</h4>
<ul>
<li>Twitter-text-js：JavaScript实现的推特文本处理库。<a href="https://github.com/twitter/twitter-text-js">官网</a></li>
<li>NLP.js：javascript及coffeescript编写的NLP工具。<a href="https://github.com/nicktesla/nlpjs">官网</a></li>
<li>natural：Node下的通用NLP工具。<a href="https://github.com/NaturalNode/natural">官网</a></li>
<li>Knwl.js：JS编写的自然语言处理器。<a href="https://github.com/loadfive/Knwl.js">官网</a></li>
</ul>
<h4><a id="user-content-数据分析数据可视化-2" class="anchor" href="#数据分析数据可视化-2" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#data-analysis--data-visualization-2"></a>数据分析/数据可视化</h4>
<ul>
<li>D3.js：<a href="http://d3js.org/">官网</a>。</li>
<li>High Charts：<a href="http://www.highcharts.com/">官网</a>。</li>
<li>NVD3.js：<a href="http://nvd3.org/">官网</a>。</li>
<li>dc.js：<a href="http://dc-js.github.io/dc.js/">官网</a>。</li>
<li>chartjs：<a href="http://www.chartjs.org/">官网</a>。</li>
<li>dimple：<a href="http://dimplejs.org/">官网</a>。</li>
<li>amCharts：<a href="http://www.amcharts.com/">官网</a>。</li>
</ul>
<h4><a id="user-content-通用机器学习-4" class="anchor" href="#通用机器学习-4" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning-4"></a>通用机器学习</h4>
<ul>
<li>Convnet.js：训练深度学习模型的JavaScript库。<a href="http://cs.stanford.edu/people/karpathy/convnetjs/">官网</a></li>
<li>Clustering.js：用JavaScript实现的聚类算法，供Node.js及浏览器使用。<a href="https://github.com/tixz/clustering.js">官网</a></li>
<li>Decision Trees：Node.js实现的决策树，使用ID3算法。<a href="https://github.com/serendipious/nodejs-decision-tree-id3">官网</a></li>
<li>Node-fann：Node.js下的快速人工神经网络库。<a href="https://github.com/rlidwka/node-fann">官网</a></li>
<li>Kmeans.js：k-means算法的简单Javascript实现，供Node.js及浏览器使用。<a href="https://github.com/tixz/kmeans.js">官网</a></li>
<li>LDA.js：供Node.js用的LDA主题建模工具。<a href="https://github.com/primaryobjects/lda">官网</a></li>
<li>Learning.js：逻辑回归/c4.5决策树的JavaScript实现。<a href="https://github.com/yandongliu/learningjs">官网</a></li>
<li>Machine Learning：Node.js的机器学习库。<a href="http://joonku.com/project/machine_learning">官网</a></li>
<li>Node-SVM：Node.js的支持向量机。<a href="https://github.com/nicolaspanel/node-svm">官网</a></li>
<li>Brain：JavaScript实现的神经网络。<a href="https://github.com/harthur/brain">官网</a></li>
<li>Bayesian-Bandit：贝叶斯强盗算法的实现，供Node.js及浏览器使用。<a href="https://github.com/omphalos/bayesian-bandit.js">官网</a></li>
</ul>
<h2><a id="user-content-julia" class="anchor" href="#julia" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#julia"></a>Julia</h2>
<h4><a id="user-content-通用机器学习-5" class="anchor" href="#通用机器学习-5" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning-5"></a>通用机器学习</h4>
<ul>
<li>PGM：Julia实现的概率图模型框架。<a href="https://github.com/JuliaStats/PGM.jl">官网</a></li>
<li>DA：Julia实现的正则化判别分析包。<a href="https://github.com/trthatcher/DA.jl">官网</a></li>
<li>Regression：回归分析算法包（如线性回归和逻辑回归）。<a href="https://github.com/lindahua/Regression.jl">官网</a></li>
<li>Local Regression：局部回归，非常平滑！。<a href="https://github.com/dcjones/Loess.jl">官网</a></li>
<li>Naive Bayes：朴素贝叶斯的简单Julia实现。<a href="https://github.com/nutsiepully/NaiveBayes.jl">官网</a></li>
<li>Mixed Models：（统计）混合效应模型的Julia包。<a href="https://github.com/dmbates/MixedModels.jl">官网</a></li>
<li>Simple MCMC：Julia实现的基本mcmc采样器。<a href="https://github.com/fredo-dedup/SimpleMCMC.jl">官网</a>。</li>
<li>Distance：Julia实现的距离评估模块。<a href="https://github.com/JuliaStats/Distance.jl">官网</a></li>
<li>Decision Tree：决策树分类器及回归分析器。<a href="https://github.com/bensadeghi/DecisionTree.jl">官网</a></li>
<li>Neural：Julia实现的神经网络。<a href="https://github.com/compressed/neural.jl">官网</a></li>
<li>MCMC：Julia下的MCMC工具。<a href="https://github.com/doobwa/MCMC.jl">官网</a></li>
<li>GLM：Julia写的广义线性模型包。<a href="https://github.com/JuliaStats/GLM.jl">官网</a></li>
<li>Online Learning：<a href="https://github.com/lendle/OnlineLearning.jl">官网</a></li>
<li>GLMNet：GMLNet的Julia包装版，适合套索/弹性网模型。<a href="https://github.com/simonster/GLMNet.jl">官网</a></li>
<li>Clustering：k-means, dp-means等数据聚类的基本函数。<a href="https://github.com/JuliaStats/Clustering.jl">官网</a></li>
<li>SVM：Julia下的支持向量机。<a href="https://github.com/JuliaStats/SVM.jl">官网</a></li>
<li>Kernal Density：Julia下的核密度估计器。<a href="https://github.com/JuliaStats/KernelDensity.jl">官网</a></li>
<li>Dimensionality Reduction：降维算法。<a href="https://github.com/JuliaStats/DimensionalityReduction.jl">官网</a></li>
<li>NMF：Julia下的非负矩阵分解包。<a href="https://github.com/JuliaStats/NMF.jl">官网</a></li>
<li>ANN：Julia实现的神经网络。<a href="https://github.com/EricChiang/ANN.jl">官网</a></li>
</ul>
<h4><a id="user-content-自然语言处理-3" class="anchor" href="#自然语言处理-3" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#natural-language-processing-3"></a>自然语言处理</h4>
<ul>
<li>Topic Models：Julia下的主题建模。<a href="https://github.com/slycoder/TopicModels.jl">官网</a></li>
<li>Text Analysis：Julia下的文本分析包。<a href="https://github.com/johnmyleswhite/TextAnalysis.jl">官网</a></li>
</ul>
<h4><a id="user-content-数据分析数据可视化-3" class="anchor" href="#数据分析数据可视化-3" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#data-analysis--data-visualization-3"></a>数据分析/数据可视化</h4>
<ul>
<li>Graph Layout：纯Julia实现的图布局算法。<a href="https://github.com/IainNZ/GraphLayout.jl">官网</a></li>
<li>Data Frames Meta：DataFrames的元编程工具。<a href="https://github.com/JuliaStats/DataFramesMeta.jl">官网</a></li>
<li>Julia Data：处理表格数据的Julia库。<a href="https://github.com/nfoti/JuliaData">官网</a></li>
<li>Data Read：从Stata、SAS、SPSS读取文件。<a href="https://github.com/WizardMac/DataRead.jl">官网</a></li>
<li>Hypothesis Tests：Julia中的假设检验包。<a href="https://github.com/JuliaStats/HypothesisTests.jl">官网</a></li>
<li>Gladfly：Julia编写的灵巧的统计绘图系统。<a href="https://github.com/dcjones/Gadfly.jl">官网</a></li>
<li>Stats：Julia编写的统计测试函数包。<a href="https://github.com/johnmyleswhite/stats.jl">官网</a></li>
<li>RDataSets：读取R语言中众多可用的数据集的Julia函数包。<a href="https://github.com/johnmyleswhite/RDatasets.jl">官网</a></li>
<li>DataFrames：处理表格数据的Julia库。<a href="https://github.com/JuliaStats/DataFrames.jl">官网</a></li>
<li>Distributions：概率分布及相关函数的Julia包。<a href="https://github.com/JuliaStats/Distributions.jl">官网</a></li>
<li>Data Arrays：元素值可以为空的数据结构。<a href="https://github.com/JuliaStats/DataArrays.jl">官网</a></li>
<li>Time Series：Julia的时间序列数据工具包。<a href="https://github.com/JuliaStats/TimeSeries.jl">官网</a></li>
<li>Sampling：Julia的基本采样算法包。<a href="https://github.com/JuliaStats/Sampling.jl">官网</a></li>
</ul>
<h4><a id="user-content-杂项演示文稿" class="anchor" href="#杂项演示文稿" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#misc-stuff--presentations"></a>杂项/演示文稿</h4>
<ul>
<li>DSP：数字信号处理。<a href="https://github.com/JuliaDSP/DSP">官网</a></li>
<li>JuliaCon Presentations：Julia大会上的演示文稿。<a href="https://github.com/JuliaCon/presentations">官网</a></li>
<li>SignalProcessing：Julia的信号处理工具。<a href="https://github.com/davidavdav/SignalProcessing">官网</a></li>
<li>Images：Julia的图片库。<a href="https://github.com/timholy/Images.jl">官网</a></li>
</ul>
<h2><a id="" class="anchor" href="#" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#matlab"></a></h2>
<h2><a id="user-content-lua" class="anchor" href="#lua" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Lua</h2>
<h4><a id="user-content-通用机器学习-6" class="anchor" href="#通用机器学习-6" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning#general-purpose-machine-learning-7"></a>通用机器学习</h4>
<ul>
<li><a href="http://torch.ch/">Torch7</a>。
<ul>
<li>cephes：—Cephes数学函数库，包装成Torch可用形式提供并包装了超过180个特殊的数学函数，由Stephen L. Moshier开发，是SciPy的核心，应用于很多场合。<a href="http://jucor.github.io/torch-cephes">官网</a></li>
<li>graph：供Torch使用的图形包。<a href="https://github.com/torch/graph">官网</a></li>
<li>randomkit：从Numpy提取的随机数生成包，包装成Torch可用形式。<a href="http://jucor.github.io/torch-randomkit/">官网</a></li>
<li>signal：Torch-7可用的信号处理工具包，可进行FFT, DCT, Hilbert, cepstrums, stft等变换。<a href="http://soumith.ch/torch-signal/signal/">官网</a></li>
<li>nn：Torch可用的神经网络包。<a href="https://github.com/torch/nn">官网</a></li>
<li>nngraph：为nn库提供图形计算能力。<a href="https://github.com/torch/nngraph">官网</a></li>
<li>nnx：一个不稳定实验性的包，扩展Torch内置的nn库。<a href="https://github.com/clementfarabet/lua---nnx">官网</a></li>
<li>optim：Torch可用的优化算法库，包括 SGD, Adagrad, 共轭梯度算法, LBFGS, RProp等算法。<a href="https://github.com/torch/optim">官网</a></li>
<li>unsup：Torch下的非监督学习包提供的模块与nn（LinearPsd、ConvPsd、AutoEncoder、...）及独立算法（k-means、PCA）等兼容。<a href="https://github.com/koraykv/unsup">官网</a></li>
<li>manifold：操作流形的包。<a href="https://github.com/clementfarabet/manifold">官网</a></li>
<li>svm：Torch的支持向量机库。<a href="https://github.com/koraykv/torch-svm">官网</a></li>
<li>lbfgs：将liblbfgs包装为FFI接口。<a href="https://github.com/clementfarabet/lbfgs">官网</a></li>
<li>vowpalwabbit：老版的vowpalwabbit对torch的接口。<a href="https://github.com/clementfarabet/vowpal_wabbit">官网</a></li>
<li>OpenGM：OpenGM是C++编写的图形建模及推断库，该binding可以用Lua以简单的方式描述图形，然后用OpenGM优化。<a href="https://github.com/clementfarabet/lua---opengm">官网</a>。</li>
<li>sphagetti：MichaelMathieu为torch7编写的稀疏线性模块。<a href="https://github.com/MichaelMathieu/lua---spaghetti">官网</a></li>
<li>LuaSHKit：将局部敏感哈希库SHKit包装成lua可用形式。<a href="https://github.com/ocallaco/LuaSHkit">官网</a></li>
<li>kernel smoothing：KNN、核权平均以及局部线性回归平滑器。<a href="https://github.com/rlowrance/kernel-smoothers">官网</a></li>
<li>cutorch：torch的CUDA后端实现。<a href="https://github.com/torch/cutorch">官网</a></li>
<li>cunn：torch的CUDA神经网络实现。<a href="https://github.com/torch/cunn">官网</a></li>
<li>imgraph：torch的图像/图形库，提供从图像创建图形、分割、建立树、又转化回图像的例程。<a href="https://github.com/clementfarabet/lua---imgraph">官网</a></li>
<li>videograph：torch的视频/图形库，提供从视频创建图形、分割、建立树、又转化回视频的例程。<a href="https://github.com/clementfarabet/videograph">官网</a></li>
<li>saliency：积分图像的代码和工具，用来从快速积分直方图中寻找兴趣点。<a href="https://github.com/marcoscoffier/torch-saliency">官网</a></li>
<li>stitch：使用hugin拼合图像并将其生成视频序列。<a href="https://github.com/marcoscoffier/lua---stitch">官网</a></li>
<li>sfm：运动场景束调整/结构包。<a href="https://github.com/marcoscoffier/lua---sfm">官网</a></li>
<li>fex：torch的特征提取包，提供SIFT和dSIFT模块。<a href="https://github.com/koraykv/fex">官网</a></li>
<li>OverFeat：当前最高水准的通用密度特征提取器。<a href="https://github.com/sermanet/OverFeat">官网</a></li>
</ul>
</li>
<li>Numeric Lua：<a href="http://numlua.luaforge.net/">官网</a>。</li>
<li>Lunatic Python：<a href="http://labix.org/lunatic-python">官网</a>。</li>
<li>SciLua：<a href="http://www.scilua.org/">官网</a>。</li>
<li>Lua - Numerical Algorithms：<a href="https://bitbucket.org/lucashnegri/lna">官网</a>。</li>
<li>Lunum：<a href="http://zrake.webfactional.com/projects/lunum">官网</a>。</li>
</ul>
<h4><a id="user-content-演示及脚本" class="anchor" href="#演示及脚本" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning#demos-and-scripts"></a>演示及脚本</h4>
<ul>
<li>Core torch7 demos repository：核心torch7演示程序库。<a href="https://github.com/e-lab/torch7-demos">官网</a>
<ul>
<li>线性回归、逻辑回归</li>
<li>人脸检测（训练和检测是独立的演示）</li>
<li>基于mst的断词器</li>
<li>train-a-digit-classifier</li>
<li>train-autoencoder</li>
<li>optical flow demo</li>
<li>train-on-housenumbers</li>
<li>train-on-cifar</li>
<li>tracking with deep nets</li>
<li>kinect demo</li>
<li>滤波可视化</li>
<li>saliency-networks</li>
</ul>
</li>
<li>Training a Convnet for the Galaxy-Zoo Kaggle challenge(CUDA demo)：<a href="https://github.com/soumith/galaxyzoo">官网</a></li>
<li>Music Tagging：torch7下的音乐标签脚本。<a href="https://github.com/mbhenaff/MusicTagging">官网</a></li>
<li>torch-datasets：<a href="https://github.com/rosejn/torch-datasets">官网</a> 读取几个流行的数据集的脚本，包括
<ul>
<li>BSR 500</li>
<li>CIFAR-10</li>
<li>COIL</li>
<li>Street View House Numbers</li>
<li>MNIST</li>
<li>NORB</li>
</ul>
</li>
<li>Atari2600：在Arcade Learning Environment模拟器中用静态帧生成数据集的脚本。<a href="https://github.com/fidlej/aledataset">官网</a></li>
</ul>
<h2><a id="user-content-matlab" class="anchor" href="#matlab" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Matlab</h2>
<h4><a id="user-content-计算机视觉-1" class="anchor" href="#计算机视觉-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#computer-vision"></a>计算机视觉</h4>
<ul>
<li>Contourlets：实现轮廓波变换及其使用函数的MATLAB源代码。<a href="http://www.ifp.illinois.edu/%7Eminhdo/software/contourlet_toolbox.tar">官网</a> 。</li>
<li>Shearlets：剪切波变换的MATLAB源码。<a href="http://www.shearlab.org/index_software.html">官网</a></li>
<li>Curvelets：Curvelet变换的MATLAB源码（Curvelet变换是对小波变换向更高维的推广，用来在不同尺度角度表示图像）。<a href="http://www.curvelet.org/software.html">官网</a></li>
<li>Bandlets：Bandlets变换的MATLAB源码。<a href="http://www.cmap.polytechnique.fr/%7Epeyre/download/">官网</a></li>
</ul>
<h4><a id="user-content-自然语言处理-4" class="anchor" href="#自然语言处理-4" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#natural-language-processing-4"></a>自然语言处理</h4>
<ul>
<li>NLP：一个Matlab的NLP库。<a href="https://amplab.cs.berkeley.edu/2012/05/05/an-nlp-library-for-matlab/">官网</a></li>
</ul>
<h4><a id="user-content-通用机器学习-7" class="anchor" href="#通用机器学习-7" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning-6"></a>通用机器学习</h4>
<ul>
<li>Training a deep autoencoder or a classifier on MNIST digits：在MNIST字符数据集上训练一个深度的autoencoder或分类器。<a href="http://www.cs.toronto.edu/%7Ehinton/MatlabForSciencePaper.html">官网</a></li>
<li>t-Distributed Stochastic Neighbor Embedding：获奖的降维技术，特别适合于高维数据集的可视化。<a href="http://homepage.tudelft.nl/19j49/t-SNE.html">官网</a></li>
<li>Spider：Matlab机器学习的完整面向对象环境。<a href="http://people.kyb.tuebingen.mpg.de/spider/">官网</a></li>
<li>LibSVM：支持向量机程序库。<a href="http://www.csie.ntu.edu.tw/%7Ecjlin/libsvm/#matlab">官网</a></li>
<li>LibLinear：大型线性分类程序库。<a href="http://www.csie.ntu.edu.tw/%7Ecjlin/liblinear/#download">官网</a></li>
<li>Machine Learning Module：M. A .Girolami教授的机器学习课程，包括PDF、讲义及代码。<a href="https://github.com/josephmisiti/machine-learning-module">官网</a></li>
<li>Caffe：考虑了代码清洁、可读性及速度的深度学习框架。<a href="http://caffe.berkeleyvision.org/">官网</a></li>
<li>Pattern Recognition Toolbox：Matlab中的模式识别工具包、完全面向对象。<a href="https://github.com/newfolder/PRT">官网</a></li>
</ul>
<h4><a id="user-content-数据分析数据可视化-4" class="anchor" href="#数据分析数据可视化-4" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#data-analysis--data-visualization-4"></a>数据分析/数据可视化</h4>
<ul>
<li>matlab_gbl：处理图像的Matlab包。<a href="https://www.cs.purdue.edu/homes/dgleich/packages/matlab_bgl/">官网</a></li>
<li>gamic：图像算法纯Matlab高效实现，对MatlabBGL的mex函数是个补充。<a href="http://www.mathworks.com/matlabcentral/fileexchange/24134-gaimc---graph-algorithms-in-matlab-code">官网</a></li>
</ul>
<h2><a id="user-content--1" class="anchor" href="#-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#python"></a></h2>
<h2><a id="user-content-net" class="anchor" href="#net" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>.NET</h2>
<h4><a id="user-content-计算机视觉-2" class="anchor" href="#计算机视觉-2" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning#computer-vision-3"></a>计算机视觉</h4>
<ul>
<li>OpenCVDotNet：包装器，使.NET程序能使用OpenCV代码。<a href="https://code.google.com/p/opencvdotnet/">官网</a></li>
<li>Emgu CV：跨平台的包装器，能在Windows、Linus、Mac OS X、iOS和Android上编译。<a href="http://www.emgu.com/wiki/index.php/Main_Page">官网</a></li>
</ul>
<h4><a id="user-content-自然语言处理-5" class="anchor" href="#自然语言处理-5" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning#natural-language-processing-6"></a>自然语言处理</h4>
<ul>
<li>Stanford.NLP for .NET：斯坦福大学NLP包在.NET上的完全移植，还可作为NuGet包进行预编译。<a href="https://github.com/sergey-tihon/Stanford.NLP.NET/">官网</a> 。</li>
</ul>
<h4><a id="user-content-通用机器学习-8" class="anchor" href="#通用机器学习-8" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning#general-purpose-machine-learning-9"></a>通用机器学习</h4>
<ul>
<li>Accord.MachineLearning：随机抽样一致性算法、交叉验证、网格搜索这个包是Accord.NET框架的一部分支持向量机、决策树、朴素贝叶斯模。型、K-means、高斯混合模型和机器学习应用的通用算法。<a href="http://www.nuget.org/packages/Accord.MachineLearning/">官网</a>：</li>
<li>Vulpes：F#语言实现的Deep belief和深度学习包，它在Alea.cuBase下利用CUDA GPU来执行。<a href="https://github.com/fsprojects/Vulpes">官网</a></li>
<li>Encog：先进的神经网络和机器学习框架，包括用来创建多种网络的类，也支。持神经网络需要的数据规则化及处理的类它的训练采用多线程弹性传播。它也能使用GPU加快处理时间提供了图形化界面来帮助建模和训练神经网络。<a href="http://www.nuget.org/packages/encog-dotnet-core/">官网</a></li>
<li>Neural Network Designer：这是一个数据库管理系统和神经网络设计器设计器用WPF开发，也是一个UI，你可以设计你的神经网络、查询网络、创建并配置聊天机器人，它能问问题，并从你的反馈中学习这些机器人甚至可以从网络搜集信息用来输出，或是用来学习。<a href="http://bragisoft.com/">官网</a></li>
</ul>
<h4><a id="user-content-数据分析数据可视化-5" class="anchor" href="#数据分析数据可视化-5" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning#data-analysis--data-visualization-6"></a>数据分析/数据可视化</h4>
<ul>
<li>numl：numl这个机器学习库，目标就是简化预测和聚类的标准建模技术。<a href="http://www.nuget.org/packages/numl/">官网</a></li>
<li>Math.NET Numerics：Math.NET项目的数值计算基础，着眼提供科学、工程以及日常数值计算的方法和算法支持 Windows、Linux 和 。Mac上的 .Net 4.0、.Net 3.5 和 Mono ，Silverlight 5、WindowsPhone/SL 8、WindowsPhone 8.1 以及装有 PCL Portable Profiles 47 及 344的Windows 8， 装有 Xamarin的Android/iOS。<a href="http://www.nuget.org/packages/MathNet.Numerics/">官网</a></li>
<li>Sho：Sho是数据分析和科学计算的交互式环境，可以让你将脚本（IronPython语言）和编译的代码（.NET）无缝连接，以快速灵活的建立原型。<a href="http://research.microsoft.com/en-us/projects/sho/">官网</a>这个环境包括强大高效的库，如线性代数、数据可视化，可供任何.NET语言使用，还为快速开发提供了功能丰富的交互式shell</li>
</ul>
<h2><a id="user-content-python" class="anchor" href="#python" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Python</h2>
<h4><a id="user-content-计算机视觉-3" class="anchor" href="#计算机视觉-3" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>计算机视觉</h4>
<ul>
<li><a href="http://hao.jobbole.com/simplecv/">SimpleCV</a>：开源计算机视觉框架，可以访问如OpenCV等高性能计算机视觉库使用Python编写，可以在Mac、Windows以及Ubuntu上运行。<a href="http://simplecv.org/">官网</a>。</li>
</ul>
<h4><a id="user-content-自然语言处理-6" class="anchor" href="#自然语言处理-6" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#natural-language-processing-5"></a>自然语言处理</h4>
<ul>
<li>NLTK：一个领先的平台，用来编写处理人类语言数据的Python程序。<a href="http://www.nltk.org/">官网</a></li>
<li>Pattern：Python可用的web挖掘模块，包括自然语言处理、机器学习等工具。<a href="http://www.clips.ua.ac.be/pattern">官网</a></li>
<li>TextBlob：为普通自然语言处理任务提供一致的API，以NLTK和Pattern为基础，并和两者都能很好兼容。<a href="http://textblob.readthedocs.org/">官网</a>。</li>
<li>jieba：中文断词工具。<a href="https://github.com/fxsjy/jieba#jieba-1">官网</a></li>
<li>SnowNLP：中文文本处理库。<a href="https://github.com/isnowfy/snownlp">官网</a></li>
<li>loso：另一个中文断词库。<a href="https://github.com/victorlin/loso">官网</a></li>
<li>genius：基于条件随机域的中文断词库。<a href="https://github.com/duanhongyi/genius">官网</a></li>
<li>nut：自然语言理解工具包。<a href="https://github.com/pprett/nut">官网</a></li>
</ul>
<h4><a id="user-content-通用机器学习-9" class="anchor" href="#通用机器学习-9" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning-7"></a>通用机器学习</h4>
<ul>
<li>Bayesian Methods for Hackers：Python语言概率规划的电子书。<a href="https://github.com/CamDavidsonPilon/%E3%80%82Probabilistic-Programming-and-Bayesian-Methods-for-Hackers">官网</a></li>
<li>MLlib in Apache Spark：Spark下的分布式机器学习库。<a href="http://spark.apache.org/docs/latest/mllib-guide.html">官网</a></li>
<li>scikit-learn：基于SciPy的机器学习模块。<a href="http://scikit-learn.org/">官网</a></li>
<li>graphlab-create：包含多种机器学习模块的库（回归、聚类、推荐系统、图分析等），基于可以磁盘存储的DataFrame。<a href="http://graphlab.com/products/create/docs/">官网</a></li>
<li>BigML：连接外部服务器的库。<a href="https://bigml.com/">官网</a></li>
<li>pattern：Python的web挖掘模块。<a href="https://github.com/clips/pattern">官网</a></li>
<li>NuPIC：Numenta公司的智能计算平台。<a href="https://github.com/numenta/nupic">官网</a></li>
<li>Pylearn2：基于Theano的机器学习库。<a href="https://github.com/lisa-lab/pylearn2">官网</a></li>
<li>hebel：Python编写的使用GPU加速的深度学习库。<a href="https://github.com/hannes-brt/hebel">官网</a></li>
<li>gensim：主题建模工具。<a href="https://github.com/piskvorky/gensim">官网</a></li>
<li>PyBrain：另一个机器学习库。<a href="https://github.com/pybrain/pybrain">官网</a></li>
<li>Crab：可扩展的、快速推荐引擎。<a href="https://github.com/muricoca/crab">官网</a></li>
<li>python-recsys：Python实现的推荐系统。<a href="https://github.com/ocelma/python-recsys">官网</a></li>
<li>thinking bayes：关于贝叶斯分析的书籍。<a href="https://github.com/AllenDowney/ThinkBayes">官网</a></li>
<li>Restricted Boltzmann Machines：Python实现的受限波尔兹曼机。<a href="https://github.com/echen/restricted-boltzmann-machines">官网</a></li>
<li>Bolt：在线学习工具箱。<a href="https://github.com/pprett/bolt">官网</a></li>
<li>CoverTree：cover tree的Python实现，scipy.spatial.kdtree便捷的替代。<a href="https://github.com/patvarilly/CoverTree">官网</a></li>
<li>nilearn：Python实现的神经影像学机器学习库。<a href="https://github.com/nilearn/nilearn">官网</a></li>
<li>Shogun：机器学习工具箱。<a href="https://github.com/shogun-toolbox/shogun">官网</a></li>
<li>Pyevolve：遗传算法框架。<a href="https://github.com/perone/Pyevolve">官网</a></li>
<li>Caffe：考虑了代码清洁、可读性及速度的深度学习框架。<a href="http://caffe.berkeleyvision.org/">官网</a></li>
<li>breze：深度及递归神经网络的程序库，基于Theano。<a href="https://github.com/breze-no-salt/breze">官网</a></li>
</ul>
<h4><a id="user-content-数据分析数据可视化-6" class="anchor" href="#数据分析数据可视化-6" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#data-analysis--data-visualization-5"></a>数据分析/数据可视化</h4>
<ul>
<li>SciPy：基于Python的数学、科学、工程开源软件生态系统。<a href="http://www.scipy.org/">官网</a></li>
<li>NumPy：Python科学计算基础包。<a href="http://www.numpy.org/">官网</a></li>
<li>Numba：Python的低级虚拟机JIT编译器，Cython and NumPy的开发者编写，供科学计算使用。<a href="http://numba.pydata.org/">官网</a></li>
<li>NetworkX：为复杂网络使用的高效软件。<a href="https://networkx.github.io/">官网</a></li>
<li>Pandas：这个库提供了高性能、易用的数据结构及数据分析工具。<a href="http://pandas.pydata.org/">官网</a></li>
<li><a href="http://hao.jobbole.com/open-mining/">Open Mining</a>：Python中的商业智能工具（Pandas web接口）。<a href="https://github.com/avelino/mining">官网</a></li>
<li><a href="http://hao.jobbole.com/pymc/">PyMC</a>：MCMC采样工具包。<a href="https://github.com/pymc-devs/pymc">官网</a></li>
<li>zipline：Python的算法交易库。<a href="https://github.com/quantopian/zipline">官网</a></li>
<li>PyDy：全名Python Dynamics，协助基于NumPy、SciPy、IPython以及 matplotlib的动态建模工作流。<a href="https://pydy.org/">官网</a></li>
<li>SymPy：符号数学Python库。<a href="https://github.com/sympy/sympy">官网</a></li>
<li>statsmodels：Python的统计建模及计量经济学库。<a href="https://github.com/statsmodels/statsmodels">官网</a></li>
<li>astropy：Python天文学程序库，社区协作编写。<a href="http://www.astropy.org/">官网</a></li>
<li>matplotlib：Python的2D绘图库。<a href="http://matplotlib.org/">官网</a></li>
<li>bokeh：Python的交互式Web绘图库。<a href="https://github.com/ContinuumIO/bokeh">官网</a></li>
<li>plotly：Python and matplotlib的协作web绘图库。<a href="https://plot.ly/python">官网</a></li>
<li>vincent：将Python数据结构转换为Vega可视化语法。<a href="https://github.com/wrobstory/vincent">官网</a></li>
<li>d3py：Python的绘图库，基于D3.js。<a href="https://github.com/mikedewar/d3py">官网</a></li>
<li>ggplot：和R语言里的ggplot2提供同样的API。<a href="https://github.com/yhat/ggplot">官网</a></li>
<li>Kartograph.py：Python中渲染SVG图的库，效果漂亮。<a href="https://github.com/kartograph/kartograph.py">官网</a></li>
<li>pygal：Python下的SVG图表生成器。<a href="http://pygal.org/">官网</a></li>
<li>pycascading：<a href="https://github.com/twitter/pycascading">官网</a></li>
</ul>
<h4><a id="user-content-杂项脚本ipython笔记代码库" class="anchor" href="#杂项脚本ipython笔记代码库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>杂项脚本/iPython笔记/代码库<a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#misc-scripts--ipython-notebooks--codebases"></a></h4>
<ul>
<li>pattern_classification：<a href="https://github.com/rasbt/pattern_classification">官网</a></li>
<li>thinking stats 2：<a href="https://github.com/Wavelets/ThinkStats2">官网</a></li>
<li>hyperopt：<a href="https://github.com/hyperopt/hyperopt-sklearn">官网</a></li>
<li>numpic：<a href="https://github.com/numenta/nupic">官网</a></li>
<li>2012-paper-diginorm：<a href="https://github.com/ged-lab/2012-paper-diginorm">官网</a></li>
<li>ipython-notebooks：<a href="https://github.com/ogrisel/notebooks">官网</a></li>
<li>decision-weights：<a href="https://github.com/CamDavidsonPilon/decision-weights">官网</a></li>
<li>Sarah Palin LDA：Sarah Palin关于主题建模的电邮。<a href="https://github.com/Wavelets/sarah-palin-lda">官网</a></li>
<li>Diffusion Segmentation：基于扩散方法的图像分割算法集合。<a href="https://github.com/Wavelets/diffusion-segmentation">官网</a></li>
<li>Scipy Tutorials：SciPy教程，已过时，请查看scipy-lecture-notes。<a href="https://github.com/Wavelets/scipy-tutorials">官网</a></li>
<li>Crab：Python的推荐引擎库。<a href="https://github.com/marcelcaraciolo/crab">官网</a></li>
<li>BayesPy：Python中的贝叶斯推断工具。<a href="https://github.com/maxsklar/BayesPy">官网</a></li>
<li>scikit-learn tutorials：scikit-learn学习笔记系列。<a href="https://github.com/GaelVaroquaux/scikit-learn-tutorial">官网</a></li>
<li>sentiment-analyzer：推特情绪分析器。<a href="https://github.com/madhusudancs/sentiment-analyzer">官网</a></li>
<li>group-lasso：坐标下降算法实验，应用于（稀疏）群套索模型。<a href="https://github.com/fabianp/group_lasso">官网</a></li>
<li>mne-python-notebooks：使用 mne-python进行EEG/MEG数据处理的IPython笔记。<a href="https://github.com/mne-tools/mne-python-notebooks">官网</a></li>
<li>pandas cookbook：使用Python pandas库的方法书。<a href="https://github.com/jvns/pandas-cookbook">官网</a></li>
<li>climin：机器学习的优化程序库，用Python实现了梯度下降、LBFGS、rmsprop、adadelta 等算法。<a href="https://github.com/BRML/climin">官网</a></li>
</ul>
<h4><a id="user-content-kaggle竞赛源代码" class="anchor" href="#kaggle竞赛源代码" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#kaggle-competition-source-code"></a>Kaggle竞赛源代码</h4>
<ul>
<li>wiki challange：Kaggle上一个维基预测挑战赛 Dell Zhang解法的实现。<a href="https://github.com/hammer/wikichallenge">官网</a></li>
<li>kaggle insults：Kaggle上”从社交媒体评论中检测辱骂“竞赛提交的代码。<a href="https://github.com/amueller/kaggle_insults">官网</a></li>
<li>kaggle_acquire-valued-shoppers-challenge：Kaggle预测回头客挑战赛的代码。<a href="https://github.com/MLWave/%E3%80%82kaggle_acquire-valued-shoppers-challenge">官网</a></li>
<li>kaggle-cifar：Kaggle上CIFAR-10 竞赛的代码，使用cuda-convnet。<a href="https://github.com/zygmuntz/kaggle-cifar">官网</a></li>
<li>kaggle-blackbox：Kaggle上blackbox赛代码，关于深度学习。<a href="https://github.com/zygmuntz/kaggle-blackbox">官网</a></li>
<li>kaggle-accelerometer：Kaggle上加速度计数据识别用户竞赛的代码。<a href="https://github.com/zygmuntz/kaggle-accelerometer">官网</a></li>
<li>kaggle-advertised-salaries：Kaggle上用广告预测工资竞赛的代码。<a href="https://github.com/zygmuntz/kaggle-advertised-salaries">官网</a></li>
<li>kaggle amazon：Kaggle上给定员工角色预测其访问需求竞赛的代码。<a href="https://github.com/zygmuntz/kaggle-amazon">官网</a></li>
<li>kaggle-bestbuy_big：Kaggle上根据bestbuy用户查询预测点击商品竞赛的代码（大数据版）。<a href="https://github.com/zygmuntz/kaggle-bestbuy_big">官网</a></li>
<li>kaggle-bestbuy_small：Kaggle上根据bestbuy用户查询预测点击商品竞赛的代码（小数据版）。<a href="https://github.com/zygmuntz/kaggle-bestbuy_small">官网</a></li>
<li>Kaggle Dogs vs. Cats：Kaggle上从图片中识别猫和狗竞赛的代码。<a href="https://github.com/kastnerkyle/kaggle-dogs-vs-cats">官网</a></li>
<li>Kaggle Galaxy Challenge：Kaggle上遥远星系形态分类竞赛的优胜代码。<a href="https://github.com/benanne/kaggle-galaxies">官网</a></li>
<li>Kaggle Gender：Kaggle竞赛，从笔迹区分性别。<a href="https://github.com/zygmuntz/kaggle-gender">官网</a></li>
<li>Kaggle Merck：Kaggle上预测药物分子活性竞赛的代码（默克制药赞助）。<a href="https://github.com/zygmuntz/kaggle-merck">官网</a></li>
<li>Kaggle Stackoverflow：Kaggle上 预测StackOverflow网站问题是否会被关闭竞赛的代码。<a href="https://github.com/zygmuntz/kaggle-stackoverflow">官网</a></li>
<li>wine-quality：预测红酒质量。<a href="https://github.com/zygmuntz/wine-quality">官网</a></li>
</ul>
<h2><a id="user-content-ruby" class="anchor" href="#ruby" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#ruby"></a>Ruby</h2>
<h4><a id="user-content-自然语言处理-7" class="anchor" href="#自然语言处理-7" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#natural-language-processing-6"></a>自然语言处理</h4>
<ul>
<li>Treat：文本检索与注释工具包，Ruby上我见过的最全面的工具包。<a href="https://github.com/louismullie/treat">官网</a></li>
<li>Ruby Linguistics：这个框架可以用任何语言为Ruby对象构建语言学工具包。括一个语言无关的通用前端，一个将语言代码映射到语言名的模块，和一个含有很有英文语言工具的模块。<a href="http://www.deveiate.org/projects/Linguistics/">官网</a></li>
<li>Stemmer：使得Ruby可用 libstemmer_c中的接口。<a href="https://github.com/aurelian/ruby-stemmer">官网</a></li>
<li>Ruby Wordnet：WordNet的Ruby接口库。<a href="http://www.deveiate.org/projects/Ruby-WordNet/">官网</a></li>
<li>Raspel：aspell绑定到Ruby的接口。<a href="http://sourceforge.net/projects/raspell/">官网</a></li>
<li>UEA Stemmer：UEALite Stemmer的Ruby移植版，供搜索和检索用的保守的词干分析器。<a href="https://github.com/ealdent/uea-stemmer">官网</a></li>
<li>Twitter-text-rb：该程序库可以将推特中的用户名、列表和话题标签自动连接并提取出来。<a href="https://github.com/twitter/twitter-text-rb">官网</a></li>
</ul>
<h4><a id="user-content-通用机器学习-10" class="anchor" href="#通用机器学习-10" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning-8"></a>通用机器学习</h4>
<ul>
<li>Ruby Machine Learning：Ruby实现的一些机器学习算法。<a href="https://github.com/tsycho/ruby-machine-learning">官网</a></li>
<li>Machine Learning Ruby：<a href="https://github.com/mizoR/machine-learning-ruby">官网</a></li>
<li>jRuby Mahout：精华！在JRuby世界中释放了Apache Mahout的威力。<a href="https://github.com/vasinov/jruby_mahout">官网</a></li>
<li>CardMagic-Classifier：可用贝叶斯及其他分类法的通用分类器模块。<a href="https://github.com/cardmagic/classifier">官网</a></li>
<li>Neural Networks and Deep Learning：《神经网络和深度学习》一书的示例代码。<a href="https://github.com/mnielsen/neural-networks-and-deep-learning">官网</a></li>
</ul>
<h4><a id="user-content-数据分析数据可视化-7" class="anchor" href="#数据分析数据可视化-7" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据分析/数据可视化<a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#data-analysis--data-visualization-6"></a></h4>
<ul>
<li>rsruby：Ruby - R bridge。<a href="https://github.com/alexgutteridge/rsruby">官网</a></li>
<li>data-visualization-ruby：关于数据可视化的Ruby Manor演示的源代码和支持内容。<a href="https://github.com/chrislo/data_visualisation_ruby">官网</a></li>
<li>ruby-plot：将gnuplot包装为Ruby形式，特别适合将ROC曲线转化为svg文件。<a href="https://www.ruby-toolbox.com/projects/ruby-plot">官网</a></li>
<li>plot-rb：基于Vega和D3的ruby绘图库。<a href="https://github.com/zuhao/plotrb">官网</a></li>
<li>scruffy：Ruby下出色的图形工具包。<a href="http://www.rubyinside.com/scruffy-a-beautiful-graphing-toolkit-for-ruby-194.html">官网</a></li>
<li>SciRuby：<a href="http://sciruby.com/">官网</a></li>
<li>Glean：数据管理工具。<a href="https://github.com/glean/glean">官网</a></li>
<li>Bioruby：<a href="https://github.com/bioruby/bioruby">官网</a></li>
<li>Arel：<a href="https://github.com/nkallen/arel">官网</a></li>
</ul>
<h4><a id="user-content-misc-杂项" class="anchor" href="#misc-杂项" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#misc"></a>Misc 杂项</h4>
<ul>
<li>Big Data For Chimps：大数据处理严肃而有趣的指南书。<a href="https://github.com/infochimps-labs/big_data_for_chimps">官网</a></li>
</ul>
<h2><a id="user-content-r" class="anchor" href="#r" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#r"></a>R</h2>
<h4><a id="user-content-通用机器学习-11" class="anchor" href="#通用机器学习-11" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning-9"></a>通用机器学习</h4>
<ul>
<li>Clever Algorithms For Machine Learning：<a href="https://github.com/jbrownlee/CleverAlgorithmsMachineLearning">官网</a>。</li>
<li>Machine Learning For Hackers：<a href="https://github.com/johnmyleswhite/ML_for_Hackers">官网</a>。</li>
<li>Machine Learning Task View on CRAN：R语言机器学习包列表，按算法类型分组。<a href="http://cran.r-project.org/web/views/MachineLearning.html">官网</a>。</li>
<li>caret：R语言150个机器学习算法的统一接口。<a href="http://caret.r-forge.r-project.org/">官网</a></li>
<li><a href="https://github.com/ecpolley/SuperLearner">SuperLearner：该包集合了多种机器学习算法</a>与<a href="http://cran.r-project.org/web/%E3%80%82packages/subsemble/index.html">subsemble</a></li>
<li>Introduction to Statistical Learning：<a href="http://www-bcf.usc.edu/%7Egareth/ISL/">官网</a>。</li>
</ul>
<h4><a id="user-content--2" class="anchor" href="#-2" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#data-analysis--data-visualization-7"></a></h4>
<h4><a id="user-content-数据分析数据可视化-8" class="anchor" href="#数据分析数据可视化-8" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据分析/数据可视化</h4>
<ul>
<li>Learning Statistics Using R：<a href="http://health.adelaide.edu.au/psychology/ccs/teaching/lsr/">官网</a></li>
<li>ggplot2：基于图形语法的数据可视化包。<a href="http://ggplot2.org/">官网</a></li>
</ul>
<h2><a id="user-content-scala" class="anchor" href="#scala" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#scala"></a>Scala</h2>
<h4><a id="user-content-自然语言处理-8" class="anchor" href="#自然语言处理-8" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#natural-language-processing-7"></a>自然语言处理</h4>
<ul>
<li>ScalaNLP：机器学习和数值计算库的套装。<a href="http://www.scalanlp.org/">官网</a></li>
<li>Breeze：Scala用的数值处理库。<a href="https://github.com/scalanlp/breeze">官网</a></li>
<li>Chalk：自然语言处理库。<a href="https://github.com/scalanlp/chalk">官网</a></li>
<li>FACTORIE：可部署的概率建模工具包，用Scala实现的软件库为用户提供简洁的语言来创建关系因素图，评估参数并进行推断。<a href="https://github.com/factorie/factorie">官网</a>。</li>
</ul>
<h4><a id="user-content-数据分析数据可视化-9" class="anchor" href="#数据分析数据可视化-9" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#data-analysis--data-visualization-8"></a>数据分析/数据可视化</h4>
<ul>
<li>MLlib in Apache Spark：Spark下的分布式机器学习库。<a href="http://spark.apache.org/docs/latest/mllib-guide.html">官网</a></li>
<li>Scalding：CAscading的Scala接口。<a href="https://github.com/twitter/scalding">官网</a></li>
<li>Summing Bird：用Scalding 和 Storm进行Streaming MapReduce。<a href="https://github.com/twitter/summingbird">官网</a></li>
<li>Algebird：Scala的抽象代数工具。<a href="https://github.com/twitter/algebird">官网</a></li>
<li>xerial：Scala的数据管理工具。<a href="https://github.com/xerial/xerial">官网</a></li>
<li>simmer：化简你的数据，进行代数聚合的unix过滤器。<a href="https://github.com/avibryant/simmer">官网</a></li>
<li>PredictionIO：供软件开发者和数据工程师用的机器学习服务器。<a href="https://github.com/PredictionIO/PredictionIO">官网</a></li>
<li>BIDMat：支持大规模探索性数据分析的CPU和GPU加速矩阵库。<a href="https://github.com/BIDData/BIDMat">官网</a></li>
</ul>
<h4><a id="user-content-通用机器学习-12" class="anchor" href="#通用机器学习-12" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a href="https://github.com/josephmisiti/awesome-machine-learning/blob/master/README.md#general-purpose-machine-learning-10"></a>通用机器学习</h4>
<ul>
<li>Conjecture：Scalding下可扩展的机器学习框架。<a href="https://github.com/etsy/Conjecture">官网</a></li>
<li>brushfire：scalding下的决策树工具。<a href="https://github.com/avibryant/brushfire">官网</a></li>
<li>ganitha：基于scalding的机器学习程序库。<a href="https://github.com/tresata/ganitha">官网</a></li>
<li>adam：使用Apache Avro, Apache Spark 和 Parquet的基因组处理引擎，有专用的文件格式，Apache 2软件许可。<a href="https://github.com/bigdatagenomics/adam">官网</a></li>
<li>bioscala：Scala语言可用的生物信息学程序库。<a href="https://github.com/bioscala/bioscala">官网</a></li>
<li>BIDMach：机器学习CPU和GPU加速库。<a href="https://github.com/BIDData/BIDMach">官网</a></li>
</ul>

## 五、经典编程书籍

 <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-经典编程书籍大全" class="anchor" href="#经典编程书籍大全" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>经典编程书籍大全</h1>
<p>100+ 经典技术书籍，涵盖：计算机系统与网络、系统架构、算法与数据结构、前端开发、后端开发、移动开发、数据库、测试、项目与团队、程序员职业修炼、求职面试 和 编程相关的经典书籍。</p>
<h2><a id="user-content-计算机系统与网络" class="anchor" href="#计算机系统与网络" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>计算机系统与网络</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00AAQXKXS/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00AAQXKXS&amp;linkCode=as2&amp;tag=vastwork-23">图灵的秘密:他的生平、思想及论文解读</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0011F9OQE/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0011F9OQE&amp;linkCode=as2&amp;tag=vastwork-23">计算机系统概论</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0011F5RYM/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0011F5RYM&amp;linkCode=as2&amp;tag=vastwork-23">深入理解Linux内核</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B003QN7J7U/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B003QN7J7U&amp;linkCode=as2&amp;tag=vastwork-23">深入Linux内核架构</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00116OTVS/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00116OTVS&amp;linkCode=as2&amp;tag=vastwork-23">TCP/IP详解 卷1：协议</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00JUM2ML4/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00JUM2ML4&amp;linkCode=as2&amp;tag=vastwork-23">Linux系统编程（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B004X3Z3D4/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B004X3Z3D4&amp;linkCode=as2&amp;tag=vastwork-23">Linux内核设计与实现（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B004BJ18KM/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B004BJ18KM&amp;linkCode=as2&amp;tag=vastwork-23">深入理解计算机系统（原书第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0011AP7RY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0011AP7RY&amp;linkCode=as2&amp;tag=vastwork-23">计算机程序的构造和解释（原书第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B009RSXIB4/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B009RSXIB4&amp;linkCode=as2&amp;tag=vastwork-23">编码：隐匿在计算机软硬件背后的语言</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0140I5WPK/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0140I5WPK&amp;linkCode=as2&amp;tag=vastwork-23">性能之颠：洞悉系统、企业与云计算</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B011S72JB6/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B011S72JB6&amp;linkCode=as2&amp;tag=vastwork-23">UNIX网络编程 卷1：套接字联网API（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B012R5A29O/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B012R5A29O&amp;linkCode=as2&amp;tag=vastwork-23">UNIX网络编程 卷2：进程间通信</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B001GS7918/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B001GS7918&amp;linkCode=as2&amp;tag=vastwork-23">Windows核心编程(第5版)</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00PB5QQ84/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00PB5QQ84&amp;linkCode=as2&amp;tag=vastwork-23">WireShark网络分析就这么简单</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01AS1OS8A/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01AS1OS8A&amp;linkCode=as2&amp;tag=vastwork-23">WireShark网络分析的艺术</a>》</li>
</ul>
<h2><a id="user-content-编程通用" class="anchor" href="#编程通用" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>编程通用</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B006P7V73G/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B006P7V73G&amp;linkCode=as2&amp;tag=vastwork-23">编程原本</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0061XKRXA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0061XKRXA&amp;linkCode=as2&amp;tag=vastwork-23">代码大全</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B008Z1IEQ8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B008Z1IEQ8&amp;linkCode=as2&amp;tag=vastwork-23">UNIX编程艺术</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0031M9GHC/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0031M9GHC&amp;linkCode=as2&amp;tag=vastwork-23">代码整洁之道</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00SFZH0DC/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00SFZH0DC&amp;linkCode=as2&amp;tag=vastwork-23">编程珠玑（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0150BMQDM/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0150BMQDM&amp;linkCode=as2&amp;tag=vastwork-23">编程珠玑（续）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00IOAM6VE/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00IOAM6VE&amp;linkCode=as2&amp;tag=vastwork-23">软件调试的艺术</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00KMJ2Q1U/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00KMJ2Q1U&amp;linkCode=as2&amp;tag=vastwork-23">修改代码的艺术</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B007HYMPBY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B007HYMPBY&amp;linkCode=as2&amp;tag=vastwork-23">编程语言实现模式</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B008B4DTG4/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B008B4DTG4&amp;linkCode=as2&amp;tag=vastwork-23">编写可读代码的艺术</a>》</li>
<li>《解析极限编程：拥抱变化》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B008UCHA58/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B008UCHA58&amp;linkCode=as2&amp;tag=vastwork-23">精通正则表达式（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B001NGO85I/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B001NGO85I&amp;linkCode=as2&amp;tag=vastwork-23">编译原理（第2版）</a>》龙书</li>
<li>《<a href="https://www.amazon.cn/gp/product/B011LPUB42/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B011LPUB42&amp;linkCode=as2&amp;tag=vastwork-23">重构：改善既有代码的设计</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00ALPRM3M/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00ALPRM3M&amp;linkCode=as2&amp;tag=vastwork-23">七周七语言：理解多种编程范型</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00CBBLUFK/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00CBBLUFK&amp;linkCode=as2&amp;tag=vastwork-23">调试九法：软硬件错误的排查之道</a>》</li>
<li>《程序设计语言：实践之路（第3版）》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00PG0MM3C/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00PG0MM3C&amp;linkCode=as2&amp;tag=vastwork-23">计算的本质：深入剖析程序和计算机</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B001130JN8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B001130JN8&amp;linkCode=as2&amp;tag=vastwork-23">设计模式 : 可复用面向对象软件的基础</a>》</li>
</ul>
<h2><a id="user-content-算法与数据结构" class="anchor" href="#算法与数据结构" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>算法与数据结构</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B009OCFQ0O/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B009OCFQ0O&amp;linkCode=as2&amp;tag=vastwork-23">算法（第4版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00AK7BYJY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00AK7BYJY&amp;linkCode=as2&amp;tag=vastwork-23">算法导论（原书第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B019NB0VCI/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B019NB0VCI&amp;linkCode=as2&amp;tag=vastwork-23">Python算法教程</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00S4HCQUI/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00S4HCQUI&amp;linkCode=as2&amp;tag=vastwork-23">算法设计与分析基础（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B016DWSF8M/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B016DWSF8M&amp;linkCode=as2&amp;tag=vastwork-23">学习 JavaScript 数据结构与算法</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01LDG2DSG/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01LDG2DSG&amp;linkCode=as2&amp;tag=vastwork-23">数据结构与算法分析 : C++描述（第4版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B002WC7NGS/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B002WC7NGS&amp;linkCode=as2&amp;tag=vastwork-23">数据结构与算法分析 : C语言描述（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01CNP0CG6/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01CNP0CG6&amp;linkCode=as2&amp;tag=vastwork-23">数据结构与算法分析 : Java语言描述（第2版）</a>》</li>
</ul>
<h2><a id="user-content-职业修炼与规划" class="anchor" href="#职业修炼与规划" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>职业修炼与规划</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00KQDTZ4S/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00KQDTZ4S&amp;linkCode=as2&amp;tag=vastwork-23">大教堂与集市</a>》</li>
<li>《卓有成效的程序员》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01LZJ8L9J/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01LZJ8L9J&amp;linkCode=as2&amp;tag=vastwork-23">程序员的职业素养</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B004GV08CY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B004GV08CY&amp;linkCode=as2&amp;tag=vastwork-23">程序员修炼之道：从小工到专家</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00H6X6LD4/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00H6X6LD4&amp;linkCode=as2&amp;tag=vastwork-23">软件开发者路线图：从学徒到高手</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00CBBKDGM/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00CBBKDGM&amp;linkCode=as2&amp;tag=vastwork-23">我编程，我快乐: 程序员职业规划之道</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B007VARUIM/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B007VARUIM&amp;linkCode=as2&amp;tag=vastwork-23">程序员的思维修炼：开发认知潜能的九堂课</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00OA9L3NU/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00OA9L3NU&amp;linkCode=as2&amp;tag=vastwork-23">高效程序员的45个习惯：敏捷开发修炼之道(修订版)</a>》</li>
</ul>
<h2><a id="user-content-大师访谈" class="anchor" href="#大师访谈" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>大师访谈</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00451BP72/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00451BP72&amp;linkCode=as2&amp;tag=vastwork-23">编程大师智慧</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00ALPRKMA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00ALPRKMA&amp;linkCode=as2&amp;tag=vastwork-23">编程大师访谈录</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00QA7GA2Y/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00QA7GA2Y&amp;linkCode=as2&amp;tag=vastwork-23">编程人生 : 15位软件先驱访谈录</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B007ED88CI/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B007ED88CI&amp;linkCode=as2&amp;tag=vastwork-23">奇思妙想 : 15位计算机天才及其重大发现</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B008G80O9K/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B008G80O9K&amp;linkCode=as2&amp;tag=vastwork-23">图灵和ACM图灵奖</a>》</li>
</ul>
<h2><a id="user-content-架构性能" class="anchor" href="#架构性能" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>架构/性能</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B01ER75V6O/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01ER75V6O&amp;linkCode=as2&amp;tag=vastwork-23">微服务设计</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00NGW4EAG/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00NGW4EAG&amp;linkCode=as2&amp;tag=vastwork-23">大数据日知录</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B003LBSRDM/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B003LBSRDM&amp;linkCode=as2&amp;tag=vastwork-23">企业应用架构模式</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00JMKWHFU/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00JMKWHFU&amp;linkCode=as2&amp;tag=vastwork-23">Web性能权威指南</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01M0EHQ43/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01M0EHQ43&amp;linkCode=as2&amp;tag=vastwork-23">SRE：Google运维解密</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0153178XM/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0153178XM&amp;linkCode=as2&amp;tag=vastwork-23">发布！软件的设计与部署</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01HZFHQQI/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01HZFHQQI&amp;linkCode=as2&amp;tag=vastwork-23">高扩展性网站的 50 条原则</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00F3Z26G8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00F3Z26G8&amp;linkCode=as2&amp;tag=vastwork-23">大型网站技术架构:核心原理与案例分析</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00EP6TGAU/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00EP6TGAU&amp;linkCode=as2&amp;tag=vastwork-23">恰如其分的软件架构：风险驱动的设计方法</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00CMMUXC4/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00CMMUXC4&amp;linkCode=as2&amp;tag=vastwork-23">软件系统架构：使用视点和视角与利益相关者合作（第2版）</a>》</li>
</ul>
<h2><a id="user-content-web前端" class="anchor" href="#web前端" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Web前端</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B013SGB2AO/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B013SGB2AO&amp;linkCode=as2&amp;tag=vastwork-23">高性能 JavaScript</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0089TDFNS/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0089TDFNS&amp;linkCode=as2&amp;tag=vastwork-23">锋利的 jQuery（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B016DWSEWO/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B016DWSEWO&amp;linkCode=as2&amp;tag=vastwork-23">JavaScript 忍者秘籍</a>》（感谢<a href="https://github.com/jobbole/awesome-programming-books/issues?q=is%3Aissue+is%3Aopen+author%3Ajoker-danta">@joker-danta</a> 补充推荐）</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00BQ7RMW0/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00BQ7RMW0&amp;linkCode=as2&amp;tag=vastwork-23">编写可维护的 JavaScript</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00W34DZ8K/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00W34DZ8K&amp;linkCode=as2&amp;tag=vastwork-23">你不知道的 JavaScript（上）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B007VISQ1Y/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B007VISQ1Y&amp;linkCode=as2&amp;tag=vastwork-23">JavaScript 权威指南（第6版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0097CON2S/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0097CON2S&amp;linkCode=as2&amp;tag=vastwork-23">JavaScript 语言精粹（修订版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B004VJM5KE/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B004VJM5KE&amp;linkCode=as2&amp;tag=vastwork-23">JavaScript DOM编程艺术 （第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B007OQQVMY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B007OQQVMY&amp;linkCode=as2&amp;tag=vastwork-23">JavaScript 高级程序设计（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00JVLEYY2/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00JVLEYY2&amp;linkCode=as2&amp;tag=vastwork-23">JavaScript 异步编程：设计快速响应的网络应用</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00GMXI1QY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00GMXI1QY&amp;linkCode=as2&amp;tag=vastwork-23">Effective JavaScript：编写高质量JavaScript代码的68个有效方法</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00H706BIG/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00H706BIG&amp;linkCode=as2&amp;tag=vastwork-23">HTML5 权威指南</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B015316VJY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B015316VJY&amp;linkCode=as2&amp;tag=vastwork-23">HTML5 秘籍（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00K58535O/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00K58535O&amp;linkCode=as2&amp;tag=vastwork-23">HTML5 与 CSS3 基础教程（第八版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01ET3FO86/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01ET3FO86&amp;linkCode=as2&amp;tag=vastwork-23">CSS 揭秘</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00M2DKZ1W/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00M2DKZ1W&amp;linkCode=as2&amp;tag=vastwork-23">CSS 设计指南（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0011F5SIC/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0011F5SIC&amp;linkCode=as2&amp;tag=vastwork-23">CSS 权威指南（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01LXL42O5/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01LXL42O5&amp;linkCode=as2&amp;tag=vastwork-23">深入浅出 HTML 与 CSS</a>》</li>
</ul>
<h2><a id="user-content-java开发" class="anchor" href="#java开发" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Java开发</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B01ER75QC8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01ER75QC8&amp;linkCode=as2&amp;tag=vastwork-23">Java8 实战</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0077K9XHW/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0077K9XHW&amp;linkCode=as2&amp;tag=vastwork-23">Java并发编程实战</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01DLB7Z66/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01DLB7Z66&amp;linkCode=as2&amp;tag=vastwork-23">Java性能权威指南</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00E0D2OX4/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00E0D2OX4&amp;linkCode=as2&amp;tag=vastwork-23">Java程序员修炼之道</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B017MEN094/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B017MEN094&amp;linkCode=as2&amp;tag=vastwork-23">实战Java高并发程序设计</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0011F7WU4/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0011F7WU4&amp;linkCode=as2&amp;tag=vastwork-23">Java编程思想 （第4版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01HI0BUF8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01HI0BUF8&amp;linkCode=as2&amp;tag=vastwork-23">深入理解Java虚拟机（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B001PTGR52/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B001PTGR52&amp;linkCode=as2&amp;tag=vastwork-23">Effective java 中文版（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01M22BGUQ/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01M22BGUQ&amp;linkCode=as2&amp;tag=vastwork-23">Java核心技术·卷1：基础知识（原书第9版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00IK7SM6O/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00IK7SM6O&amp;linkCode=as2&amp;tag=vastwork-23">Java核心技术·卷2：高级特性（原书第9版）</a>》</li>
</ul>
<h2><a id="user-content-net" class="anchor" href="#net" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>.NET</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00DVDDP0K/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00DVDDP0K&amp;linkCode=as2&amp;tag=vastwork-23">精通C#（第6版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00J94AG2A/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00J94AG2A&amp;linkCode=as2&amp;tag=vastwork-23">深入理解C#（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00P8VZ8T4/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00P8VZ8T4&amp;linkCode=as2&amp;tag=vastwork-23">CLR via C#（第4版）</a>》</li>
</ul>
<h2><a id="user-content-python" class="anchor" href="#python" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Python</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00UI93JD8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00UI93JD8&amp;linkCode=as2&amp;tag=vastwork-23">集体智慧编程</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00P6OJ0TC/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00P6OJ0TC&amp;linkCode=as2&amp;tag=vastwork-23">笨办法学Python</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00KAFX65Q/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00KAFX65Q&amp;linkCode=as2&amp;tag=vastwork-23">Python基础教程</a>》</li>
<li>《Python源码剖析》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B007NB2B4M/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B007NB2B4M&amp;linkCode=as2&amp;tag=vastwork-23">Head First Python</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00HECW20S/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00HECW20S&amp;linkCode=as2&amp;tag=vastwork-23">与孩子一起学编程</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B004TUJ7A6/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B004TUJ7A6&amp;linkCode=as2&amp;tag=vastwork-23">Python学习手册（第4版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00WKR1OKG/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00WKR1OKG&amp;linkCode=as2&amp;tag=vastwork-23">Python Cookbook（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01MCUN37Y/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01MCUN37Y&amp;linkCode=as2&amp;tag=vastwork-23">Python参考手册（第4版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01FQAS0KK/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01FQAS0KK&amp;linkCode=as2&amp;tag=vastwork-23">Python核心编程（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01HCVUJFA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01HCVUJFA&amp;linkCode=as2&amp;tag=vastwork-23">Python科学计算（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00GHGZLWS/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00GHGZLWS&amp;linkCode=as2&amp;tag=vastwork-23">利用 Python 进行数据分析</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01ION3W54/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01ION3W54&amp;linkCode=as2&amp;tag=vastwork-23">Think Python：像计算机科学家一样思考Python（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00MHDPIJ6/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00MHDPIJ6&amp;linkCode=as2&amp;tag=vastwork-23">Python编程实战:运用设计模式、并发和程序库创建高质量程序</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B019ZRGBVU/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B019ZRGBVU&amp;linkCode=as2&amp;tag=vastwork-23">Python绝技：运用Python成为顶级黑客</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0153177A6/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0153177A6&amp;linkCode=as2&amp;tag=vastwork-23">Flask Web开发:基于Python的Web应用开发实战</a>》</li>
</ul>
<h2><a id="user-content-android" class="anchor" href="#android" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Android</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B01FSXCBOQ/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01FSXCBOQ&amp;linkCode=as2&amp;tag=vastwork-23">Android编程权威指南（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00SFZGX08/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00SFZGX08&amp;linkCode=as2&amp;tag=vastwork-23">移动应用UI设计模式（第2版）</a>》</li>
</ul>
<h2><a id="user-content-ios" class="anchor" href="#ios" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>iOS</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00NKZCM3U/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00NKZCM3U&amp;linkCode=as2&amp;tag=vastwork-23">iOS编程实战</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B013UG2ULW/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B013UG2ULW&amp;linkCode=as2&amp;tag=vastwork-23">iOS编程（第4版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00DE60G3S/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00DE60G3S&amp;linkCode=as2&amp;tag=vastwork-23">Objective-C高级编程</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00IDSGY06/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00IDSGY06&amp;linkCode=as2&amp;tag=vastwork-23">Effective Objective-C 2.0：编写高质量iOS与OS X代码的52个有效方法</a>》</li>
</ul>
<h2><a id="user-content-php" class="anchor" href="#php" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>PHP</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B004R1QIJU/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B004R1QIJU&amp;linkCode=as2&amp;tag=vastwork-23">Head First PHP &amp; MySQL（中文版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B005D6IRRY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B005D6IRRY&amp;linkCode=as2&amp;tag=vastwork-23">深入PHP：面向对象、模式与实践（第3版）</a>》</li>
</ul>
<h2><a id="user-content-c语言" class="anchor" href="#c语言" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>C语言</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00IZW4DK8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00IZW4DK8&amp;linkCode=as2&amp;tag=vastwork-23">C标准库</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00163LU68/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00163LU68&amp;linkCode=as2&amp;tag=vastwork-23">C和指针</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0012NIW9K/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0012NIW9K&amp;linkCode=as2&amp;tag=vastwork-23">C专家编程</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0012UMPBY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0012UMPBY&amp;linkCode=as2&amp;tag=vastwork-23">C陷阱与缺陷</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01D10NSCM/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01D10NSCM&amp;linkCode=as2&amp;tag=vastwork-23">C语言接口与实现</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0011425T8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0011425T8&amp;linkCode=as2&amp;tag=vastwork-23">C程序设计语言（第2版）</a>》</li>
<li>《C语言参考手册（第5版）》</li>
</ul>
<h2><a id="user-content-c" class="anchor" href="#c" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>C++</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00YLZIRHI/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00YLZIRHI&amp;linkCode=as2&amp;tag=vastwork-23">C++标准库</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B005CFUQR0/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B005CFUQR0&amp;linkCode=as2&amp;tag=vastwork-23">C++编程思想</a>》</li>
<li>《C++语言的设计与演化》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B003VPX6YS/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B003VPX6YS&amp;linkCode=as2&amp;tag=vastwork-23">C++程序设计原理与实践</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00ESUIL0O/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00ESUIL0O&amp;linkCode=as2&amp;tag=vastwork-23">C++ Primer （中文第5版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00S6U4C6E/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00S6U4C6E&amp;linkCode=as2&amp;tag=vastwork-23">C++ Primer习题集(第5版)</a> 》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01I9BNASA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01I9BNASA&amp;linkCode=as2&amp;tag=vastwork-23">C++程序设计语言(第1-3部分)(原书第4版)</a> 》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B004G72P24/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B004G72P24&amp;linkCode=as2&amp;tag=vastwork-23">Effective C++:改善程序与设计的55个具体做法(第3版)(中文版) </a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B004IP8BD6/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B004IP8BD6&amp;linkCode=as2&amp;tag=vastwork-23">More Effective C++:35个改善编程与设计的有效方法(中文版) </a>》
 </li>
</ul>
<h2><a id="user-content-机器学习和数据挖掘" class="anchor" href="#机器学习和数据挖掘" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>机器学习和数据挖掘</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00JUE9DXW/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00JUE9DXW&amp;linkCode=as2&amp;tag=vastwork-23">数据之巅</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00NTM5GK0/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00NTM5GK0&amp;linkCode=as2&amp;tag=vastwork-23">矩阵分析</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B002WC7NH2/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B002WC7NH2&amp;linkCode=as2&amp;tag=vastwork-23">机器学习</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B007TSFMTA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B007TSFMTA&amp;linkCode=as2&amp;tag=vastwork-23">统计学习方法</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B01AG3ZV9K/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B01AG3ZV9K&amp;linkCode=as2&amp;tag=vastwork-23">机器学习导论</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B008AK5YJO/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B008AK5YJO&amp;linkCode=as2&amp;tag=vastwork-23">推荐系统实践</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00D747PTK/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00D747PTK&amp;linkCode=as2&amp;tag=vastwork-23">机器学习实战</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00AY830HS/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00AY830HS&amp;linkCode=as2&amp;tag=vastwork-23">Web数据挖掘</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B006PHIVNA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B006PHIVNA&amp;linkCode=as2&amp;tag=vastwork-23">深入浅出统计学</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00116C3DY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00116C3DY&amp;linkCode=as2&amp;tag=vastwork-23">模式分类（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00264GG56/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00264GG56&amp;linkCode=as2&amp;tag=vastwork-23">概率论与数理统计</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00PRH2BXA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00PRH2BXA&amp;linkCode=as2&amp;tag=vastwork-23">统计学习基础(第2版)(英文)</a> 》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B007NR0T4A/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B007NR0T4A&amp;linkCode=as2&amp;tag=vastwork-23">数据挖掘：概念与技术（第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00K5I91WK/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00K5I91WK&amp;linkCode=as2&amp;tag=vastwork-23">数据挖掘：实用机器学习工具与技术（原书第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B011I34CGA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B011I34CGA&amp;linkCode=as2&amp;tag=vastwork-23">大数据：互联网大规模数据挖掘与分布式处理（第2版）</a>》</li>
</ul>
<h2><a id="user-content-数据库" class="anchor" href="#数据库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>数据库</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00H6X6M1A/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00H6X6M1A&amp;linkCode=as2&amp;tag=vastwork-23">SQL应用重构</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/0596009763/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=0596009763&amp;linkCode=as2&amp;tag=vastwork-23">SQL Cookbook</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00C1W58DE/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00C1W58DE&amp;linkCode=as2&amp;tag=vastwork-23">高性能MySQL （第3版）</a>》</li>
<li>《深入浅出SQL（中文版）》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00ETOV48K/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00ETOV48K&amp;linkCode=as2&amp;tag=vastwork-23">MySQL技术内幕 : InnoDB存储引擎（第2版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00KR87J8G/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00KR87J8G&amp;linkCode=as2&amp;tag=vastwork-23">深入浅出MySQL : 数据库开发、优化与管理维护</a>》</li>
</ul>
<h2><a id="user-content-测试" class="anchor" href="#测试" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>测试</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B003JBIV0S/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B003JBIV0S&amp;linkCode=as2&amp;tag=vastwork-23">探索式软件测试</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00PVOND2W/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00PVOND2W&amp;linkCode=as2&amp;tag=vastwork-23">有效的单元测试</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00FH36R6G/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00FH36R6G&amp;linkCode=as2&amp;tag=vastwork-23">Google软件测试之道</a>》</li>
</ul>
<h2><a id="user-content-项目与团队" class="anchor" href="#项目与团队" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>项目与团队</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00VR8ZO28/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00VR8ZO28&amp;linkCode=as2&amp;tag=vastwork-23">人月神话</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B001DBRWL0/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B001DBRWL0&amp;linkCode=as2&amp;tag=vastwork-23">快速软件开发</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00MO7R1SG/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00MO7R1SG&amp;linkCode=as2&amp;tag=vastwork-23">人件（原书第3版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00CBBKRQ8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00CBBKRQ8&amp;linkCode=as2&amp;tag=vastwork-23">门后的秘密：卓越管理的故事</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00BLZMG8W/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00BLZMG8W&amp;linkCode=as2&amp;tag=vastwork-23">极客与团队：软件工程师的团队生存秘笈</a>》</li>
</ul>
<h2><a id="user-content-求职面试" class="anchor" href="#求职面试" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>求职面试</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B00G8VOQOG/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00G8VOQOG&amp;linkCode=as2&amp;tag=vastwork-23">程序员面试金典（第5版）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00W5269HO/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00W5269HO&amp;linkCode=as2&amp;tag=vastwork-23">编程之美 : 微软技术面试心得</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00ALPRM7S/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00ALPRM7S&amp;linkCode=as2&amp;tag=vastwork-23">金领简历：敲开苹果、微软、谷歌的大门</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00L5LKMVU/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00L5LKMVU&amp;linkCode=as2&amp;tag=vastwork-23">剑指Offer：名企面试官精讲典型编程题（纪念版）</a>》</li>
</ul>
<h2><a id="user-content-编程之外" class="anchor" href="#编程之外" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>编程之外</h2>
<ul>
<li>《<a href="https://www.amazon.cn/gp/product/B005DSK4W8/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B005DSK4W8&amp;linkCode=as2&amp;tag=vastwork-23">暗时间</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00P6OJ09C/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00P6OJ09C&amp;linkCode=as2&amp;tag=vastwork-23">数学之美</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00ANY9KZE/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00ANY9KZE&amp;linkCode=as2&amp;tag=vastwork-23">赢得朋友</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B008MIFWJG/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B008MIFWJG&amp;linkCode=as2&amp;tag=vastwork-23">精益创业</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00QPZARMA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00QPZARMA&amp;linkCode=as2&amp;tag=vastwork-23">批判性思维</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00M2DKZNA/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00M2DKZNA&amp;linkCode=as2&amp;tag=vastwork-23">世界是数字的</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00A4H3JJS/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00A4H3JJS&amp;linkCode=as2&amp;tag=vastwork-23">程序员的数学</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00N4LZ6RO/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00N4LZ6RO&amp;linkCode=as2&amp;tag=vastwork-23">程序员健康指南</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B005O4PUFC/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B005O4PUFC&amp;linkCode=as2&amp;tag=vastwork-23">禅与摩托车维修艺术</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B0081M8TZ2/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B0081M8TZ2&amp;linkCode=as2&amp;tag=vastwork-23">关键对话：如何高效能沟通</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00EY8JUBO/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00EY8JUBO&amp;linkCode=as2&amp;tag=vastwork-23">写作法宝：非虚构写作指南</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00G1ZT2C0/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00G1ZT2C0&amp;linkCode=as2&amp;tag=vastwork-23">黑客与画家 : 来自计算机时代的高见</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00WDTQU8M/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00WDTQU8M&amp;linkCode=as2&amp;tag=vastwork-23">软件随想录（卷1）</a>》《<a href="https://www.amazon.cn/gp/product/B00WFT32FY/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00WFT32FY&amp;linkCode=as2&amp;tag=vastwork-23">软件随想录（卷2）</a>》</li>
<li>《<a href="https://www.amazon.cn/gp/product/B00ICWNKT6/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&amp;camp=536&amp;creative=3200&amp;creativeASIN=B00ICWNKT6&amp;linkCode=as2&amp;tag=vastwork-23">如何把事情做到最好：改变全球9800万人的人生指导书</a>》</li>
</ul>
</article>
  </div>

