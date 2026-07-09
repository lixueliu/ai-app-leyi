# AI 小游戏乐园

这是一个无需构建的静态入口页项目，用来收纳小朋友和 AI 一起生成的小游戏。

## 当前结构

每个小游戏都放在根目录的独立文件夹里，文件夹内只有一个入口文件：

```text
game-folder/
  index.html
```

首页会使用 `game-folder/` 作为链接，因此访问路径里不会显示 `index.html`。

## 添加一个小游戏

1. 新建文件夹，例如 `star-run/`。
2. 在文件夹里放唯一入口文件 `star-run/index.html`。
3. 打开根目录的 `index.html`，在 `games` 数组里加入：

```js
{
  name: "星星接力",
  folder: "star-run",
  creator: "乐乐",
  type: "闯关",
  description: "一个收集星星的小冒险。",
  color: "#bde7ff",
}
```

根目录的 `index.html` 会把它渲染成入口卡片。
