﻿Компиляция BrowserExt в Windows
===============================

Процесс компиляции будет описан для Visual Studio 2012:

1.  Установите библиотеку Qt5 и задайте переменную окружения
    QTDIR, указывающую на директорию с Qt. Например, С:\Qt\qt-5.3.1.

2.  Теперь следует откомпилировать статическую библиотеку browserext-static.
    В директории есть проект для Visual Studio. Откомпилированная библиотека
    будет называться phpbrowser_a.lib (или phpbrowser_a_debug.lib).

3.  Далее следует компилировать php, как это описано 
    [здесь](https://wiki.php.net/internals/windows/stepbystepbuild),
    предварительно скопировав директорию phpextension в ext исходников php
    и phpbrowser_a.lib в директорию с внешними библиотеками для php
    (deps\lib).

