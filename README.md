**经验集中在 LLM 应用、AIGC 性能优化、爬虫、广告投放、风控**

#### 构建

- Comfyui-qwself - ComfyUI 生产环境工具：增加缓存并提前初始化 ultralytics，以优化生图速度。
- RiskModel - 风控模型：1. 文本风控模型 2. 用户风控模型 3. AI 陪聊人物设定。
- lstm-video-title-classification - 基于 LSTM 的标题分类模型。
- pyMicroHarness - 轻量级测试脚手架，便于理解底层原理；支持飞书。
- MicroPyRpc - 极简 RPC 服务；用于 ComfyUI 任务场景的 side service，处理频繁 import/tool 代理的情况。

#### 贡献于

- stable-diffusion-webui - 修复 `checkpoints_loaded` 中 `model.load_state_dict` 在字典值为空时的问题（#13535）。通过将 `orderdict` 用作 LRU 缓存进行优化/修复（#13313）。
