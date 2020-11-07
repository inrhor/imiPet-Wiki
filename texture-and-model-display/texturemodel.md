# 关于Java模型纹理材质

{% hint style="success" %}
4.1.0+推出了自动生成纹理资源包功能，因此**你可以跳过本教程**
{% endhint %}

## 前言 <a id="&#x524D;&#x8A00;"></a>

{% hint style="danger" %}
注意

这里仅讲纹理与部件显示的有关内容，若想学习模型制作，请另寻教程
{% endhint %}

{% hint style="info" %}
好消息

imiPet-4.0.0后可以自定义物品材质，默认是钻石锄子
{% endhint %}

{% hint style="success" %}
有关模型创建和调用的超详细的教程：[https://pack.imipet.com/](https://pack.imipet.com/)
{% endhint %}

## 高清修复 <a id="&#x9AD8;&#x6E05;&#x4FEE;&#x590D;"></a>

高清修复就是OptiFine

```text
animation:
  # 空闲状态
  idle:
    # 物品名称
    itemName: "pet1"
```

我们来剖解纹理包看看

```text
type=item
items=minecraft:diamond_hoe
nbt.display.Name=pet1
model=./head
```

可以看到，minecraft:diamond\_hoe是钻石锄子的名称，pet1是物品名称

具体请看：[https://pack.imipet.com/](https://pack.imipet.com/)

## 模型数据 <a id="&#x6A21;&#x578B;&#x6570;&#x636E;"></a>

如果不想要耐久值或高清修复，那么有模型数据值得选择  
请看：[https://pack.imipet.com/](https://pack.imipet.com/)

## 常见问题 <a id="&#x5E38;&#x89C1;&#x95EE;&#x9898;"></a>

{% hint style="danger" %}
纹理包版本过低？
{% endhint %}

提示旧版本是材质包内pack.mcmeta文件设置问题

```text
{
  "pack": {
    "pack_format": 3
  }
}
```

请根据需要，修改数字  
1.12 pack\_format=3  
1.13-1.14 pack\_format=4  
1.15 pack\_format=5  
1.16 pack\_format=6

{% hint style="info" %}
如何将多个纹理包放入同一纹理包？
{% endhint %}

请看教程：[http://www.imipet.com/threads/23/](http://www.imipet.com/threads/23/)

{% hint style="info" %}
纹理包是什么？客户端如何使用纹理包？
{% endhint %}

这么简单都不懂，纹理包也就是材质包，也就是资源包，我只是喜欢这么称呼

纹理包放入客户端的位置：.minecraft\resourcepacks

然后在客户端按 ESC键，点击资源包，放入右侧完成后自动加载资源包

