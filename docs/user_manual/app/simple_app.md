# 简单配置应用

!!! Abstract ""
    点击【创建应用】，输入应用名称以及应用描述，选择【简易配置】，点击【创建】，进入简易配置应用设置页面。

![选择应用类型](../../img/app/selectAppType.png)

!!! Abstract ""
    左侧为应用信息，右侧为调试预览界面。   

    * 应用名称：提问时对话框的标题和名字。
    * 应用描述：对应用场景及用途的简要描述。
    * AI模型：可选择在【系统设置】-【模型管理】中添加的大语言模型，也可直接添加。
    * 角色设定：通过给模型指定一个特定的角色或身份，来指导模型的输出更加符合特定的场景或任务需求。
    * 提示词：系统默认有智能知识库的提示词，用户可以自定义通过调整提示词内容，可以引导大模型聊天方向，该提示词会被固定在上下文的开头。可以使用变量，例如：{data} 是引用知识库中已知信息，{question}是用户提出的问题。目前可针对是否引用知识库设置不同的提示词。
    * 历史聊天记录：大模型提交当前会话中最后 N 条对话内容，否则仅向大模型提交当前问题。
    * 关联知识库：用户提问优先在关联的知识库中检索分段，引用分段生成提示词发送给大模型进行询问。若未关联知识库或未匹配到分段内容，则默认将用户问题发送给大模型进行询问。知识库可设置检索方式、知识库的相似度，引用分段数 Top-N 和最大引用字符数、无引用知识库分段时的回答策略以及是否进行问题优化等。
    * 开场白：打开对话时，系统弹出的默认引导说明。支持 Markdown 格式，[-]后的内容为快捷问题，一行一个。
    * 语音输入：在语音输入完成后会转化为文字后再发送提问，需要语音识别模型的支持。
    * 语音播放：将大模型生成的回答内容转换为语音进行播放，需要语音合成模型的支持。


!!! Abstract ""   
    应用信息设置完成后，可在右侧调试预览中进行提问测试，调试过程不计入对话日志。</br>
    点击【保存并发布】后，应用设置才生效。

![应用设置](../../img/app/app_setting.png)

