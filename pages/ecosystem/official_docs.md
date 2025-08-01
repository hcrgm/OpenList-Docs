---
title:
  en: OpenList Docs
  zh-CN: OpenList Docs
categories:
  - ecosystem
  - eco_official
top: 990
---

## What is OpenList Docs { lang="en" }

## OpenList Docs 是什么 { lang="zh-CN" }

### [OpenListTeam/OpenList-Docs](https://github.com/OpenListTeam/OpenList-Docs)

:::en
[OpenListTeam/OpenList-Docs](https://github.com/OpenListTeam/OpenList-Docs) is the official documentation website for OpenList, led by [@cxw620](https://github.com/cxw620) and collaboratively developed with other [main contributors](https://github.com/OpenListTeam/OpenList-Docs/graphs/contributors). Built with Valaxy framework, it provides comprehensive documentation for OpenList, including installation guides, configuration instructions, API references, and ecosystem information. The documentation supports multiple languages and features real-time builds from the GitHub repository.

:::

:::zh-CN
[OpenListTeam/OpenList-Docs](https://github.com/OpenListTeam/OpenList-Docs) 是 OpenList 的官方文档网站，由 [@cxw620](https://github.com/cxw620) 牵头，和其他[主要贡献者](https://github.com/OpenListTeam/OpenList-Docs/graphs/contributors)共同协作完成。基于 Valaxy 框架构建，为 OpenList 提供全面的文档，包括安装指南、配置说明、API 参考和生态系统信息。文档支持多种语言，并基于 GitHub 仓库实时构建。

:::

## How to use OpenList Docs { lang="en" }

## 如何使用 OpenList Docs { lang="zh-CN" }

:::en
You can directly access [doc.oplist.org.cn](https://doc.oplist.org.cn/) to view the documentation.

:::

:::zh-CN
可直接在线访问[doc.oplist.org.cn](https://doc.oplist.org.cn/) 查阅文档。

:::

## Local Development { lang="en" }

### Prerequisites { lang="en" }

:::en

- **Node.js**: Required for running the development environment
- **pnpm**: Recommended package manager
- **Git**: For version control and cloning the repository

1. **Clone the repository**

   ```bash
   git clone https://github.com/OpenListTeam/OpenList-Docs.git
   cd OpenList-Docs
   ```

2. **Install dependencies**

   ```bash
   pnpm install
   ```

3. **Start development server**

   ```bash
   pnpm dev
   ```

4. **Open in browser**

   The documentation site will be available at `http://localhost:4859`

:::

### Building { lang="en" }

:::en
In Windows, you may need to run `npm install -g win-node-env` to solve the `NODE_OPTIONS` environment variable problem.

```bash
# Build static site
pnpm build

# Preview build
pnpm serve
```

:::

## 本地开发 { lang="zh-CN" }

### 环境要求 { lang="zh-CN" }

:::zh-CN

- **Node.js**：运行开发环境所需
- **pnpm**：推荐的包管理器
- **Git**：用于版本控制和克隆仓库

1. **克隆仓库**

   ```bash
   git clone https://github.com/OpenListTeam/OpenList-Docs.git
   cd OpenList-Docs
   ```

2. **安装依赖**

   ```bash
   pnpm install
   ```

3. **启动开发服务器**

   ```bash
   pnpm dev
   ```

4. **在浏览器中打开**

   文档站点将在 `http://localhost:4859` 处可用

:::

### 构建 { lang="zh-CN" }

:::zh-CN
在Windows操作系统下，可能需要运行`npm install -g win-node-env`解决`NODE_OPTIONS`环境变量问题。

```bash
# 构建静态站点
pnpm build

# 预览构建
pnpm serve
```

:::

### Development Tips { lang="en" }

:::en
`:::tip` Markdown Parsing Issues
When writing documentation, please note these important parsing rules:

1. **Language Block Syntax**: For language-specific content blocks, only use one closing `:::` at the end:

   ![Wrong Content Syntax - Light](/img/dev-tip/wrongcontent-light.png#light)
   ![Wrong Content Syntax - Dark](/img/dev-tip/wrongcontent-dark.png#dark)

   The above should be written as:

   ![Correct Content Syntax - Light](/img/dev-tip/correctcontent-light.png#light)
   ![Correct Content Syntax - Dark](/img/dev-tip/correctcontent-dark.png#dark)

   The language will automatically switch when encountering `:::en`.

2. **Title Language Specification**: Titles must use `{ lang="en" }` syntax and cannot use language blocks:

   ![Correct Title Syntax - Light](/img/dev-tip/correcttitle-light.png#light)
   ![Correct Title Syntax - Dark](/img/dev-tip/correcttitle-dark.png#dark)

   Do NOT use:

   ![Wrong Title Syntax - Light](/img/dev-tip/wrongtitle-light.png#light)
   ![Wrong Title Syntax - Dark](/img/dev-tip/wrongtitle-dark.png#dark)

3. **Text Format Convention**: For better readability in plain text environments, please follow the **English first, then Chinese** order when writing bilingual content. This makes it easier to observe and navigate the documentation structure in text editors and version control systems.

4. **Line Break Before Closing `:::`**: Always add a line break before the closing `:::`, especially when using lists (`li`), otherwise formatting may be corrupted:

   ![Wrong Translate End Line Syntax - Light](/img/dev-tip/wrongtranslateendline-light.png#light)
   ![Wrong Translate End Line Syntax - Dark](/img/dev-tip/wrongtranslateendline-dark.png#dark)

   The above should be written as:

   ![Correct Translate End Line Syntax - Light](/img/dev-tip/correcttranslateendline-light.png#light)
   ![Correct Translate End Line Syntax - Dark](/img/dev-tip/correcttranslateendline-dark.png#dark)

5. **Empty Line for Line Breaks**: Content needs an empty line to create line breaks. Without empty lines, content will render as continuous text:

   ![Wrong End Line Syntax - Light](/img/dev-tip/wrongendline-light.png#light)
   ![Wrong End Line Syntax - Dark](/img/dev-tip/wrongendline-dark.png#dark)

   The above should be written as:

   ![Correct End Line Syntax - Light](/img/dev-tip/correctendline-light.png#light)
   ![Correct End Line Syntax - Dark](/img/dev-tip/correctendline-dark.png#dark)

   Note: Lists (`li`) are not affected by this issue.

:::

### 开发提示 { lang="zh-CN" }

:::zh-CN
`:::tip` Markdown 解析问题
在编写文档时，请注意以下重要的解析规则：

1. **语言块语法**：对于特定语言的内容块，结尾只需要一个 `:::`：

   ![错误内容语法 - Light](/img/dev-tip/wrongcontent-light.png#light)
   ![错误内容语法 - Dark](/img/dev-tip/wrongcontent-dark.png#dark)

   上面的写法应该改为：

   ![正确内容语法 - Light](/img/dev-tip/correctcontent-light.png#light)
   ![正确内容语法 - Dark](/img/dev-tip/correctcontent-dark.png#dark)

   当遇到 `:::en` 时语言会自动切换。

2. **标题语言指定**：标题必须使用 `{ lang="en" }` 语法，不能使用语言块：

   ![正确标题语法 - Light](/img/dev-tip/correcttitle-light.png#light)
   ![正确标题语法 - Dark](/img/dev-tip/correcttitle-dark.png#dark)

   不要使用：

   ![错误标题语法 - Light](/img/dev-tip/wrongtitle-light.png#light)
   ![错误标题语法 - Dark](/img/dev-tip/wrongtitle-dark.png#dark)

3. **文本格式约定**：为了方便在纯文本环境下的观察起见，在编写双语内容时请遵循**先英文后中文**的顺序。这样可以更容易在文本编辑器和版本控制系统中观察和导航文档结构。

4. **结束块 `:::` 前换行**：结束块的 `:::` 前最好换行，尤其是使用了列表（`li`），否则会被格式化乱掉：

   ![错误翻译结束行语法 - Light](/img/dev-tip/wrongtranslateendline-light.png#light)
   ![错误翻译结束行语法 - Dark](/img/dev-tip/wrongtranslateendline-dark.png#dark)

   上面的写法应该改为：

   ![正确翻译结束行语法 - Light](/img/dev-tip/correcttranslateendline-light.png#light)
   ![正确翻译结束行语法 - Dark](/img/dev-tip/correcttranslateendline-dark.png#dark)

5. **内容换行需要空行**：内容需要空一行才能换行。没有空行的话，内容会渲染成连续的文本：

   ![错误结束行语法 - Light](/img/dev-tip/wrongendline-light.png#light)
   ![错误结束行语法 - Dark](/img/dev-tip/wrongendline-dark.png#dark)

   上面的写法应该改为：

   ![正确结束行语法 - Light](/img/dev-tip/correctendline-light.png#light)
   ![正确结束行语法 - Dark](/img/dev-tip/correctendline-dark.png#dark)

   注意：列表（`li`）不涉及这个问题。

:::

## License & Legal { lang="en" }

### License { lang="en" }

:::en
This documentation project is licensed under the **[GNU Affero General Public License v3.0 (AGPL-3.0)](https://www.gnu.org/licenses/agpl-3.0.en.html)**.

- **Freedom to Use**: You can use, modify, and distribute this documentation
- **Copyleft**: Any derivative works must also be licensed under AGPL-3.0
- **Network Use**: If you run a modified version on a server, you must provide the source code
- **Attribution**: You must preserve copyright notices and license information

For the full license text, see the [LICENSE](https://github.com/OpenListTeam/OpenList-Docs/blob/main/LICENSE) file.

By contributing to this project, you agree that your contributions will be licensed under the same AGPL-3.0 license.

:::

## 许可证与法律 { lang="zh-CN" }

### 许可证 { lang="zh-CN" }

:::zh-CN
本文档项目采用 **[GNU Affero General Public License v3.0 (AGPL-3.0)](https://www.gnu.org/licenses/agpl-3.0.en.html)** 许可证。

- **使用自由**：您可以使用、修改和分发此文档
- **Copyleft**：任何衍生作品也必须采用 AGPL-3.0 许可证
- **网络使用**：如果您在服务器上运行修改版本，必须提供源代码
- **署名**：您必须保留版权声明和许可证信息

完整的许可证文本请参见 [LICENSE](https://github.com/OpenListTeam/OpenList-Docs/blob/main/LICENSE) 文件。

通过为本项目做出贡献，您同意您的贡献将采用相同的 AGPL-3.0 许可证。

:::
