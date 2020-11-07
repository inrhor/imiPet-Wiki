# Example

Add a model to the entity

  
1.Use a pet model that has been successfully registered through configuration

```text
Entity entity = ...;
String modelId = "modelID"
ModelEntityManager modelEntityManager = new ModelEntityManager(entity, modelId);
ModelEntityManager.fastSpawnModel(modelEntityManager, modelId);
```



2.Do not use registered model ID

```text
Entity entity = ...;
String modelId = "modelID"
ModelEntityManager modelEntityManager = new ModelEntityManager(entity, modelId);
modelEntityManager.setAnimationItemNameIdle(itemName);
modelEntityManager.setAnimationItemNameWalk(itemName);
modelEntityManager.setAnimationItemNameAttack(itemName);
modelEntityManager.setAnimationCustomModelDataIdle(customModelDataIdle);
modelEntityManager.setAnimationCustomModelDataWalk(customModelDataIdle);
modelEntityManager.setAnimationCustomModelDataAttack(customModelDataIdle);
modelEntityManager.setModelLocationH(height);
modelEntityManager.spawnModel();
```

