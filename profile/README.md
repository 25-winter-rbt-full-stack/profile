# 2025 Winter RBT FullStack Lesson

![RBT FullStack](https://img.shields.io/badge/RBT-FullStack-red)  ![React.js](https://img.shields.io/badge/React.js-1677ff)  ![Nodejs](https://img.shields.io/badge/Node.js-389e0d)  ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-eb2f96)  ![Docker](https://img.shields.io/badge/Docker-003eb3)

![RBT Interview System 01](https://github.com/user-attachments/assets/d232008e-e20d-45da-a08a-4a95ca9820d2)

![RBT Interview System 02](https://github.com/user-attachments/assets/a46bc49d-83cb-404b-bc5e-60c138ffb47a)



## 开发工具

同学们电脑需要准备以下开发工具，自行去官网下载安装即可：

- [VSCode](https://code.visualstudio.com/)
- [Chrome](https://www.google.com/chrome/)
- [Node.js](https://nodejs.org/)

## 新增 .gitignore 文件

在项目根目录下新增 .gitignore 文件，用于忽略一些不必要的文件，比如 `node_modules` 文件夹，`.DS_Store` 文件等。

![image](https://github.com/user-attachments/assets/877bab27-17ec-4f7f-a1b9-4ad643536e4c)

具体步骤如下：

1. 新建 `.gitignore` 文件

2. 在 `.gitignore` 文件中添加以下内容：

```bash
**/node_modules/
.DS_Store
```

## 安装 git 钩子

在提交代码前，需要先安装 git 钩子，确保提交的代码符合规范。具体步骤：

1. 克隆老师仓库到你们本地 `Luffyzh`

```bash
git clone git@github.com:25-winter-rbt-full-stack/Luffyzh.git
```

2. 将根目录文件夹 `git-hooks` 拷贝到你们仓库根目录下

注意，文件夹名字以及内容需要相同。

3. 拷贝完成之后，在项目根目录命令行运行如下命令：

```bash
# 在 Mac 或 Linux 系统中运行
./git-hooks/setup.sh

# 在 Windows 系统中运行
./git-hooks/setup.bat
```

![commit-msg-hooks-01](https://github.com/user-attachments/assets/cd762f56-27a8-4349-8618-64a2a7acfd74)


4. 代码规范验证

运行成功之后，你们提交代码就会遵循严格的规范，具体提交规范含义如下：

| Commit 前缀 | 含义       |
| ----------- | ---------- |
| `feat:`     | 新增功能   |
| `fix:`      | 修复 bug   |
| `to:`       | 未完成提交 |
| `docs:`     | 文档修改   |
| `style:`    | 代码格式化 |
| `refactor:` | 代码重构   |
| `test:`     | 测试       |
| `chore:`    | 其他修改   |

为了验证你是否安装成功，你可以在本地更新一下 README.md 文件，然后提交代码，看看是否符合规范。举例说明如下：

```bash
git add README.md
git commit -m "更新 README.md 文件"
```

这样的提交，不符合规范，因此在控制台会出现如下提示：

![commit-msg-hooks-02](https://github.com/user-attachments/assets/9dac97f4-001c-4785-91ae-6af06d22bdc4)


此时就表示你 git 钩子安装成功了，这也是为了从基础规范同学们的提交，对以后进入大厂工作十分有帮助，是加分项。然后我们因为修改的是 `README.md` 文件，所以使用 `docs:` 前缀，然后提交代码，如下：

```bash
git add README.md
git commit -m "docs: 更新 README.md 文件"
```

提交结果如图所示：

![commit-msg-hooks-03](https://github.com/user-attachments/assets/6c9d3eb5-9005-4a21-bc3f-d764885614e6)


至此，我们整个开发前的 Git 前置准备工作就完成了。

