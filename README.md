﻿# Android之Mina集成，自定义解码，断包、粘包处理


---

---
##自定义消息格式
- 每条消息的格式为：**消息头（一个int类型：表示消息体的长度、一个short类型：表示事件号）+消息体（为字符串，可以假定认为是json字符串）**。