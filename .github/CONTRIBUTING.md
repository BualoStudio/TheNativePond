# 贡献指南

你好！感谢你有兴趣为 _The Native Pond_ 贡献力量。本指南将帮助你入门。

## 0. 📖 先决条件

在开始贡献前，请确保你已经：

- 阅读本项目的 [README](https://github.com/BualoStudio/TheNativePond/edit/main/README.md) 文件，对本项目有大致了解。
- 仔细阅读并遵守 [LICENSE](https://github.com/BualoStudio/TheNativePond/blob/main/LICENSE)。
- 仔细阅读并遵守 [行为准则](https://github.com/BualoStudio/TheNativePond/blob/main/.github/CODE_OF_CONDUCT.md)。
- 阅读 [TheNativePond FlatbreadList](https://github.com/BualoStudio/TheNativePond/blob/main/docs/game/FlatbreadList.md) 文件。
- 阅读 [TheNativePond Values](https://github.com/BualoStudio/TheNativePond/blob/main/docs/game/Values-zh_CN.md) 文件，不要贡献违背价值观的内容。
- 准备 TurboWarp 编辑器：[TurboWarp Desktop](https://desktop.turbowarp.org/) （推荐） 或 [TurboWarp Webapp](turbowarp.org/editor)。
- 搜索已有的 [Issue](https://github.com/BualoStudio/TheNativePond/issues) 和 [Pull Request](https://github.com/BualoStudio/TheNativePond/pulls)，避免重复工作。


## 1. 🛠️ Fork 本项目

1. 点击 [TheNativePond](https://github.com/BualoStudio/TheNativePond) 页面右上角的 **Fork** 按钮。
2. 修改完基本信息（如果有需要）后，点击下面的 **Create fork** 按钮。

## 2. 📂 选择你要贡献的方向

由于 _The Native Pond_ 是一个多媒体的游戏项目，所以你只需选择你要贡献的方向即可。

### 💻 代码

#### TurboWarp 工程文件（.sb3）

> [!WARNING]
> 
> 由于 TurboWarp 工程文件属于二进制文件，不适合进行代码审查，因此请勿直接向工程文件提交 Pull Request。一般情况下，我们不接受对工程文件的 Pull Request。

如果确实需要修改工程文件，请：

- 提交包含完整修改方案的 Issue
- 或设计对应的 JavaScript 自定义扩展
- 或 [联系我们](mailto:thenativepond@gmail.com)

如果我们认为你的申请是合理且有必要的，我们可能会邀请你共同修改工程文件。

##### 我们不接受：

- 未经讨论提交对工程文件的 Pull Request
- 修改 Scratch Blocks
- 修改 TurboWarp 内核
- 提交未经讨论的大规模重构

#### 自定义扩展（.js）

由于 TurboWarp 提供的功能较为有限，无法满足 _The Native Pond_ 的开发需要，所以我们会使用自定义扩展以补充缺失的功能。

##### 允许贡献：

- 带有新功能的自定义扩展
- 对已有自定义扩展的 Bug 修复
- 对已有自定义扩展的性能优化
- 对已有自定义扩展的 API 改进
- 对已有自定义扩展的注释完善和文档补充

##### 我们不接受：

- 修改 Scratch Blocks
- 修改 TurboWarp 内核
- 提交未经讨论的大规模重构

##### 在编写 JavaScript 自定义扩展时，请：

- 使用现代的 JavaScript
- 保证代码可读性和风格统一
- 使用有意义的变量名称（请遵守 [命名规范](https://github.com/BualoStudio/Icelet/wiki/Naming-Conventions)）
- 避免重复代码
- 添加必要的注释
- 删除调试代码
- 不提交压缩后的代码

##### 在提交贡献前，请再次确认：

- 能够正常运行
- 无 Console Error
- 不影响其它扩展
- 已完成基本测试

### 🖌️ 美术素材

> [!NOTE]
> 
> 我们强烈建议你使用 **SVG** 格式的美术素材。一般情况下，我们不接受其他图片格式的 Pull Request。

允许贡献：

- UI 图标
- 游戏地图
- 物品贴图
- 插图（特别的，插图可以使用其他图片格式）
- 其他矢量素材

在贡献美术资产时，请：

- 使用 SVG 格式的矢量图（插图除外）
- 确保该素材可编辑
- 尽量减少节点的数量
- 请遵守 [命名规范](https://github.com/BualoStudio/Icelet/wiki/Naming-Conventions)
- 保持统一的设计风格（详见 [TheNativePond 美术设计规范]()）

### 🪗 音乐&音效素材

允许贡献：

- 背景音乐
- 控件（交互）音效
- 提示音
- 环境音

在贡献音乐&音效素材时，请：

- 保持适中的音量（与其他音频文件音量一致即可）
- 尽量避免削波
- 请确保你拥有对应资源的版权

### 🌐 本地化

我们正在寻找能够帮助将 _The Native Pond_ 翻译成简体中文以外其他语言的人。如果你对此感兴趣，请继续阅读。

成为翻译者的要求：

- 你必须**精通**简体中文。
- 例如，如果你能看懂 Bilibili 上的简体中文视频，那么你的简体中文水平就很高。如果你需要借助翻译才能理解句子，那么你的简体中文水平就不高。
- 你必须是**目标**语言的母语人士。（如果你不是母语人士，但认为自己的语言水平足够流利，也可以申请加入。请记住，参加一些语言课程并不能让您达到流利的程度。如果你不会把智能手机的系统语言改成目标语言，那就说明你的语言水平还不够！）

允许贡献：

- 新语言支持
- 已有的语言的错误修正

在贡献本地化翻译时，请：

- 

我们希望 _The Native Pond_ 能被全球玩家体验。如果你想帮助将游戏翻译成你的语言：

1. 找到语言文件（位于 `/lang/` 目录）。
2. 添加或更新翻译。

## 🤝 参与共建

_The Native Pond_ 不仅仅是我们的作品；我们希望它能成为所有疲惫玩家的“精神加油站”。无论你是否了解游戏开发或代码，你都可以为这个小池塘做出贡献！

我们非常欢迎以下形式的 Issue：

### 1. 💡 新内容建议

> [!IMPORTANT]
> 
> 在提交新内容建议之前，请先阅读 [本水塘大饼清单](https://github.com/BualoStudio/TheNativePond/blob/main/docs/game/FlatbreadList.md) 和 [本水塘价值观](https://github.com/BualoStudio/TheNativePond/blob/main/docs/game/Values.md)！

1. **记忆碎片投稿**：为游戏撰写感人的文案，或分享一篇带有时代感的怀旧短文。
2. **家乡食谱贡献**：设计一个全新的食谱（例如如何制作一碗地道的热干面），并分解其制作步骤。

> [!TIP]
> 
> 想要为 _The Native Pond_ 制作优秀的衍生修改版本或 MOD？请参考 _[The Native Pond 技术文档](https://github.com/BualoStudio/TheNativePond/tree/main/TechnicalDocumentation)_ 和 _[Icelet 开发指南](https://github.com/BualoStudio/Icelet/wiki)_，并遵守 [LICENSE](https://github.com/BualoStudio/TheNativePond/blob/main/LICENSE) 文件。

### 2. 🐛 现有问题

1. 报告游戏在特定情况下触发的问题、缺陷和错误。
2. 为当前存在的问题、缺陷和错误提供解决方案。

> [!NOTE]
> 
> 由于 TurboWarp 的单源文件限制，请勿直接向源文件提交 Pull Request。但你可以将错误提交到 [Issue](https://github.com/BualoStudio/TheNativePond/issues)。

## 3. 📡 提交

像往常那样，将你的贡献提交到你的 fork 仓库。

## 4. 🔗 创建 Pull Request

导航到 [TheNativePond](https://github.com/BualoStudio/TheNativePond) 页面，点击 **Pull requests** 选项卡，然后点击 **New pull request** 按钮，点击 **Compare across forks** 链接，选择你的 fork 仓库。

审查更改，然后点击 **Create pull request** 按钮。

## 5. 🎉 哇哦！你做到了！

恭喜你！你完成了对本项目的贡献。现在你可以等待我们审阅你的拉取请求。
