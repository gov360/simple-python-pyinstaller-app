#simple-python-pyinstaller-app

这个存储库是为了
[使用PyInstaller构建Python应用程序]（https://jenkins.io/doc/tutorials/build-a-python-app-with-pyinstaller/）
[Jenkins用户文档]（https://jenkins.io/doc/）中的教程。

存储库包含一个简单的Python应用程序，它是一个命令行工具“add2vals”，它输出两个值的相加。如果至少有一个
values是一个字符串，“add2vals”将这两个值视为字符串而是
连接值。 “calc”库中的“add2”函数（其中
“add2vals”导入）伴随着一组单元测试。这些是使用pytest测试的，以检查此功能是否按预期工作并保存结果
到JUnit XML报告。

通过PyInstaller交付“add2vals”工具将此工具转换为
Linux的独立可执行文件，可以通过Jenkins下载
并在没有Python的Linux机器上的命令行执行。

`jenkins`目录包含`Jenkinsfile`的示例（即Pipeline）
你将在本教程中创建自己。
