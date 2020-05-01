# OpenTSDB 


```
cp ../OpenTSDB/README.md .
cp -r ../OpenTSDB/HuGo/themes/book ./HuGo/themes
cp -r ../OpenTSDB/HuGo/config.* ./HuGo
cp -r ../OpenTSDB/HuGo/assets ./HuGo
sed -i '' 's/OpenTSDB/_NewProject_/g' `grep OpenTSDB --include=\*.{md,html,xml,yaml,toml} -rl .`

git config user.email ykb553@163.com
git config -l | grep user

# 更新主题模块
# git submodule add -f https://github.com/o-fork/hugo-book HuGo/themes/book
$ git submodule init
$ git submodule update

# 本地服务
hugo server -s HuGo/

# 生成静态站点
hugo -s HuGo/
```
