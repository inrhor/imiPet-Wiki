---
description: 其它功能
---

# feature.yml

{% hint style="danger" %}
必填
{% endhint %}

## 示例

```text
# 回复血量需求
cureHP:
  requirement:
    # 需要经济
    #   回复一血需要多少经济
    money: 0.1
    # 是否允许通过MC回血药水对宠物回血
    potion: false

# 宠物活力值
food:
  # 是否会消耗活力
  enable: true
  # 活力补充需求
  requirement:
    # 需要经济
    #   补充一活力需要多少经济
    money: 0.1

# 关于坐骑
ride:
  # 是否允许坐骑
  enable: true
  # 是否为小型盔甲架(坐骑时)
  isSmall: true
  # 是否可以飞行，否则是跳跃
  canFly: false
```

## 回复血量需求

```text
cureHP:
  requirement:
    # 需要经济
    #   回复一血需要多少经济
    money: 0.1
    # 是否允许通过MC回血药水对宠物回血
    potion: false
```

{% hint style="warning" %}
money 值 只在界面操作
{% endhint %}

## 宠物活力值

```text
# 宠物活力值
food:
  # 是否会消耗活力
  enable: true
  # 活力补充需求
  requirement:
    # 需要经济
    #   补充一活力需要多少经济
    money: 0.1
```

{% hint style="warning" %}
money 值 只在界面操作
{% endhint %}

## 关于坐骑

```text
# 关于坐骑
ride:
  # 是否允许坐骑
  enable: true
  # 是否为小型盔甲架(坐骑时)
  isSmall: true
  # 是否可以飞行，否则是跳跃
  canFly: false
```

