---
description: 模型技能动态动作
---

# skill.yml

{% hint style="warning" %}
选填
{% endhint %}

## 示例

```text
skillModel:
  # 技能ID，必须是已注册的技能ID，可忽略大小写
  MechaEngineering:
    # 技能的译名
    name: "&f机甲工程"
    animation:
      # 动态ID
      # 宠物模型动态动作从第一个动态ID开始运行
      a:
        # 是否启用ModelEngine模型引擎插件
        # 播放动画要求名称为 skill-技能ID-动态ID 即skill-MechaEngineering-a
        useModelEngine: false
        # 物品名称
        # Item Name
        itemName: "§8§a"
        # 模型数据，仅支持1.14+
        customModelData: 10000
        material: "PLAYER_HEAD"
        # 显示时长，秒，小于或等于0则无该动态
        time: 10
        # 下一个动态ID，无或留空则取消技能动态动作
        nextAnimationID: "ha"
      ha:
        itemName: "§8§9"
        customModelData: 10001
        material: "PLAYER_HEAD"
        time: 5
    # 该技能冷却时长，秒，小于或等于0则无冷却
    coolDown: 60
    # 释放技能过程是否可以移动
    canMove: false
    # 触发条件，满足所有条件即可触发
    #    food:消耗所需活力值
    #    permission:权限
    triggerList:
      - "food:10"
  # 可以添加更多已注册的技能ID
  #xxx:
```

## 技能ID

指在 skills 文件夹中已成功创建并注册的技能ID

[点击查看技能相关内容](../../skillmodel/)

## 技能的译名

```text
skillModel:
  技能ID:
    # 技能的译名
    name: "&f机甲工程"
```

## 动态ID

{% hint style="info" %}
宠物模型动态动作从第一个动态ID开始运行
{% endhint %}

对于动态ID没有严格要求

## 动态ID的物品

{% hint style="info" %}
目的是实现宠物模型技能动态动作

原理是根据 释放技能 而赋予指定的动态动作，其中动态动作主要由动态模型材质实现的
{% endhint %}

```text
    animation:
      # 动态ID
      # 宠物模型动态动作从第一个动态ID开始运行
      a:
        # 物品名称
        # Item Name
        itemName: "§8§a"
        # 模型数据，仅支持1.14+
        customModelData: 10000
        material: "PLAYER_HEAD"
        # 显示时长，秒，小于或等于0则无该动态
        time: 10
        # 下一个动态ID，无或留空则取消技能动态动作
        nextAnimationID: "ha"
```



