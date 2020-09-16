# svn:global-ignores
```
target

.classpath
.project
.settings

.idea
*.iml

.vscode
.theia

.DS_Store
node_modules

Thunbs.*
```

# idea中配置svn:global-ignores
1. 在工程名上点击右键 -> 选择Subversion -> Edit Properties
2. 添加 name 为 svn:global-ignores，值为上面的项
3. 添加成功后，文件或者文件夹颜色变为黄色
![](images/ignores.jpg)