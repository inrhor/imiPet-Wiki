# 权限与命令

{% hint style="warning" %}
本命令帮助基于4.1.0+版本
{% endhint %}

## 普通命令权限 <a id="&#x666E;&#x901A;&#x547D;&#x4EE4;&#x6743;&#x9650;"></a>

```text
普通玩家通用的权限：imipet.player.use

/imipet help
  说明：查看命令帮助
  
/imipet admin
  权限：imipet.admin.help
  说明：查看管理命令帮助
  
/imipet open
  说明：打开宠物系统界面
  
/imipet packlist
  说明：查看宠物背包列表
  
/imipet expbox look
  说明：查看经验存储盒的经验值
  
/imipet follow 宠物槽位
  说明：召唤或收回指定宠物 宠物槽位为1-6
  
/imipet cure 宠物数位 回血量数
  说明：治疗指定宠物 宠物槽位为1-6
  
/imipet food 宠物槽位 回复活力数
  说明：喂养指定宠物 宠物槽位为1-6
  
/imipet givepetexp 宠物槽位 给定经验数
  说明：给予经验给指定宠物 宠物槽位为1-6
  
/imipet evolution 宠物数位
  说明：进化指定宠物 宠物槽位为1-6
  
/imipet release 宠物槽位
  说明：放生指定宠物 宠物槽位为1-6
  
/imipet rename 宠物数位 新名称
  说明：为指定宠物更改名称 宠物槽位为1-6
  
/imipet transfer 宠物槽位 目标玩家
  说明：为指定宠物更改名称 宠物槽位为1-6
  
imipet into 仓库宠物数位 背包宠物数位
  说明：将指定仓库的宠物放入背包 仓库宠物数位为无限 宠物槽位为1-6
  
/imipet ride
/imipet ride 宠物槽位(1-6)
  说明：骑行正在跟随的宠物
  
/imipet skill open
  说明：打开跟随的宠物的技能触发器界面
```

## 管理员命令权限 <a id="&#x7BA1;&#x7406;&#x5458;&#x547D;&#x4EE4;&#x6743;&#x9650;"></a>

```text
/imipet petGive 玩家 模型ID
  权限：imipet.admin.pet.give
  说明：给予指定玩家一个宠物
/imipet release 玩家 宠物槽位
  权限：imipet.admin.release
  说明：放生玩家的目标宠物 宠物槽位为1-6
  
/imipet expboxlook 玩家
  权限：imipet.admin.expbox.look
  说明：查看指定玩家经验存储盒的经验值
  
/imipet expbox give 玩家 经验值
  权限：imipet.admin.expbox.give
  说明：给予指定玩家经验存储盒的经验值
  
/imipet expboxdel 玩家 经验值
  权限：imipet.admin.expbox.del
  说明：扣除指定玩家经验存储盒的经验值
  
/imipet expboxset 玩家 经验值
  权限：imipet.admin.expbox.set
  说明：设置指定玩家经验存储盒的经验值
  
/imipet takeback 玩家
  权限：imipet.admin.takeback
  说明：强制收回玩家的目标宠物
  
/imipet lottery 玩家 模型ID 概率
  权限：imipet.lottery
  说明：宠物抽奖，概率可填0至1之间的数字
  
/imipet skillGive 目标玩家 技能ID
  权限：imipet.admin.skillgive
  说明：为目标玩家的宠物新增非装载的技能
```

