# 项目简介
- 旨在实现一个基于streamlit的最简版的chatbot web客户端
- 参考项目：https://github.com/marshmellow77/streamlit-chatgpt-ui

# 迭代内容
- 修复了客户端在提交时会重复显示文本框和提交按钮的问题
- 调整了页面图标、人物图标、页面标题等内容

# 使用方法
- 配置.env文件中的openai key
- 安装streamlit、streamlit_chat库
- 在文件所在目录下，运行：streamlit run app.py

# 实现逻辑介绍
- 前端页面元素采用streamlit框架生成
- 使用streamlit_chat库来呈现对话内容，通过制定对话者的身份，可以自动的将user内容靠右展示，ai内容靠左展示
- 使用st.session_state保存历史对话信息，刷新页面后st.session_state内容清空
- demo中默认使用gpt-3.5-turbo原生接口，可自行替换为其它LLM接口