# CSV数据分析智能工具

这是一个基于Streamlit和LangChain的CSV数据分析工具，使用OpenAI GPT模型来分析和可视化数据。

## 功能特性

- 📊 CSV文件上传和预览
- 🤖 AI驱动的数据分析
- 📈 自动生成图表（条形图、折线图、散点图）
- 💬 自然语言查询数据

## 部署到Streamlit Cloud

1. 将代码推送到GitHub仓库
2. 访问 [Streamlit Cloud](https://streamlit.io/cloud)
3. 连接您的GitHub账户
4. 选择仓库和分支
5. 设置主文件为 `main.py`
6. 点击部署

## 本地运行

```bash
pip install -r requirements.txt
streamlit run main.py
```

## 使用说明

1. 在侧边栏输入您的OpenAI API密钥
2. 上传CSV文件
3. 在文本框中输入您的问题或分析需求
4. 点击"生成回答"获取AI分析结果

## 注意事项

- 需要有效的OpenAI API密钥
- 支持的图表类型：条形图、折线图、散点图
- 文件大小限制：200MB
- ⚠️ **安全提醒**：此应用使用LangChain的pandas agent，可以执行Python代码来分析数据。请确保只上传可信的CSV文件。

## 更新日志

### v1.1 (2025-05-27)
- 修复Python 3.13兼容性问题
- 添加`allow_dangerous_code=True`参数以支持新版LangChain
- 优化错误处理机制
- 简化依赖管理
- 添加缺失的依赖包：`tabulate`、`matplotlib`、`seaborn` 