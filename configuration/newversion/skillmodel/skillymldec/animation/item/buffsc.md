# 效果脚本

## 格式

```text
skill:
  animation:
    动态ID:
      type: item
      item:
        # 效果脚本
        buff:
          # MythicMobs:技能:多少秒后触发
          script:
            - "MythicMobs:AngrySludgePoison:3"
          # 多少秒后执行condition值
          timeCondition: 3
          # 关于再触发效果
          condition: "aim:false:all:10:3:2"
```

## script

```text
MythicMobs:技能:多少秒后触发
```

## timeCondition

```text
多少秒后执行condition值
```

## condition

### 扫描目标若没有目标则执行下一个动态ID，否则再次触发效果

{% hint style="warning" %}
建议[显示时长](../displaytime.md)的值填为 0 或 不填
{% endhint %}

```text
aim:盔甲架是否点头瞄准:瞄准目标:范围:扫描时长:下一个动态ID
```

### 触发即结束\(或不填\)

```text
one_time
```

