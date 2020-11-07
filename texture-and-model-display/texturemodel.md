# Texture And Model

## Common problem <a id="&#x5E38;&#x89C1;&#x95EE;&#x9898;"></a>

{% hint style="danger" %}
The texture pack version is too low?
{% endhint %}

Prompt that the old version is a problem with the pack.mcmeta file setting in the texture pack

```text
{
  "pack": {
    "pack_format": 3
  }
}
```

Please modify the number as needed  
1.12 pack\_format=3  
1.13-1.14 pack\_format=4  
1.15 pack\_format=5  
1.16 pack\_format=6

{% hint style="info" %}
How to put multiple texture packs into the same texture pack?
{% endhint %}

See tutorial：[http://www.imipet.com/threads/23/](http://www.imipet.com/threads/23/)

{% hint style="info" %}
How does the client use the texture pack?
{% endhint %}

The location where the texture package is placed on the client.：.minecraft\resourcepacks

Then press the ESC key on the client side, click the resource package, and automatically load the resource package after placing it on the right.

