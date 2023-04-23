Semantic Kernel C# 笔记本
当前文件夹包含几个 C# Jupyter 笔记本，展示了如何使用 Semantic Kernel 开始工作。笔记本按照复杂度递增的顺序进行组织。

要运行这些笔记本，我们建议按照以下步骤操作：

安装 .NET 7
安装 Visual Studio Code (VS Code)
启动 VS Code 并安装“Polyglot”扩展。要求的最小版本为：v1.0.4102020（2022年2月）。
以上步骤应该足够了，现在您可以在 VS Code 中打开所有的 C# 笔记本。

VS Code 截图示例：

image

设置 OpenAI API 密钥
要开始使用这些笔记本，请确保将适当的 API 密钥添加到 config/settings.json 中。

您可以手动创建文件，也可以运行设置笔记本。

对于 Azure OpenAI：

json
Copy code
{
  "type": "azure",
  "model": "...", // Azure OpenAI 部署名称
  "endpoint": "...", // Azure OpenAI 终结点
  "apikey": "..." // Azure OpenAI 密钥
}
对于 OpenAI：

json
Copy code
{
  "type": "openai",
  "model": "text-davinci-003", // OpenAI 模型名称
  "apikey": "...", // OpenAI API 密钥
  "org": "" // 仅适用于拥有多个组织的 OpenAI 账户
}
如果您需要 Azure OpenAI 密钥，请单击此处。
如果您需要 OpenAI 密钥，请单击此处。

主题
在开始之前，请确保配置了 config/settings.json，请参见前一节。

要快速开始，请查看入门笔记本。

加载和配置 Semantic Kernel
从文件运行 AI 提示
在运行时创建语义函数（即内联函数）
使用上下文变量构建聊天体验
创建和执行计划
使用嵌入构建内存
