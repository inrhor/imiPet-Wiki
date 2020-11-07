# skill.yml

## Example

```text
skillModel:
  # Skill ID, must be a registered skill ID, case can be ignored
  MechaEngineering:
    # Skill Translation
    name: "&fMecha Engineering"
    animation:
      # Dynamic ID
      # The dynamic action of the pet model runs from the first dynamic ID
      a:
        # Whether to enable the ModelEngine plugin
        # The animation requirement name is skill-SkillID-DynamicID
        # like > skill-MechaEngineering-a
        useModelEngine: false
        itemName: "§8§a"
        customModelData: 10000
        material: "PLAYER_HEAD"
        # Display duration, seconds, less than or equal to 0, no such dynamic
        time: 10
        # Next dynamic ID, if none or left blank, the dynamic action of the skill will be cancelled
        nextAnimationID: "ha"
      ha:
        itemName: "§8§9"
        customModelData: 10001
        material: "PLAYER_HEAD"
        time: 5
    # The cooling time of this skill, in seconds, no cooling if less than or equal to 0
    coolDown: 60
    # Whether to allow movement during the skill release
    canMove: false
    # Trigger conditions, all conditions are met to trigger
    #    food:Food value needed to consume
    #    permission:Permission
    triggerList:
      - "food:10"
  # You can add more registered skill ID
  #xxx:
```

## Skill ID <a id="ji-neng-id"></a>

Refers to the skill ID that has been successfully created and registered in the skills folder

​[点击查看技能相关内容](https://wiki.imipet.com/configuration/newversion/skillmodel)​

## Dynamic ID

No strict requirements

​

