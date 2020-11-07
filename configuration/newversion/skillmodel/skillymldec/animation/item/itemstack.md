# 物品

{% hint style="info" %}
主要将物品用于头戴大型盔甲架，从而实现动态模型材质
{% endhint %}

{% hint style="danger" %}
若出错，说明材料填写不正确

诸如高版本和低版本绳子，两者名称是不相同的
{% endhint %}

```text
skill:
  animation:
    动态ID:
      type: item
      item:
        # 物品材料
        material: PLAYER_HEAD
        # 物品名称
        name: ""
        # 物品Lore
        lore:
          - ""
          - ""
        # 物品数据
        customModelData: 76382
```

{% hint style="info" %}
Lore可以去掉不填
{% endhint %}

