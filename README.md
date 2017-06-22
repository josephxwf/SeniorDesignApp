You can download the application or source code: </br>
     1. myapp.app.zip is the mac version application for mac user.</br>
     2. myappInstaller.exe is the installer for windows user.</br>
     3. The source code only contains an example of Threshold. I didn't include other functionalities or the OpenGL</br> version code in it.

# setup

For Windows:
IP library is compile with 64-bit VS2013.
1) You need to get 64-bit VS2013 and  download Qt 5.5.1 for Windows 64-bit .
(http://download.qt.io/official_releases/qt/5.5/5.5.1/qt-opensource-windows-x86-msvc2013_64-5.5.1.exe)
2) Add "C:\Qt\Qt5.5.1\5.5\msvc2013_64\bin" to your system or user PATH.
3) Open a terminal or Windows shell in qip directory.
4) Type: qmake -tp vc qip.pro
5) Then open qip.vcxproj with Visual studio to compile/debug your code.


For Mac:
1) Download Qt 5.5.1 for OS X (679 MB) .
2) By default, it installs in the user home directory. 
Add ~/Qt5.5.1\5.5\clang_64\bin to your system PATH.
3) Make sure qmake is running from the above. (type: which qmake).
4) Open a terminal in qip directory.
5) Type:> qmake -spec macx-clang qip.pro
6)          > make

You can use xcode. First install the latest xcode(7.3) from Apple developer website.
5) Type:> qmake -spec macx-xcode qip.pro
6) open qip.xcodeproj
