# 生成 versions/baseline.json

手动先创建空目录结构和基准文件
```
mkdir -p versions
echo '{"default": {}}' > versions/baseline.json

# 生成版本数据库  需要显示指定目录
/g/vcpkg/vcpkg.exe x-add-version --all --overwrite-version --x-builtin-ports-root=./ports --x-builtin-registry-versions-dir=./versions
```