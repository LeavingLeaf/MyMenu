# ShangTangWawacai
## Materials
### Core
- Wawacai (Chinese Cabbage or other alternatives: baby cabbage)
  - Num: Depends
- SongHuaEgg (Preserved Egg)
  - Num: 2
- Egg
  - Num: 1~2
- WucanPork (Spam / luncheon meat)
  - Depends
- Water
  - Depends
### Alternatives
- Carrot
- Mushroom
### Seasoning
- Chicken Powder
- Salt
## Pseudo STEPs
1. **Pre-Process**
  - WashedVeg = Wash(Wawacai, Alternatives*)
  - Egg_Dice = Dice(Egg_Pancake)
    - Egg_Pancake = Fry([Egg, Salt.quarterSpoon], 3min, LEVEL5 )
  - SonghuaEgg_Dice = Dice(SonghuaEgg_Peeled)
    - SonghuaEgg_Peeled = Peel(SongHua_Egg)
  - Topping = [Dice(Alternatives*, WucanPork), Egg_Dice]
  - [Wawacai_blanch, Soup_Boil] = Blanch(Wawacai, 3min, LEVEL5) 
2. **Main-Process**
    1. interProduct = Fry(SonghuaEgg_Dice, 3min, LEVEL5)
    2. interProduct = Fry([interProduct, Soup_Boil], 1min, LEVEL5)
    3. Soup = Fry([interProduct, ChickernPowder.halfSpoon, Salt.quarterSpoon], 1min, LEVEL5])
3. **Plate Presentation**
    1. interPlate = Plate([Wawacai_blach, Topping )
    2. FinalPlate = Plate(interPlate, Soup)
