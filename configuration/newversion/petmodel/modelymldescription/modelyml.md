---
description: 模型ID和普通动态动作
---

# model.yml

{% hint style="danger" %}
必填
{% endhint %}

## 示例

```text
# 模型的唯一ID
modelId: "test"

# 关于ModelEngine模型引擎插件
modelEngine:
  use: false
  animation:
    # 攻击状态
    attack:
      # 到多少tick使动画重新开始
      retime: 100
      # 攻击动作时长，tick
      stopTime: 100
    # Gui模型显示
    gui:
      # 物品名称
      itemName: "§8"
      # 模型数据，仅支持1.14+
      customModelData: 10000
      # 物品材料，无则默认钻石锄子
      material: "DIAMOND_HOE"

# 关于模型与动态模型
# 若不启用ModelEngine模型引擎插件时
animation:
  # 关于模型位置
  location:
    # 显示高度
    h: 1
  # 空闲状态
  idle:
    # 物品名称
    itemName: "§8"
    # 模型数据，仅支持1.14+
    customModelData: 10000
    # 物品材料，无则默认钻石锄子
    material: "DIAMOND_HOE"
  # 行走状态
  walk:
    itemName: "§a"
    customModelData: 10001
    material: "DIAMOND_HOE"
  # 攻击状态
  attack:
    itemName: "§5"
    customModelData: 10002
    material: "DIAMOND_HOE"
    # 显示攻击动作动态时长，秒
    time: 5
    
# 其它
entity:
  # 真实实体是否可见，默认不可见
  visible: false
```

## 模型ID

{% hint style="danger" %}
必须是唯一的

不忽略大小写

不建议添加任何符号，诸如 ~ : - ! 等
{% endhint %}

```text
modelId: "test"
```

## 关于ModelEngine

{% hint style="warning" %}
需要前置插件ModelEngine
{% endhint %}

使用ModelEngine，你就可以使用基岩动画模型

## 关于模型与动态模型

{% hint style="warning" %}
只适用于非ModelEngine，即Java模型
{% endhint %}

{% hint style="info" %}
只是普通动态动作：空闲，行走，攻击

而技能动态动作在 skill.yml 中设置
{% endhint %}

```text
# 关于模型与动态模型
animation:
  # 关于模型位置
  location:
    # 显示高度
    h: 1
  # 空闲状态
  idle:
    # 物品名称
    # Item Name
    itemName: "§8"
    # 模型数据，仅支持1.14+
    customModelData: 10000
  # 行走状态
  walk:
    itemName: "§a"
    customModelData: 10001
  # 攻击状态
  attack:
    itemName: "§5"
    customModelData: 10002
    # 显示攻击动作动态时长，秒
    time: 5
```

