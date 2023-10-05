# Recipes

```java
    public void generate(RecipeExporter exporter) {
        customHeadToHelmetItem(exporter, ModItems.DRAGON_HELMET, ModItems.ABSOLUTE_ENDER_PEARL, ModItems.DRAGON_HELMET_DUMMY);
        customHeadToHelmetItem(exporter, ModItems.WITHER_HELMET, Items.WITHER_SKELETON_SKULL, ModItems.WITHER_HELMET_DUMMY);
        customHeadToHelmetItem(exporter, ModItems.NECRON_HELMET, Items.WITHER_SKELETON_SKULL, ModItems.NECRON_HELMET_DUMMY);
        customHeadToHelmetItem(exporter, ModItems.STORM_HELMET, Items.WITHER_SKELETON_SKULL, ModItems.STORM_HELMET_DUMMY);
        customHeadToHelmetItem(exporter, ModItems.MAXOR_HELMET, Items.WITHER_SKELETON_SKULL, ModItems.MAXOR_HELMET_DUMMY);
        customHeadToHelmetItem(exporter, ModItems.GOLDOR_HELMET, Items.WITHER_SKELETON_SKULL, ModItems.GOLDOR_HELMET_DUMMY);

        offerNetheriteLikeUpgradeRecipe(exporter, Items.NETHERITE_SWORD, ModItems.DRAGON_FRAGMENT, ModItems.TESSELATED_ENDER_PEARL, RecipeCategory.COMBAT, ModItems.ASPECT_OF_THE_DRAGONS);

        offerNetheriteLikeUpgradeRecipe(exporter, Items.NETHERITE_HELMET, ModItems.DRAGON_FRAGMENT, ModItems.TESSELATED_ENDER_PEARL, RecipeCategory.COMBAT, ModItems.DRAGON_HELMET_DUMMY);
        offerNetheriteLikeUpgradeRecipe(exporter, Items.NETHERITE_CHESTPLATE, ModItems.DRAGON_FRAGMENT, ModItems.TESSELATED_ENDER_PEARL, RecipeCategory.COMBAT, ModItems.DRAGON_CHESTPLATE);
        offerNetheriteLikeUpgradeRecipe(exporter, Items.NETHERITE_LEGGINGS, ModItems.DRAGON_FRAGMENT, ModItems.TESSELATED_ENDER_PEARL, RecipeCategory.COMBAT, ModItems.DRAGON_LEGGINGS);
        offerNetheriteLikeUpgradeRecipe(exporter, Items.NETHERITE_BOOTS, ModItems.DRAGON_FRAGMENT, ModItems.TESSELATED_ENDER_PEARL, RecipeCategory.COMBAT, ModItems.DRAGON_BOOTS);

        swordCraftShape(exporter, ModItems.ROGUE_SWORD, Items.GOLD_BLOCK, Items.GOLD_BLOCK, Items.STICK);

        swordCraftShape(exporter, ModItems.NECRON_BLADE, ModItems.WITHER_CATALYST, ModItems.WITHER_CATALYST, ModItems.NECRON_HANDLE);

        bigSwordCraftShape(exporter, ModItems.ASPECT_OF_THE_END, ModItems.ABSOLUTE_ENDER_PEARL, Items.STICK);
        bigSwordCraftShape(exporter, ModItems.ASPECT_OF_THE_VOID, ModItems.TESSELATED_ENDER_PEARL, ModItems.ASPECT_OF_THE_END);

        swordCraftShape(exporter, ModItems.YETI_SWORD, Items.BLUE_ICE, Items.BLUE_ICE, ModItems.TRUE_ICE);

        recipe8x1(exporter, ModItems.FLOWER_OF_TRUTH, Items.WITHER_ROSE, ModItems.ANCIENT_ROSE, RecipeCategory.COMBAT);

        offerNetheriteLikeUpgradeRecipe(exporter, ModItems.ASPECT_OF_THE_DRAGONS, ModItems.GOLEM_ROSE, ModItems.ANCIENT_ROSE, RecipeCategory.COMBAT, ModItems.GIANT_SWORD);

        swordCraftShape(exporter, ModItems.SILENT_DEATH, ModItems.SILENT_DUST, ModItems.DEATH_POWDER, Items.STICK);

        ShapedRecipeJsonBuilder.create(RecipeCategory.MISC, ModItems.DARK_BLADE, 1)
                .pattern("  #")
                .pattern(" # ")
                .pattern("#  ")
                .input('#', Blocks.NETHERITE_BLOCK)
                .criterion(hasItem(Blocks.NETHERITE_BLOCK), conditionsFromItem(Blocks.NETHERITE_BLOCK))
                .offerTo(exporter, new Identifier(getRecipeName(ModItems.DARK_BLADE)));

        offerNetheriteLikeUpgradeRecipe(exporter, ModItems.GIANT_SWORD, ModItems.DARK_HANDLE, ModItems.DARK_BLADE, RecipeCategory.COMBAT, ModItems.DARK_CLAYMORE);

        addScrollsToWitherBlade(exporter, ModItems.VALKYRIE_SCROLLED, ModItems.VALKYRIE);
        addScrollsToWitherBlade(exporter, ModItems.HYPERION_SCROLLED, ModItems.HYPERION);
        addScrollsToWitherBlade(exporter, ModItems.SCYLLA_SCROLLED, ModItems.SCYLLA);
        addScrollsToWitherBlade(exporter, ModItems.ASTRAEA_SCROLLED, ModItems.ASTRAEA);
        addScrollsToWitherBlade(exporter, ModItems.NECRON_BLADE_SCROLLED, ModItems.NECRON_BLADE);

        witherItemsCraftShape(exporter, ModItems.VALKYRIE, ModItems.DIAMANTE_HANDLE, ModTags.Items.NECRON_BLADES);
        witherItemsCraftShape(exporter, ModItems.HYPERION, ModItems.LASR_EYE, ModTags.Items.NECRON_BLADES);
        witherItemsCraftShape(exporter, ModItems.SCYLLA, ModItems.BIGFOOT_LASSO, ModTags.Items.NECRON_BLADES);
        witherItemsCraftShape(exporter, ModItems.ASTRAEA, ModItems.JOLLY_PINK_ROCK, ModTags.Items.NECRON_BLADES);

        witherItemsCraftShape(exporter, ModItems.VALKYRIE_SCROLLED, ModItems.DIAMANTE_HANDLE, ModTags.Items.SCROLLED_NECRON_BLADES);
        witherItemsCraftShape(exporter, ModItems.HYPERION_SCROLLED, ModItems.LASR_EYE, ModTags.Items.SCROLLED_NECRON_BLADES);
        witherItemsCraftShape(exporter, ModItems.SCYLLA_SCROLLED, ModItems.BIGFOOT_LASSO, ModTags.Items.SCROLLED_NECRON_BLADES);
        witherItemsCraftShape(exporter, ModItems.ASTRAEA_SCROLLED, ModItems.JOLLY_PINK_ROCK, ModTags.Items.SCROLLED_NECRON_BLADES);


        offerNetheriteLikeUpgradeRecipe(exporter, ModItems.DRAGON_HELMET_DUMMY, ModItems.WITHER_FRAGMENT, ModItems.WITHER_CATALYST, RecipeCategory.COMBAT, ModItems.WITHER_HELMET_DUMMY);
        offerNetheriteLikeUpgradeRecipe(exporter, ModItems.DRAGON_CHESTPLATE, ModItems.WITHER_FRAGMENT, ModItems.WITHER_CATALYST, RecipeCategory.COMBAT, ModItems.WITHER_CHESTPLATE);
        offerNetheriteLikeUpgradeRecipe(exporter, ModItems.DRAGON_LEGGINGS, ModItems.WITHER_FRAGMENT, ModItems.WITHER_CATALYST, RecipeCategory.COMBAT, ModItems.WITHER_LEGGINGS);
        offerNetheriteLikeUpgradeRecipe(exporter, ModItems.DRAGON_BOOTS, ModItems.WITHER_FRAGMENT, ModItems.WITHER_CATALYST, RecipeCategory.COMBAT, ModItems.WITHER_BOOTS);

        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_HELMETS, ModItems.DIAMANTE_HANDLE, ModItems.DIAMANTE_HANDLE, RecipeCategory.COMBAT, ModItems.NECRON_HELMET_DUMMY);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_CHESTPLATES, ModItems.DIAMANTE_HANDLE, ModItems.DIAMANTE_HANDLE, RecipeCategory.COMBAT, ModItems.NECRON_CHESTPLATE);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_LEGGINGS, ModItems.DIAMANTE_HANDLE, ModItems.DIAMANTE_HANDLE, RecipeCategory.COMBAT, ModItems.NECRON_LEGGINGS);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_BOOTS, ModItems.DIAMANTE_HANDLE, ModItems.DIAMANTE_HANDLE, RecipeCategory.COMBAT, ModItems.NECRON_BOOTS);

        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_HELMETS, ModItems.LASR_EYE, ModItems.LASR_EYE, RecipeCategory.COMBAT, ModItems.STORM_HELMET_DUMMY);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_CHESTPLATES, ModItems.LASR_EYE, ModItems.LASR_EYE, RecipeCategory.COMBAT, ModItems.STORM_CHESTPLATE);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_LEGGINGS, ModItems.LASR_EYE, ModItems.LASR_EYE, RecipeCategory.COMBAT, ModItems.STORM_LEGGINGS);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_BOOTS, ModItems.LASR_EYE, ModItems.LASR_EYE, RecipeCategory.COMBAT, ModItems.STORM_BOOTS);

        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_HELMETS, ModItems.BIGFOOT_LASSO, ModItems.BIGFOOT_LASSO, RecipeCategory.COMBAT, ModItems.MAXOR_HELMET_DUMMY);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_CHESTPLATES, ModItems.BIGFOOT_LASSO, ModItems.BIGFOOT_LASSO, RecipeCategory.COMBAT, ModItems.MAXOR_CHESTPLATE);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_LEGGINGS, ModItems.BIGFOOT_LASSO, ModItems.BIGFOOT_LASSO, RecipeCategory.COMBAT, ModItems.MAXOR_LEGGINGS);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_BOOTS, ModItems.BIGFOOT_LASSO, ModItems.BIGFOOT_LASSO, RecipeCategory.COMBAT, ModItems.MAXOR_BOOTS);

        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_HELMETS, ModItems.JOLLY_PINK_ROCK, ModItems.JOLLY_PINK_ROCK, RecipeCategory.COMBAT, ModItems.GOLDOR_HELMET_DUMMY);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_CHESTPLATES, ModItems.JOLLY_PINK_ROCK, ModItems.JOLLY_PINK_ROCK, RecipeCategory.COMBAT, ModItems.GOLDOR_CHESTPLATE);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_LEGGINGS, ModItems.JOLLY_PINK_ROCK, ModItems.JOLLY_PINK_ROCK, RecipeCategory.COMBAT, ModItems.GOLDOR_LEGGINGS);
        offerNetheriteLikeUpgradeRecipeWithTags(exporter, ModTags.Items.WITHER_BOOTS, ModItems.JOLLY_PINK_ROCK, ModItems.JOLLY_PINK_ROCK, RecipeCategory.COMBAT, ModItems.GOLDOR_BOOTS);


        offer3x3CompactingRecipe(exporter, ModItems.ABSOLUTE_ENDER_PEARL, Items.ENDER_PEARL, RecipeCategory.MISC);
        offer3x3CompactingRecipe(exporter, ModItems.TESSELATED_ENDER_PEARL, ModItems.ABSOLUTE_ENDER_PEARL, RecipeCategory.MISC);

        offer3x3CompactingRecipe(exporter, ModItems.ANCIENT_ROSE, Items.POPPY, RecipeCategory.MISC);

        offer3x3CompactingRecipe(exporter, ModItems.GOLDEN_POWDER, Items.GOLD_BLOCK, RecipeCategory.MISC);

        recipe8x1(exporter, ModItems.JUJU_SHORTBOW, Items.BOW, ModItems.TESSELATED_ENDER_PEARL, RecipeCategory.COMBAT);

        offerNetheriteLikeUpgradeRecipe(exporter, ModItems.JUJU_SHORTBOW, ModItems.JUDGEMENT_CORE, ModItems.TESSELATED_ENDER_PEARL, RecipeCategory.COMBAT, ModItems.TERMINATOR);
    }

    private static void recipe8x1(RecipeExporter exporter, Item result, Item input, Item part, RecipeCategory category) {
        ShapedRecipeJsonBuilder.create(category, result, 1)
                .pattern("###")
                .pattern("#b#")
                .pattern("###")
                .input('#', part)
                .input('b', input)
                .criterion(hasItem(input), conditionsFromItem(input))
                .criterion(hasItem(part), conditionsFromItem(part))
                .offerTo(exporter, new Identifier(getRecipeName(result)));
    }

    private static void offer3x3CompactingRecipe(RecipeExporter exporter, Item result, Item input, RecipeCategory category) {
        ShapedRecipeJsonBuilder.create(category, result, 1)
                .pattern("###")
                .pattern("###")
                .pattern("###")
                .input('#', input)
                .criterion(RecipeProvider.hasItem(input), RecipeProvider.conditionsFromItem(input))
                .offerTo(exporter, new Identifier(getRecipeName(result) + "_3x3"));
    }

    private static void swordCraftShape(RecipeExporter exporter, Item result, Item bladeTop, Item bladeBottom, Item stick) {
        ShapedRecipeJsonBuilder.create(RecipeCategory.COMBAT, result, 1)
                .pattern("1")
                .pattern("2")
                .pattern("s")
                .input('1', bladeTop)
                .input('2', bladeBottom)
                .input('s', stick)
                .criterion(hasItem(bladeTop), conditionsFromItem(bladeTop))
                .criterion(hasItem(bladeBottom), conditionsFromItem(bladeBottom))
                .criterion(hasItem(stick), conditionsFromItem(stick))
                .offerTo(exporter, new Identifier(getRecipeName(result) + "_sword"));
    }

    private static void bigSwordCraftShape(RecipeExporter exporter, Item result, Item blade, Item stick) {
        ShapedRecipeJsonBuilder.create(RecipeCategory.COMBAT, result, 1)
                .pattern("###")
                .pattern("###")
                .pattern("#s#")
                .input('#', blade)
                .input('s', stick)
                .criterion(hasItem(blade), conditionsFromItem(blade))
                .criterion(hasItem(stick), conditionsFromItem(stick))
                .offerTo(exporter, new Identifier(getRecipeName(result) + "_big_sword"));
    }

    private static void witherItemsCraftShape(RecipeExporter exporter, Item result, Item part, TagKey<Item> inputItems) {
        ShapedRecipeJsonBuilder.create(RecipeCategory.COMBAT, result, 1)
                .pattern("###")
                .pattern("#a#")
                .pattern("###")
                .input('#', part)
                .input('a', inputItems)
                .criterion(hasItem(part), conditionsFromItem(part))
                .offerTo(exporter, new Identifier(getRecipeName(result) + "_wither_crafting"));
    }

    private static void addScrollsToWitherBlade(RecipeExporter exporter, Item result, Item input) {
        result.postProcessNbt(input.getDefaultStack().getNbt());
        ShapedRecipeJsonBuilder.create(RecipeCategory.COMBAT, result, 1)
                .pattern(" 1 ")
                .pattern("2s3")
                .pattern(" w ")
                .input('1', ModItems.IMPLOSION)
                .input('2', ModItems.WITHER_SHIELD)
                .input('3', ModItems.SHADOW_WARP)
                .input('w', ModItems.WITHER_CATALYST)
                .input('s', input)
                .criterion(hasItem(input), conditionsFromItem(input))
                .criterion(hasItem(ModItems.IMPLOSION), conditionsFromItem(ModItems.IMPLOSION))
                .criterion(hasItem(ModItems.WITHER_SHIELD), conditionsFromItem(ModItems.WITHER_SHIELD))
                .criterion(hasItem(ModItems.SHADOW_WARP), conditionsFromItem(ModItems.SHADOW_WARP))
                .criterion(hasItem(ModItems.WITHER_CATALYST), conditionsFromItem(ModItems.WITHER_CATALYST))
                .offerTo(exporter, new Identifier(getRecipeName(result)  + "_add_scrolls"));
    }

    private static void offerNetheriteLikeUpgradeRecipe(RecipeExporter exporter, Item input, Item template, Item addition, RecipeCategory category, Item result) {
        SmithingTransformRecipeJsonBuilder.create(
                        Ingredient.ofItems(template),
                        Ingredient.ofItems(input),
                        Ingredient.ofItems(addition),
                        category, result)
                .criterion(hasItem(addition), conditionsFromItem(addition))
                .criterion(hasItem(input), conditionsFromItem(input))
                .criterion(hasItem(template), conditionsFromItem(template))
                .offerTo(exporter, RecipeProvider.getItemPath(result) + "_smithing");
    }

    private static void offerNetheriteLikeUpgradeRecipeWithTags(RecipeExporter exporter, TagKey<Item> input, Item template, Item addition, RecipeCategory category, Item result) {
        SmithingTransformRecipeJsonBuilder.create(
                        Ingredient.ofItems(template),
                        Ingredient.fromTag(input),
                        Ingredient.ofItems(addition),
                        category, result)
                .criterion(hasItem(template), conditionsFromItem(template))
                .offerTo(exporter, RecipeProvider.getItemPath(result) + "_smithing");
    }

    private static void customHeadToHelmetItem(RecipeExporter exporter, Item input, Item addition, Item output) {
        SmithingTransformRecipeJsonBuilder.create(
                        Ingredient.ofItems(ModItems.RECOMBOBULATOR_3000),
                        Ingredient.ofItems(input),
                        Ingredient.ofItems(addition),
                        RecipeCategory.COMBAT, output)
                .criterion(hasItem(addition), conditionsFromItem(addition))
                .criterion(hasItem(input), conditionsFromItem(input))
                .criterion(hasItem(ModItems.RECOMBOBULATOR_3000), conditionsFromItem(ModItems.RECOMBOBULATOR_3000))
                .offerTo(exporter, RecipeProvider.getItemPath(output) + "_head_to_helmet");
    }
