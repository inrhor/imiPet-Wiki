---
description: 手持喂养
---

# eat.yml

{% hint style="danger" %}
必填
{% endhint %}

## 手持喂养

```text
# 关于手持喂养
eat:
  # 是否启用
  enable: true
  # 格式为 标识符:数值:数量:脚本:脚本的值
  # 标识符仅支持 material name lore
  list:
    - 'material:APPLE:1:addHP:2'
    - 'name:&a卡哇伊:1:addFood:2'
    - 'lore:&a描述:1:command_op:give @player minecraft:apple 1'
```

## 格式

```text
标识符:数值:数量:脚本:脚本的值
```

## 标识符

标识符仅支持

* material
* name
* lore

## 脚本的规范

目前仅支持如下（请严格遵守格式）

```text
- "material:APPLE:XXX:addHP:XX" # XXX和XX必须是整数，即消耗XXX个苹果并恢复XX宠物血量
- "name:&a卡哇伊:1:addFood:2" # 判断物品名称补充宠物2活力
- "lore:&a描述:1:command_op:give @player minecraft:apple 1" # 以OP身份运行命令 支持变量@player
```

{% hint style="warning" %}
根据代码逻辑，依然会先从第一行开始判断

只要其中一行配对成功，就终止下一行判断，开始触发脚本
{% endhint %}

