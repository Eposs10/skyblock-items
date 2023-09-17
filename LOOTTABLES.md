# LootTables

```java
public class MobLootTableModifiers {

    private static final Identifier WITHER_ID = new Identifier("minecraft", "entities/wither");
    private static final Identifier WITHER_SKELETON_ID = new Identifier("minecraft", "entities/wither_skeleton");
    private static final Identifier ENDERMAN_ID = new Identifier("minecraft", "entities/enderman");
    private static final Identifier ENDER_DRAGON_ID = new Identifier("minecraft", "entities/ender_dragon");
    private static final Identifier POLAR_BEAR_ID = new Identifier("minecraft", "entities/polar_bear");

    private static final Identifier BASTION_TREASURE_ID = new Identifier("minecraft", "chests/bastion_treasure");
    private static final Identifier BASTION_OTHER_ID = new Identifier("minecraft", "chests/bastion_other");
    private static final Identifier BASTION_HOGLIN_STABLE_ID = new Identifier("minecraft", "chests/bastion_hoglin_stable");
    private static final Identifier BASTION_bridge_ID = new Identifier("minecraft", "chests/bastion_hoglin_bridge");

    public static void modifyLootTables() {
        LootTableEvents.MODIFY.register(((resourceManager, lootManager, id, tableBuilder, source) -> {
            if (WITHER_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(1))
                        .conditionally(RandomChanceLootCondition.builder(0.1f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.NECRON_HANDLE)) // Item
                        .with(ItemEntry.builder(ModItems.IMPLOSION)) // Item
                        .with(ItemEntry.builder(ModItems.WITHER_SHIELD)) // Item
                        .with(ItemEntry.builder(ModItems.SHADOW_WARP)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 1.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }

            if (WITHER_SKELETON_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(1))
                        .conditionally(RandomChanceLootCondition.builder(0.01f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.WITHER_CATALYST)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 1.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }

            if (ENDERMAN_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(1))
                        .conditionally(RandomChanceLootCondition.builder(0.01f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.ABSOLUTE_ENDER_PEARL)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 3.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }

            if (ENDERMAN_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(1))
                        .conditionally(RandomChanceLootCondition.builder(0.001f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.JUDGEMENT_CORE)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 1.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }

            if (ENDER_DRAGON_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(1))
                        .conditionally(RandomChanceLootCondition.builder(0.35f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.DRAGON_FRAGMENT)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 1.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }

            if (POLAR_BEAR_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(1))
                        .conditionally(RandomChanceLootCondition.builder(0.2f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.TRUE_ICE)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 1.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }

            if (BASTION_TREASURE_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(2))
                        .conditionally(RandomChanceLootCondition.builder(0.2f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.DIAMANTE_HANDLE)) // Item
                        .with(ItemEntry.builder(ModItems.LASR_EYE)) // Item
                        .with(ItemEntry.builder(ModItems.BIGFOOT_LASSO)) // Item
                        .with(ItemEntry.builder(ModItems.JOLLY_PINK_ROCK)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 3.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }

            if (BASTION_HOGLIN_STABLE_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(1))
                        .conditionally(RandomChanceLootCondition.builder(0.2f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.DIAMANTE_HANDLE)) // Item
                        .with(ItemEntry.builder(ModItems.LASR_EYE)) // Item
                        .with(ItemEntry.builder(ModItems.BIGFOOT_LASSO)) // Item
                        .with(ItemEntry.builder(ModItems.JOLLY_PINK_ROCK)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 2.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }

            if (BASTION_bridge_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(1))
                        .conditionally(RandomChanceLootCondition.builder(0.2f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.DIAMANTE_HANDLE)) // Item
                        .with(ItemEntry.builder(ModItems.LASR_EYE)) // Item
                        .with(ItemEntry.builder(ModItems.BIGFOOT_LASSO)) // Item
                        .with(ItemEntry.builder(ModItems.JOLLY_PINK_ROCK)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 2.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }

            if (BASTION_OTHER_ID.equals(id)) {
                var poolBuilder = LootPool.builder()
                        .rolls(ConstantLootNumberProvider.create(1))
                        .conditionally(RandomChanceLootCondition.builder(0.2f))   // Drop Chance 1 = 100%
                        .with(ItemEntry.builder(ModItems.DIAMANTE_HANDLE)) // Item
                        .with(ItemEntry.builder(ModItems.LASR_EYE)) // Item
                        .with(ItemEntry.builder(ModItems.BIGFOOT_LASSO)) // Item
                        .with(ItemEntry.builder(ModItems.JOLLY_PINK_ROCK)) // Item
                        .apply(SetCountLootFunction.builder(UniformLootNumberProvider.create(1.0f, 2.0f)).build()); // Item count

                tableBuilder.pool(poolBuilder.build());
            }
        }));
    }
}

