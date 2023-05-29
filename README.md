## Laboratory work I

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [ ] 1. Ознакомиться со ссылками учебного материала
- [ ] 2. Выполнить инструкцию учебного материала
- [ ] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**

## Tutorial

```bash
$ export GITHUB_USERNAME=HECCYLLIujTbmy
$ export GIST_TOKEN=<сохраненный_токен>
$ alias edit=nano
```

```sh
$ mkdir -p ${GITHUB_USERNAME}/workspace
$ cd ${GITHUB_USERNAME}/workspace
$ pwd
$ cd ..
$ pwd
```

```sh
$ mkdir -p workspace/tasks/
$ mkdir -p workspace/projects/
$ mkdir -p workspace/reports/
$ cd workspace
```

```sh
# Debian
$ wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
$ tar -xf node-v6.11.5-linux-x64.tar.xz
$ rm -rf node-v6.11.5-linux-x64.tar.xz
$ mv node-v6.11.5-linux-x64 node
```

```sh
$ ls node/bin
$ echo ${PATH}
$ export PATH=${PATH}:`pwd`/node/bin
$ echo ${PATH}
$ mkdir scripts
$ cat > scripts/activate<<EOF
export PATH=\${PATH}:`pwd`/node/bin
EOF
$ source scripts/activate
```

```sh
$ gem install gist
```

```sh
$ (umask 0077 && echo ${GIST_TOKEN} > ~/.gist)
```

## Report

```sh
$ export LAB_NUMBER=01
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
$ mkdir reports/lab${LAB_NUMBER}
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
$ cd reports/lab${LAB_NUMBER}
$ edit REPORT.md
$ gist REPORT.md
```

## Links

### Unix commands

- [ar](https://en.wikipedia.org/wiki/Ar_(Unix))
- [cat](https://en.wikipedia.org/wiki/Cat_(Unix))
- [cd](https://en.wikipedia.org/wiki/Cd_(command))
- [cp](https://en.wikipedia.org/wiki/Cp_(Unix))
- [cut](https://en.wikipedia.org/wiki/Cut_(Unix))
- [echo](https://en.wikipedia.org/wiki/Echo_(command))
- [env](https://en.wikipedia.org/wiki/Env_(shell))
- [ex](https://en.wikipedia.org/wiki/Ex_(editor))
- [file](https://en.wikipedia.org/wiki/File_(command))
- [find](https://en.wikipedia.org/wiki/Find)
- [ls](https://en.wikipedia.org/wiki/Ls)
- [man](https://en.wikipedia.org/wiki/Man_page)
- [mkdir](https://en.wikipedia.org/wiki/Mkdir)
- [mv](https://en.wikipedia.org/wiki/Mv)
- [nm](https://en.wikipedia.org/wiki/Nm_(Unix))
- [ps](https://en.wikipedia.org/wiki/Ps_(Unix))
- [pwd](https://en.wikipedia.org/wiki/Pwd)
- [rm](https://en.wikipedia.org/wiki/Rm_(Unix))
- [sed](https://en.wikipedia.org/wiki/Sed)
- [touch](https://en.wikipedia.org/wiki/Touch_(Unix))

### Package Managers

- [apt](http://help.ubuntu.ru/wiki/apt) | [dnf](https://en.wikipedia.org/wiki/DNF_(software)) | [yum](https://fedoraproject.org/wiki/Yum/ru)
- [brew](https://brew.sh) | [linuxbrew](http://linuxbrew.sh)
- [npm](https://docs.npmjs.com)

### Software

- [curl](https://www.gitbook.com/book/bagder/everything-curl/details)
- [wget](https://www.gnu.org/software/wget/manual/wget.pdf)
- [clang](https://clang.llvm.org)
- [g++](https://gcc.gnu.org/onlinedocs/gcc-4.0.2/gcc/G_002b_002b-and-GCC.html)
- [make](https://en.wikipedia.org/wiki/Make_(software))
- [open](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/open.1.html)
- [openssl](https://www.openssl.org)
- [nano](https://www.nano-editor.org)
- [tree](https://linux.die.net/man/1/tree)
- [vim](http://www.vim.org)

## Homework - P.S Я делал эту лабу, только почему то отчет не сохранился на гите 😢

1. Скачайте библиотеку *boost* с помощью утилиты **wget**. Адрес для скачивания `https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz`.
```sh
 wget https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz
<details><summary>
--2023-05-28 18:29:34--  https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz
Resolving sourceforge.net (sourceforge.net)... 104.18.11.128, 104.18.10.128, 2606:4700::6812:a80, ...
Connecting to sourceforge.net (sourceforge.net)|104.18.11.128|:443... connected.</summary>
HTTP request sent, awaiting response... 301 Moved Permanently
Location: https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz/ [following]
--2023-05-28 18:29:35--  https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz/
Reusing existing connection to sourceforge.net:443.
HTTP request sent, awaiting response... 301 Moved Permanently
Location: https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz/download [following]
--2023-05-28 18:29:35--  https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz/download
Reusing existing connection to sourceforge.net:443.
HTTP request sent, awaiting response... 302 Found
Location: https://downloads.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz?ts=gAAAAABkc9XQRrdp8fkDxsqN84PHXdYAPHmOeEQdgZUtag-2XDA-a-zOq41jdH_P8Ze-DQ5PHKTfTagoXEiB6-3CmQ_Yff_-yA%3D%3D&use_mirror=deac-ams&r= [following]
--2023-05-28 18:29:35--  https://downloads.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz?ts=gAAAAABkc9XQRrdp8fkDxsqN84PHXdYAPHmOeEQdgZUtag-2XDA-a-zOq41jdH_P8Ze-DQ5PHKTfTagoXEiB6-3CmQ_Yff_-yA%3D%3D&use_mirror=deac-ams&r=
Resolving downloads.sourceforge.net (downloads.sourceforge.net)... 204.68.111.105
Connecting to downloads.sourceforge.net (downloads.sourceforge.net)|204.68.111.105|:443... connected.
HTTP request sent, awaiting response... 302 Found

Location: https://deac-ams.dl.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz [following]
--2023-05-28 18:29:36--  https://deac-ams.dl.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz
Resolving deac-ams.dl.sourceforge.net (deac-ams.dl.sourceforge.net)... 185.34.27.55
Connecting to deac-ams.dl.sourceforge.net (deac-ams.dl.sourceforge.net)|185.34.27.55|:443... connected.
HTTP request sent, awaiting response... 302 Moved Temporarily
Location: https://downloads.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz?download&failedmirror=deac-ams.dl.sourceforge.net [following]
--2023-05-28 18:29:37--  https://downloads.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz?download&failedmirror=deac-ams.dl.sourceforge.net
Connecting to downloads.sourceforge.net (downloads.sourceforge.net)|204.68.111.105|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://nav.dl.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz [following]
--2023-05-28 18:29:38--  https://nav.dl.sourceforge.net/project/boost/boost/1.69.0/boost_1_69_0.tar.gz
Resolving nav.dl.sourceforge.net (nav.dl.sourceforge.net)... 5.154.224.27
Connecting to nav.dl.sourceforge.net (nav.dl.sourceforge.net)|5.154.224.27|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 111710205 (107M) [application/x-gzip]
</details>

Saving to: ‘boost_1_69_0.tar.gz’

boost_1_69_0.tar.gz     100%[===============================>] 106.53M   777KB/s    in 2m 15s  

2023-05-28 18:31:54 (808 KB/s) - ‘boost_1_69_0.tar.gz’ saved [111710205/111710205]
```

```sh
2. Разархивируйте скаченный файл в директорию `~/boost_1_69_0`

```

```sh
3. Подсчитайте количество файлов в директории `~/boost_1_69_0` **не включая** вложенные директории.
  (kali㉿kali)-[~/HECCYLLIujTbmy/workspace]
└─$  tree -a -L 1
.
├── boost_1_69_0
├── boost_1_69_0.tar.gz
├── node
├── projects
├── reports
├── scripts
└── tasks

6 directories, 1 file
```

```sh
4. Подсчитайте количество файлов в директории `~/boost_1_69_0` **включая** вложенные директории.
 tree -a
.
├── boost_1_69_0
│   ├── boost
│   │   ├── accumulators
│   │   │   ├── accumulators_fwd.hpp
│   │   │   ├── accumulators.hpp
│   │   │   ├── framework
│   │   │   │   ├── accumulator_base.hpp
│   │   │   │   ├── accumulator_concept.hpp
│   │   │   │   ├── accumulators
│   │   │   │   │   ├── droppable_accumulator.hpp
│   │   │   │   │   ├── external_accumulator.hpp
│   │   │   │   │   ├── reference_accumulator.hpp
│   │   │   │   │   └── value_accumulator.hpp
│   │   │   │   ├── accumulator_set.hpp
│   │   │   │   ├── depends_on.hpp
│   │   │   │   ├── external.hpp
│   │   │   │   ├── extractor.hpp
│   │   │   │   ├── features.hpp
│   │   │   │   └── parameters
```

```sh
5. Подсчитайте количество заголовочных файлов, файлов с расширением `.cpp`, сколько остальных файлов (не заголовочных и не `.cpp`).
└─$ find -name '*.h' | wc -l
296

─$ find -name '*.cpp' | wc -l
13774

└─$ find '!' -name '*.h' -a '!' -name '*.cpp' | wc -l
52759
```
```sh
6. Найдите полный пусть до файла `any.hpp` внутри библиотеки *boost*.
$  readlink -f any.hpp
/home/kali/HECCYLLIujTbmy/workspace/boost_1_69_0/any.hpp
```
```sh

7. Выведите в консоль все файлы, где упоминается последовательность `boost::asio`.
$ grep -rl 'boost::asio' 

<details><summary>...</summary>
libs/coroutine2/doc/coro.qbk
libs/coroutine2/doc/motivation.qbk
libs/process/example/wait.cpp
libs/process/example/async_io.cpp
libs/process/example/io.cpp
........
doc/html/boost/process/std_in.html
doc/html/boost/process/std_out.html
</details>
```

```sh
8. Скомпилирутйе *boost*. Можно воспользоваться [инструкцией](https://www.boost.org/doc/libs/1_61_0/more/getting_started/unix-variants.html#or-build-custom-binaries) или [ссылкой](https://codeyarns.com/2017/01/24/how-to-build-boost-on-linux/).
cd tools/build/
$ ./boosttrap.sh

Bootstrapping the build engine with toolset gcc... engine/bin.linuxx86_64/b2

Bootstrapping is done. To build and install, run:
./b2 install --prefix=<DIR>
/b2 install --prefix=boost_output
```

```sh
9. Перенесите все скомпилированные на предыдущем шаге статические библиотеки в директорию `~/boost-libs`.
$ mv boost_1_69_0/tools/build/boost_output/ boost-libs

```

```sh
11. Подсчитайте сколько занимает дискового пространства каждый файл в этой директории.
$ du -h
20K     ./example/make
12K     ./example/variant/libs
32K     ./example/variant
24K     ./example/gettext
16K     ./example/time
20K     ./example/generator
20K     ./example/qt/qt4/hello
12K     ./example/qt/qt4/moccable-cpp
16K     ./example/qt/qt4/uic
52K     ./example/qt/qt4
20K     ./example/qt/qt3/hello
12K     ./example/qt/qt3/moccable-cpp
16K     ./example/qt/qt3/uic
52K     ./example/qt/qt3
112K    ./example/qt
16K     ./example/hello
8.0K    ./example/libraries/util/foo/include
20K     ./example/libraries/util/foo
24K     ./example/libraries/util
12K     ./example/libraries/app
44K     ./example/libraries
8.0K    ./example/sass/include
28K     ./example/sass
40K     ./example/customization
12K     ./example/built_tool/tblgen
12K     ./example/built_tool/core
36K     ./example/built_tool
8.0K    ./example/pch/include
8.0K    ./example/pch/source
24K     ./example/pch
20K     ./example/testing
20K     ./example/python_modules
16K     ./example/try_compile
24K     ./example/complex-testing
16K     ./example/asciidoctor
24K     ./example/generate
548K    ./example
56K     ./src/kernel
28K     ./src/engine/boehm_gc/Mac_files
236K    ./src/engine/boehm_gc/include/private
432K    ./src/engine/boehm_gc/include
72K     ./src/engine/boehm_gc/tests
124K    ./src/engine/boehm_gc/cord
476K    ./src/engine/boehm_gc/doc
3.6M    ./src/engine/boehm_gc
28K     ./src/engine/debian
48K     ./src/engine/modules
5.0M    ./src/engine
268K    ./src/util
56K     ./src/contrib
12K     ./src/options
16K     ./src/tools/xsltproc
44K     ./src/tools/generators
208K    ./src/tools/features
120K    ./src/tools/types
8.0K    ./src/tools/doxygen
1.7M    ./src/tools
764K    ./src/build
7.9M    ./src
184K    ./test/qt5
8.0K    ./test/prebuilt/ext/debug
8.0K    ./test/prebuilt/ext/release
40K     ./test/prebuilt/ext
56K     ./test/prebuilt
96K     ./test/qt4
48K     ./test/core-language
12K     ./test/test2
24K     ./test/project-test4/lib
12K     ./test/project-test4/lib2
72K     ./test/project-test4
16K     ./test/project-test3/lib3
12K     ./test/project-test3/lib
12K     ./test/project-test3/lib2/helper
28K     ./test/project-test3/lib2
76K     ./test/project-test3
8.0K    ./test/railsys/program/include
12K     ./test/railsys/program/liba
12K     ./test/railsys/program/main
44K     ./test/railsys/program
12K     ./test/railsys/libx/src
8.0K    ./test/railsys/libx/include
28K     ./test/railsys/libx
76K     ./test/railsys
16K     ./test/boostbook
8.0K    ./test/startup/bootstrap-env
8.0K    ./test/startup/no-bootstrap2
12K     ./test/startup/boost-root/build
20K     ./test/startup/boost-root
8.0K    ./test/startup/bootstrap-explicit
8.0K    ./test/startup/no-bootstrap1/subdir
16K     ./test/startup/no-bootstrap1
8.0K    ./test/startup/no-bootstrap3
8.0K    ./test/startup/bootstrap-implicit
80K     ./test/startup
100K    ./test/toolset-mock/src
120K    ./test/toolset-mock
1.9M    ./test
36K     ./notes
656K    ./doc/html
8.0K    ./doc/src/pygments
8.0K    ./doc/src/hljs/styles
28K     ./doc/src/hljs
416K    ./doc/src
1.1M    ./doc
12M     .


```
```sh
11. Найдите *топ10* самых "тяжёлых".
$ sudo du -a | sort -n -r | head -n 10
11644   .
8024    ./src
5072    ./src/engine
3684    ./src/engine/boehm_gc
1908    ./test
1712    ./src/tools
1084    ./doc
764     ./src/build
736     ./src/engine/boehm_gc/configure
656     ./doc/html


```
Copyright (c) 2015-2021 The ISC Authors
```
