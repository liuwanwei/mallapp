使用方法：

1，新版本程序（.apk或.ipa文件）发来时，拷贝到packages目录下。
2，如果是.apk文件，修改android.html，将下载地址替换成.apk文件对应的地址。
3，如果是.ipa文件，修改iPhone.html，将下载地址替换成.ipa文件对应的地址。

例如，新版本程序名字是Mall_V1.33.ipa：
1，将它拷贝到packages目录下。
2，打开iPhone.html文件，搜索“iPhone客户端”，找到它所在的<a/>标签，将href修改成“/packages/Mall_V1.33.ipa”。

以上修改完成后，在根目录下，执行：
git add packages/Mall_V1.33.ipa
git add iPhone.html
git commit -m "添加iPhone 1.33版程序" .
git push origin master

