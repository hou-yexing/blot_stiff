# 螺栓柔度计算器

这是一个基于 VDI 2230 拉伸柔度公式整理的静态网页版计算器。

在线访问：<https://hou-yexing.github.io/blot_stiff/>

## 使用方式

直接打开 `index.html` 即可本地使用，无需安装依赖或启动服务器。公网版本由 GitHub Pages 发布。

## 当前功能

- 标准公制螺栓公称直径和螺距选择
- 自动计算中径 `d2` 和小径 `d3`
- 贯穿连接 / 盲孔连接切换
- 按 VDI 2230 截图公式计算拉伸柔度分项
- 输出拉伸柔度、弯曲柔度参考值和轴向刚度
- 显示连接尺寸参考图、计算分段示意图和公式说明
- 对关键输入进行错误/警告提示

## 计算边界

拉伸柔度按当前已核对的 VDI 2230 截图公式实现。弯曲柔度 `βS` 仍按现有分段 `l/(E·I)` 估算，仅作为参考值。

## 更新和发布

GitHub Pages 发布源为 `main` 分支根目录。修改网页后执行：

```powershell
git add .
git commit -m "Update calculator"
git push
```

推送后，GitHub Pages 会自动更新：<https://hou-yexing.github.io/blot_stiff/>

## 文件

- `index.html`: 网页计算器
- `assets/bolt-connection-diagram.png`: 螺栓连接尺寸示意图
- `螺栓柔度理论计算.pdf`: 原始参考资料
