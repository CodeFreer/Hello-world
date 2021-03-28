# GitHub Hello World

10分钟阅读

**Hello World** 项目是计算机编程中的一个历史悠久的传统。它是一项简单的练习，让你在学习新东西的过程中入门。让我们开始学习 GitHub!

**你将会学习到如何:**

- 创建以及使用一个库
- 开始并管理一个新的分支
- 对一个文件进行更改，并把它们按提交(commits)的方式推送(push)到 GitHub
- 打开并合并拉取(pull)请求

## 什么是 GitHub?

GitHub 是一个用于版本控制和协作的代码托管平台。它让你和来自任何地方的其它人在项目上一起努力。

这个教程将教导你一些 GitHub 的基本概念，例如*库(repositories)*, *分支(branches)*, *提交(commits)* 以及*拉取请求(Pull Requests)*。你将创建你自己的 Hello World 库并学习 GitHub’ 的拉取请求的工作流程，一种用于创建和审查代码的流行方式。

#### 无需进行代码

要完成本教程，你需要一个 [GitHub.com 账户](http://github.com/) 和互联网访问方式。你不需要知道如何进行编码、使用命令行或安装 Git (GitHub 所构建在的版本控制软件)。

> **提示:** 在一个单独的浏览器窗口(或标签页)中打开本指南，以便你在完成本教程中的步骤时能够查看它。

## 第 1 步. 创建一个库(Repository)

一个 **库(repository)** 通常用于组织一个单一项目。库可以包含文件夹、文件、图像、视频、电子表格和数据集 – 你的项目所需要的任何内容。 我们建议你包含一个 *README*，或者一个带有有关你的项目的信息的文件。 GitHub 让你在创建你的新库的同时轻松添加一个这样的文件。 *它还提供了一些常见的选项，譬如许可文件。*

你的 `hello-world` 库可以是一个存放你的创意、资源，甚至是分享以及和其它人讨论的地方。

### 要创建一个新库

1. 在右上角，在你的头像或标识图标旁边，点击，然后选择 **New repository(新建库)**。
2. 命名你的库为 `hello-world`。
3. 编写简短的说明。
4. 选择 **Initialize this repository with a README(使用一个 README 来初始化这个库)**。

![new-repo-form](https://guides.github.com/activities/hello-world/create-new-repo.png)

点击 **Create repository(创建库)**。

## 第 2 步. 创建一个分支(Branch)

**Branching(分支)** 是一次在一个库的不同版本上工作的方法。

默认情况下，你的库拥有一个名为 `main` 的分支，它被认为是最明确(definitive)的分支。在提交到 `main` 前，我们会使用多个分支来进行实验和进行编辑。

当你在`main` 分支上创建一个分支时，你就是对`main` 当时的情况建立一个拷贝，或者一个快照。如果当你正在努力于你的分支上时其他人对`main`分支进行了更改的话，你可以在那些更新中拉取/提取(pull)。

这个图解展示:

- `main` 分支
- 一个称为`feature` 的分支(因为我们正在这个分支上进行 ‘feature work(功能性的工作)’)
- `feature` 在它被合并入`main` 前所采取的过程(journey)

![a branch](https://guides.github.com/activities/hello-world/branching.png)

你有没有保存过一个文件的不同版本? 像这样:

- `story.txt`
- `story-joe-edit.txt`
- `story-joe-edit-reviewed.txt`

分支在 GitHub 库中就是实现类似的目标。

在 GitHub 中，我们的开发者、编写人员以及设计人员使用多个分支来使得错误修复和特性工作保持和我们的 `main` (生产)分支分离开。当准备好一次更改时，他们就合并他们的分支到 `main` 中。

### 创建一个新分支

1. 转到你的新库 `hello-world`。
2. 点击位于文件列表顶部的下拉按钮，该按钮称为 **branch: main**。
3. 键入一个分支名称，如 `readme-edits` 到新的分支文本框中。
4. 然后选择出现在下面的**Create branch(创建分支): readme-edits from \`main\`** 框或点击键盘上的“Enter”。

![branch gif](https://guides.github.com/activities/hello-world/readme-edits.gif)

现在你就拥有两个分支， `main` 和 `readme-edits` 了(当前你在后一个分支中)。它们看起来完全一样，但是很快就不一样了! 下一步我们将会添加我们的更改到新分支。

## 第 3 步. 进行更改并提交更改(Make and commit changes)

好极了!现在你是在你的 `readme-edits` 分支的代码视图中，这个分支是 `main` 的一个副本。让我们进行一些编辑。

在 GitHub 上，保存更改被称为 *commits(提交或者记录某修改，重点在于记录)*。每次的提交记录都有一个相关的*commit message(提交消息)*，它是解释为何做出某个特定更改的描述说明。提交消息捕捉你的更改的历史，以便其它贡献人员可以明白你已经完成了什么以及为何这样做。

#### 进行并提交更改

1. 点击 `README.md` 文件。
2. 点击文件视图右上角的铅笔图标进行编辑。
3. 在出现的编辑器中，随便写一些有关你自己的东西。
4. 编写一条描述你的更改的提交消息。
5. 点击**Commit changes(提交更改)** 按钮。

![commit](https://guides.github.com/activities/hello-world/commit.png)

这些更改将只会在你的`readme-edits`分支上的 README 文件上发生，所以现在这个分支包含了和 `main` 不一样的内容。

## 第 4 步. 打开一个拉取请求(Pull Request)

编辑得不错!现在你既然已经在 `main` 外的一个分支中做出了更改，就可以打开一个 *pull request(拉取请求)*。

Pull Requests 是 GitHub 上协助的核心部分。当你开启一个*拉取请求*时，你就是在提出你的更改并要求某人审查并在你的贡献中提取(拉取)，以及合并它们到他们的分支中。拉取请求显示*diffs(差异)*，或者来自两个分支的内容及其中的差异。各种变化，增、删内容会以红、绿显示。

一旦你进行一次提交，你就可以开启一次拉取请求并开始一次讨论，即使在代码完成前。

通过在你的拉取请求消息中使用 GitHub 的 [@提及系统(mention system)](https://help.github.com/articles/about-writing-and-formatting-on-github/#text-formatting-toolbar)，你可以要求来自特定的人或团队的反馈，无论它正在大厅散步还是在10个时区之外。

你甚至可以在你自己的库中开启拉取请求并自己来合并它们。这是在着力于更大的项目之前，一个学习 GitHub 流程的好办法。

#### 开启对 README 的更改的一次拉取请求

*点击下面的图像得到一个较大的版本*

| 步骤                                                                                | 截屏                                                                                                                                               |
| --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| 点击 **Pull Request (拉取请求)** 选项卡，然后在”拉取请求“页面中，点击绿色的 **New pull request(新拉取请求)** 按钮。 | [![pr-tab](https://guides.github.com/activities/hello-world/pr-tab.gif)](https://guides.github.com/activities/hello-world/pr-tab.gif)            |
| 在下面的 **Example Comparisons(示例比较)** 框，选择你做出的分支，`readme-edits`，和`main` (原本)。        | [![branch](https://guides.github.com/activities/hello-world/pick-branch.png)](https://guides.github.com/activities/hello-world/pick-branch.png)  |
| 在”比较“页面上的查看差异(diffs)中你的更改，确保它们就是你要提交的内容。                                          | [![diff](https://guides.github.com/activities/hello-world/diff.png)](https://guides.github.com/activities/hello-world/diff.png)                  |
| 当你满意这些就是你想递交(submit)的更改时，点击大的绿色 **Create Pull Request(创建拉取请求)** 按钮。               | [![create-pull](https://guides.github.com/activities/hello-world/create-pr.png)](https://guides.github.com/activities/hello-world/create-pr.png) |
| 赋予你的拉取请求一个标题并写下你的更改的一个简单说明。                                                       | [![pr-form](https://guides.github.com/activities/hello-world/pr-form.png)](https://guides.github.com/activities/hello-world/pr-form.png)         |

当你完成了你的消息，点击**Create pull request(创建拉取请求)**!

---

> **提示**: 你可以使用 [emoji](https://help.github.com/articles/basic-writing-and-formatting-syntax/#using-emoji) 以及 [拖放图像和 gifs](https://help.github.com/articles/file-attachments-on-issues-and-pull-requests/) 到注释上并拉取请求。

## 第 5 步. 合并你的拉取请求

在这个最后一步中，是时候把你的所有更改放到一起 – 合并你的 `readme-edits` 分支到 `main` 分支中。

1. 点击绿色的 **Merge pull request(合并拉取请求)** 按钮以合并多个更改到 `main` 中。
2. 点击**Confirm merge(确认合并)**.
3. 继续前进并删除该分支，因为它的更改已被吸收，使用在紫色框中的 **Delete branch(删除分支)** 按钮。

![merge](https://guides.github.com/activities/hello-world/merge-button.png) ![delete](https://guides.github.com/activities/hello-world/delete-button.png)

### 干杯!

通过完成这个教程，你已经学到在 GitHub 上创建一个项目并进行一次拉取请求!

这里是你在本教程中实现的内容:

- 创建一个开源的库
- 开始并管理一个新的分支
- 更改一个文件并提交那些更改到 GitHub
- 打开并合并一次拉取请求

查看一下你的 GitHub profile(配置档)，你将会看到你的新[贡献方格](https://help.github.com/articles/viewing-contributions)!

要进一步了解有关拉取请求的威力，我们建议阅读 [GitHub 流程指南](http://guides.github.com/overviews/flow/)。你还可以访问 [GitHub Explore](http://github.com/explore) 并参与一个开源项目。

---

> **提示**: 查看我们的其它[指南](http://guides.github.com/), [YouTube 频道](http://youtube.com/githubguides) 和 [点播培训](https://services.github.com/on-demand/) 了解更多关于如何开始使用 GitHub 的信息。

本文英文原版最后更新于 2020.7.24，翻译于 2021.3.29

[GitHub](https://github.com/) 是构建和发布软件的。 
为开源和私有项目提供强大的协作、代码审查和代码管理。
