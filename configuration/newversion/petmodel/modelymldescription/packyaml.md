# pack.yml

## 这是什么

这是关于自动生成纹理资源包的配置

## 第一步：创建配置

目录：plugins\imiPet\models\模型\pack.yml（无就自行创建）

{% hint style="info" %}
optiFine是需要optiFine-Mod\(最新\)，识别物品名称而赋予材质模型

customModelData是判断物品数据而赋予材质模型，无需MOD，但仅支持Minecraft1.14+

all是生成optiFine和customModelData
{% endhint %}

```text
# 是否自动生成纹理包
autoSpawn: false
# 纹理包类型
#   optiFine
#   customModelData
#   all
type: "optiFine"
```

## 第二步

配置设置好了后，你需要在目录plugins\imiPet\models\模型\

创建名为pack文件夹，将纹理材质（json\[模型\]，png\[贴图\]，mcmeta\[动态\]）放进去

## 第三步

将刚才放入的纹理材质的名称统一改为如下（除了后缀）：

* idle  \(若该纹理材质是空闲状态，请改为idle\)
* walk \(同理，行走状态\)
* attack \(同理，攻击状态\)
* 技能\_动画ID （其它动作的纹理材质，根据[skill.yml](skillyml.md)

如图（技能为**MechaEngineering**，动画ID为**ha**）

![](../../../../.gitbook/assets/imipet2.png)

## 第四步

启动服务器或/imiPet reload重载

将会生成于目录plugins\imiPet

那么resourcePack就是你需要用的纹理资源包了

且慢，你还差一项工作：[pack.mcmeta](../../../../texture-and-model-display/texturemodel.md#常见问题)

## 最后

[放入客户端加载材质资源包即可](../../../../texture-and-model-display/texturemodel.md#常见问题)





