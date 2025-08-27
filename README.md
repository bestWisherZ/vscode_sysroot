# 在远程服务器上执行
mkdir -p ~/.vscode-server/sysroot
# 假设压缩包已上传到用户主目录 ~
tar zxvf ~/vscode-sysroot-x86_64-linux-gnu.tgz -C ~/.vscode-server/sysroot --strip-components=1
# 在远程服务器上执行
echo 'source ~/.vscode-server/sysroot.sh' >> ~/.bashrc
# 在远程服务器上执行
source ~/.bashrc\

重新打开 VS Code 并链接到远程服务器，不出意外应该已经好了。
