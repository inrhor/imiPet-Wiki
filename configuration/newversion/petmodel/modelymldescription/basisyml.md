---
description: 基本值
---

# basis.yml

{% hint style="danger" %}
必填
{% endhint %}

## 示例

```text
# 基本值
basis:
  display:
    # 默认的宠物名称
    name: "小天使"
    # 名称格式
    format: "&7[&6主人：&f%imipet_owner%&7] &f%imipet_name%"
    # 是否显示名称
    show: true
    # 可选：hd，tr, cmi
    useShow: hd
    # 全息
    hd:
      # 显示名称Y轴
      height: 2
      # 显示名称X轴
      x: 0
      # 显示名称Z轴
      z: 0
      formatList:
        - "&7[&6主人：&f%imipet_owner%&7][&flv.%imipet_level%&7]"
        - "&f%imipet_name%"
        - "&c血量 &f%imipet_nowhp%&7/&f%imipet_maxhp%"
    # 太弱全息
    tr:
      height: 2
      x: 0
      z: 0
      formatList:
        - "&7[&6主人：&f%imipet_owner%&7][&flv.%imipet_level%&7]"
        - '&e%animations_typewriter?pause=3,reverse=true_%imipet_name%%<update:5>'
        - "&c血量 &f%imipet_nowhp%&7/&f%imipet_maxhp%"
    # cmi
    cmi:
      height: 2
      x: 0
      z: 0
      formatList:
        - "&7[&6主人：&f%imipet_owner%&7][&flv.%imipet_level%&7]"
        - "&f%imipet_name%"
        - "&c血量 &f%imipet_nowhp%&7/&f%imipet_maxhp%"
  # 初始血量
  HP: 20
  # 初始伤害范围
  minDamage: 2
  maxDamage: 6
  # 初始活力值
  food: 20
  # 初始最极经验值
  exp: 100
  # 等级上限
  level: 100
```

## 可填变量

```text
%imipet_owner%  主人名称
%imipet_name%  宠物名称
%imipet_level%  宠物等级
%imipet_nowexp%  宠物当前经验
%imipet_maxexp%  宠物最大经验
%imipet_nowhp%  宠物当前血量
%imipet_maxhp%  宠物最大血量
%imipet_nowfood%  宠物当前活力
%imipet_maxfood%  宠物最大活力
%imipet_damage% 宠物攻击力
```



