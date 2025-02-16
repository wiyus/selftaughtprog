In [[Fabric 1.21.4]], you may register items:

```
package org.name.mod.items;  
  
import net.minecraft.item.Item;  
import net.minecraft.item.Items;  
import net.minecraft.registry.RegistryKey;  
import net.minecraft.registry.RegistryKeys;  
import net.minecraft.util.Identifier;  
import java.util.function.Function;

public final class ModItems {  
    private ModItems() {  
    }  
  
    public static final Item PLACEHOLDER = register("placeholder", Item::new, new Item.Settings());  
  
    private static Item register(String p, Function<Item.Settings, Item> i, Item.Settings s) {  
        final RegistryKey<Item> registryKey = RegistryKey.of(RegistryKeys.ITEM, Identifier.of("modname", p));  
        return Items.register(registryKey, i, s);  
    }  // creates the function to register items
  
    public static void initialize() {  
    }  // allows the class to be initialized within the mod
}
```