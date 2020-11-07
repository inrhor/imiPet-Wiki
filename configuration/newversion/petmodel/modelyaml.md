---
description: 第一步：快速了解结构
---

# 模型配置目录结构

我觉得旧版本的模型配置太麻烦了，查找不容易，容易写错

于是决定在imiPet-4.0.0完成模型配置全新目录结构

当然，旧版本模型配置也是可以注册的，但有些功能无法使用，而且在未来可能会移除

{% hint style="success" %}
建议大家快速将旧版配置转化为新版配置
{% endhint %}

{% hint style="info" %}
接下来我们第一步是快速了解结构
{% endhint %}

```text
models  # 存放模型配置文件
  xxx  # 随便命名
    ├─model.yml  # 模型ID和普通动态动作 [必填]
    ├─pack.yml  # 自动生成纹理资源包 [选填]
    ├─pack  # 放置关于纹理资源包 [如果pack.yml启用自动生成纹理资源包]
    ├─skill.yml  # 模型技能动态动作 [选填]
    ├─basis.yml  # 基本值 [必填]
    ├─formula.yml  # 相关公式 [必填]
    ├─feature.yml  # 其它功能 [必填]
    ├─interaction.yml  # 交互式信息 [必填]
    ├─eat.yml  # 手持喂养 [必填]
    ├─evolution.yml  # 关于进化 [必填]
    ├─attribute.yml  # 其它外部属性 [选填]
    ├─buff.yml  # 加成反应 [选填]
    └─vexview.yml  # 关于VexView界面 [选填]
```

{% hint style="warning" %}
必填是必须创建的文件

必须同名文件名称，大小写必须符合

选填指可以不创建的文件，可以不填写
{% endhint %}

{% hint style="info" %}
4.1.3+版本后内置了示例配置
{% endhint %}

请以ZIP方式打开imiPet插件

![](../../../.gitbook/assets/111.png)

