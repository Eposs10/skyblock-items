# Item list

```java
    public static final Item ROGUE_SWORD = registerItem("rogue_sword",
            new RogueSword(ModItemMaterial.ZERO_POINT_FIVE_DIA, 2, -2.4f,  new FabricItemSettings().maxCount(1), "COMMON", "SWORD"));

    public static final Item ASPECT_OF_THE_END = registerItem("aspect_of_the_end",
            new AspectOfTheEnd(ModItemMaterial.ZERO_POINT_FIVE_DIA, 2, -2.4f, new FabricItemSettings().maxCount(1), "RARE", "SWORD"));
    public static final Item ASPECT_OF_THE_VOID = registerItem("aspect_of_the_void",
            new AspectOfTheVoid(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1), "EPIC", "SWORD"));

    public static final Item ASPECT_OF_THE_DRAGONS = registerItem("aspect_of_the_dragons",
            new WeaponWithRarity(ModItemMaterial.DRAGON_FRAGMENT, 5, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "LEGENDARY", "SWORD"));

    public static final Item SILENT_DEATH = registerItem("silent_death",
            new WeaponWithRarity(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1), "EPIC", "SWORD"));

    public static final Item FLOWER_OF_TRUTH = registerItem("flower_of_truth",
            new WeaponWithRarity(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1), "LEGENDARY", "SWORD"));

    public static final Item YETI_SWORD = registerItem("yeti_sword",
            new WeaponWithRarity(ModItemMaterial.ZERO_POINT_FIVE_DIA, 2, -2.4f, new FabricItemSettings().maxCount(1), "LEGENDARY", "SWORD"));

    public static final Item GIANT_SWORD = registerItem("giant_sword",
            new WeaponWithRarity(ModItemMaterial.DRAGON_FRAGMENT, 7, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "MYTHIC", "LONGSWORD"));

    public static final Item DARK_CLAYMORE = registerItem("dark_claymore",
            new WeaponWithRarity(ModItemMaterial.DRAGON_FRAGMENT, 9, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "SUPREME", "LONGSWORD"));

    public static final Item NECRON_BLADE = registerItem("necron_blade",
            new NecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "LEGENDARY", "SWORD"));
    public static final Item NECRON_BLADE_SCROLLED = registerItem("necron_blade_scrolled",
            new ScrolledNecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "MYTHIC", "SWORD"));
    public static final Item HYPERION = registerItem("hyperion",
            new NecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "LEGENDARY", "SWORD"));
    public static final Item HYPERION_SCROLLED = registerItem("hyperion_scrolled",
            new ScrolledNecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "MYTHIC", "SWORD"));
    public static final Item ASTRAEA = registerItem("astraea",
            new NecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "LEGENDARY", "SWORD"));
    public static final Item ASTRAEA_SCROLLED = registerItem("astraea_scrolled",
            new ScrolledNecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "MYTHIC", "SWORD"));
    public static final Item VALKYRIE = registerItem("valkyrie",
            new NecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "LEGENDARY", "SWORD"));
    public static final Item VALKYRIE_SCROLLED = registerItem("valkyrie_scrolled",
            new ScrolledNecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "MYTHIC", "SWORD"));
    public static final Item SCYLLA = registerItem("scylla",
            new NecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "LEGENDARY", "SWORD"));
    public static final Item SCYLLA_SCROLLED = registerItem("scylla_scrolled",
            new ScrolledNecronBlades(ModItemMaterial.ZERO_POINT_FIVE_DIA, 3, -2.4f, new FabricItemSettings().maxCount(1).fireproof(), "MYTHIC", "SWORD"));


    public static final Item JUJU_SHORTBOW = registerItem("juju_shortbow", new JujuShortbow(new FabricItemSettings().maxCount(1)));
    public static final Item TERMINATOR = registerItem("terminator", new Terminator(new FabricItemSettings().maxCount(1).fireproof()));


    public static final Item DRAGON_HELMET = registerItem("dragon_helmet",
            new ArmorItemWithRarity(ModArmorMaterials.DRAGON_FRAGMENT, ArmorItem.Type.HELMET, new FabricItemSettings().fireproof(), "LEGENDARY"));
    public static final Item DRAGON_CHESTPLATE = registerItem("dragon_chestplate",
            new ArmorItemWithRarity(ModArmorMaterials.DRAGON_FRAGMENT, ArmorItem.Type.CHESTPLATE, new FabricItemSettings().fireproof(), "LEGENDARY"));
    public static final Item DRAGON_LEGGINGS = registerItem("dragon_leggings",
            new ArmorItemWithRarity(ModArmorMaterials.DRAGON_FRAGMENT, ArmorItem.Type.LEGGINGS, new FabricItemSettings().fireproof(), "LEGENDARY"));
    public static final Item DRAGON_BOOTS = registerItem("dragon_boots",
            new ArmorItemWithRarity(ModArmorMaterials.DRAGON_FRAGMENT, ArmorItem.Type.BOOTS, new FabricItemSettings().fireproof(), "LEGENDARY"));

    public static final Item WITHER_HELMET = registerItem("wither_helmet",
            new ArmorItemWithRarity(ModArmorMaterials.WITHER, ArmorItem.Type.HELMET, new FabricItemSettings().fireproof(), "LEGENDARY"));
    public static final Item WITHER_CHESTPLATE = registerItem("wither_chestplate",
            new ArmorItemWithRarity(ModArmorMaterials.WITHER, ArmorItem.Type.CHESTPLATE, new FabricItemSettings().fireproof(), "LEGENDARY"));
    public static final Item WITHER_LEGGINGS = registerItem("wither_leggings",
            new ArmorItemWithRarity(ModArmorMaterials.WITHER, ArmorItem.Type.LEGGINGS, new FabricItemSettings().fireproof(), "LEGENDARY"));
    public static final Item WITHER_BOOTS = registerItem("wither_boots",
            new ArmorItemWithRarity(ModArmorMaterials.WITHER, ArmorItem.Type.BOOTS, new FabricItemSettings().fireproof(), "LEGENDARY"));

    public static final Item NECRON_HELMET = registerItem("necron_helmet",
            new ArmorItemWithRarity(ModArmorMaterials.NECRON, ArmorItem.Type.HELMET, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item NECRON_CHESTPLATE = registerItem("necron_chestplate",
            new ArmorItemWithRarity(ModArmorMaterials.NECRON, ArmorItem.Type.CHESTPLATE, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item NECRON_LEGGINGS = registerItem("necron_leggings",
            new ArmorItemWithRarity(ModArmorMaterials.NECRON, ArmorItem.Type.LEGGINGS, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item NECRON_BOOTS = registerItem("necron_boots",
            new ArmorItemWithRarity(ModArmorMaterials.NECRON, ArmorItem.Type.BOOTS, new FabricItemSettings().fireproof(), "MYTHIC"));

    public static final Item STORM_HELMET = registerItem("storm_helmet",
            new ArmorItemWithRarity(ModArmorMaterials.STORM, ArmorItem.Type.HELMET, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item STORM_CHESTPLATE = registerItem("storm_chestplate",
            new ArmorItemWithRarity(ModArmorMaterials.STORM, ArmorItem.Type.CHESTPLATE, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item STORM_LEGGINGS = registerItem("storm_leggings",
            new ArmorItemWithRarity(ModArmorMaterials.STORM, ArmorItem.Type.LEGGINGS, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item STORM_BOOTS = registerItem("storm_boots",
            new ArmorItemWithRarity(ModArmorMaterials.STORM, ArmorItem.Type.BOOTS, new FabricItemSettings().fireproof(), "MYTHIC"));

    public static final Item MAXOR_HELMET = registerItem("maxor_helmet",
            new ArmorItemWithRarity(ModArmorMaterials.MAXOR, ArmorItem.Type.HELMET, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item MAXOR_CHESTPLATE = registerItem("maxor_chestplate",
            new ArmorItemWithRarity(ModArmorMaterials.MAXOR, ArmorItem.Type.CHESTPLATE, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item MAXOR_LEGGINGS = registerItem("maxor_leggings",
            new ArmorItemWithRarity(ModArmorMaterials.MAXOR, ArmorItem.Type.LEGGINGS, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item MAXOR_BOOTS = registerItem("maxor_boots",
            new ArmorItemWithRarity(ModArmorMaterials.MAXOR, ArmorItem.Type.BOOTS, new FabricItemSettings().fireproof(), "MYTHIC"));

    public static final Item GOLDOR_HELMET = registerItem("goldor_helmet",
            new ArmorItemWithRarity(ModArmorMaterials.GOLDOR, ArmorItem.Type.HELMET, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item GOLDOR_CHESTPLATE = registerItem("goldor_chestplate",
            new ArmorItemWithRarity(ModArmorMaterials.GOLDOR, ArmorItem.Type.CHESTPLATE, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item GOLDOR_LEGGINGS = registerItem("goldor_leggings",
            new ArmorItemWithRarity(ModArmorMaterials.GOLDOR, ArmorItem.Type.LEGGINGS, new FabricItemSettings().fireproof(), "MYTHIC"));
    public static final Item GOLDOR_BOOTS = registerItem("goldor_boots",
            new ArmorItemWithRarity(ModArmorMaterials.GOLDOR, ArmorItem.Type.BOOTS, new FabricItemSettings().fireproof(), "MYTHIC"));


    public static final Item ABSOLUTE_ENDER_PEARL = registerItem("absolute_ender_pearl",
            new ItemWithRarity(new FabricItemSettings().maxCount(16), "UNCOMMON", "ITEM"));
    public static final Item TESSELATED_ENDER_PEARL = registerItem("tesselated_ender_pearl",
            new ItemWithRarity(new FabricItemSettings().maxCount(16), "RARE", "ITEM"));

    public static final Item WITHER_CATALYST = registerItem("wither_catalyst", new ItemWithRarity(new FabricItemSettings(), "RARE", "ITEM"));
    public static final Item WITHER_FRAGMENT = registerItem("wither_fragment", new ItemWithRarity(new FabricItemSettings(), "EPIC", "ITEM"));

    public static final Item BIGFOOT_LASSO = registerItem("bigfoot_lasso", new ItemWithRarity(new FabricItemSettings(), "EPIC", "ITEM"));
    public static final Item DIAMANTE_HANDLE = registerItem("diamante_handle", new ItemWithRarity(new FabricItemSettings(), "EPIC", "ITEM"));
    public static final Item JOLLY_PINK_ROCK = registerItem("jolly_pink_rock", new ItemWithRarity(new FabricItemSettings(), "EPIC", "ITEM"));
    public static final Item LASR_EYE = registerItem("lasr_eye", new ItemWithRarity(new FabricItemSettings(), "EPIC", "ITEM"));

    public static final Item NECRON_HANDLE = registerItem("necron_handle", new ItemWithRarity(new FabricItemSettings().fireproof(), "EPIC", "ITEM"));
    public static final Item IMPLOSION = registerItem("implosion", new WitherScrolls(new FabricItemSettings().fireproof()));
    public static final Item SHADOW_WARP = registerItem("shadow_warp", new WitherScrolls(new FabricItemSettings().fireproof()));
    public static final Item WITHER_SHIELD = registerItem("wither_shield", new WitherScrolls(new FabricItemSettings().fireproof()));

    public static final Item DRAGON_FRAGMENT = registerItem("dragon_fragment", new ItemWithRarity(new FabricItemSettings().fireproof(), "EPIC", "ITEM"));

    public static final Item ANCIENT_ROSE = registerItem("ancient_rose", new ItemWithRarity(new FabricItemSettings().fireproof(), "UNCOMMON", "ITEM"));
    public static final Item GOLEM_ROSE = registerItem("golem_rose", new ItemWithRarity(new FabricItemSettings().fireproof(), "RARE", "ITEM"));

    public static final Item GOLDEN_POWDER = registerItem("golden_powder", new ItemWithRarity(new FabricItemSettings().fireproof(), "RARE", "ITEM"));

    public static final Item SPELL_POWDER = registerItem("spell_powder", new ItemWithRarity(new FabricItemSettings().fireproof(), "UNCOMMON", "ITEM"));

    public static final Item TRUE_ICE = registerItem("true_ice", new ItemWithRarity(new FabricItemSettings().fireproof(), "RARE", "ITEM"));

    public static final Item JUDGEMENT_CORE = registerItem("judgement_core", new ItemWithRarity(new FabricItemSettings().fireproof(), "MYTHIC", "ITEM"));

    public static final Item DARK_HANDLE = registerItem("dark_handle", new ItemWithRarity(new FabricItemSettings().fireproof(), "SUPREME", "ITEM"));
    public static final Item DARK_BLADE = registerItem("dark_blade", new ItemWithRarity(new FabricItemSettings().fireproof(), "SUPREME", "ITEM"));

    public static final Item RECOMBOBULATOR_3000 = registerItem("recombobulator_3000", new ItemWithRarity(new FabricItemSettings(), "SPECIAL", "ITEM"));
