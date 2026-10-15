# VillagersPlus - More Trades - Clutter Coral

A data pack that adds the Clutter mod's coral to the VillagersPlus Oceanographer. The coral trades follow the same pattern VillagersPlus already uses for vanilla coral.

## Added Trades

**Sell** means the villager sells the item to you. **Exchange** means you hand over the dead form plus the emeralds and get the living form back.

| Profession    | Level      | Type     | Item                                      | Amount | Price     |
| ------------- | ---------- | -------- | ----------------------------------------- | ------ | --------- |
| Oceanographer | Apprentice | Sell     | Clutter Coral (any of the 11 types)       | 1      | 3 Emerald |
| Oceanographer | Apprentice | Exchange | Dead Clutter Coral for living coral       | 1      | 1 Emerald |
| Oceanographer | Journeyman | Sell     | Clutter Coral Fan                         | 1      | 3 Emerald |
| Oceanographer | Journeyman | Exchange | Dead Clutter Coral Fan for living fan     | 1      | 1 Emerald |
| Oceanographer | Expert     | Sell     | Clutter Coral Block                       | 1      | 5 Emerald |
| Oceanographer | Expert     | Exchange | Dead Clutter Coral Block for living block | 1      | 1 Emerald |
| Oceanographer | Master     | Sell     | Prismarine Crystals                       | 9      | 2 Emerald |
| Oceanographer | Master     | Sell     | Prismarine Shard                          | 9      | 2 Emerald |

That is 66 coral trades plus the 2 prismarine trades, 68 in total.

### Coral types and item ids

The 11 Clutter coral types are cup, ghost, slate, stone, thorn, cocoa, passion, toxic, gem, diamond and anchor. For each type `<type>`:

| Form       | Living                       | Dead                              |
| ---------- | ---------------------------- | --------------------------------- |
| Coral      | `clutter:<type>_coral`       | `clutter:dead_<type>_coral`       |
| Coral fan  | `clutter:<type>_coral_fan`   | `clutter:dead_<type>_coral_fan`   |
| Coral block | `clutter:<type>_coral_block` | `clutter:dead_<type>_coral_block` |

The trade data is in `data/villagersplus/villager_trades/oceanographer.json`.

## Requirements

- Minecraft 1.20.1
- [VillagersPlus](https://modrinth.com/mod/villagersplus)
- [Clutter](https://modrinth.com/mod/clutter)

## Testing

If you need to test, you can spawn a specific level of villager that will roll on the trade tables at that specific level only.

```
/summon villager ~ ~ ~ {VillagerData:{type:plains,profession:'villagersplus:oceanographer',level:5}}
```

This will summon an Oceanographer at the master level and pick two random master level trades.

## References

- [Minecraft Wiki - Trading](https://minecraft.wiki/w/Trading)
- [VillagersPlus - Adding Trades to Villagers](https://github.com/finallion/VillagersPlus?tab=readme-ov-file#adding-trades-to-villagers)
