# FogUnciv - Ukrainian Civilization Mod for Unciv

## 📖 Description

**FogUnciv** is a mod for the turn-based strategy game **Unciv** that adds the **Ukrainian civilization** with its unique leader and military units. This mod aims to represent Ukraine as a playable nation with historically-inspired characteristics.

## ✨ Features

### 🏛️ Civilization: Ukraine
- **Leader:** Volodymyr Zelenskyy
- **Preferred Victory Type:** Scientific
- **Start Bias:** Plains and Rivers
- **Unique Unit:** Shahed (reconnaissance and attack drone)
- **National Colors:** 
  - Outer Color: Blue (#0066CC)
  - Inner Color: Gold (#FFCD00)

### 🚁 Unique Unit: Shahed
A modern unmanned aerial vehicle designed for reconnaissance and targeted strikes:
- **Type:** Ranged Unit
- **Cost:** 60 production
- **Movement Range:** 10 tiles
- **Combat Strength:** 40
- **Ranged Strength:** 75
- **Attack Range:** 3 tiles
- **Required Technology:** Radar
- **Special Rules:**
  - Cannot enter ocean tiles
  - Must set up before ranged attack

### 🏙️ Cities

Ukraine includes 20 historically significant Ukrainian cities:
Kyiv, Kharkiv, Odesa, Lviv, Dnipro, Donetsk, Luhansk, Zaporizhzhia, Mykolaiv, Mariupol, Chernivtsi, Rivne, Vinnytsia, Zhytomyr, Sumy, Poltava, Cherkasy, Khmelnytskyi, Ternopil, Ivano-Frankivsk

## 📦 Installation

### Prerequisites
- Unciv 4.0.0 or later
- (Optional) Understanding of Unciv mod structure

### Installation Steps

1. **Locate Unciv Mods Directory:**
   - **Windows:** `%APPDATA%\.unciv\mods\`
   - **Linux:** `~/.unciv/mods/`
   - **macOS:** `~/Library/Application Support/.unciv/mods/`

2. **Clone or Download This Repository:**
   ```bash
   git clone https://github.com/brawlvitya460-code/FogUnciv.git
   ```
   Or download as ZIP and extract.

3. **Move to Mods Directory:**
   - Copy the `FogUnciv` folder to your Unciv mods directory

4. **Enable in Unciv:**
   - Launch Unciv
   - Go to **Mods**
   - Find and enable **FogUnciv**
   - Restart Unciv

5. **Start New Game:**
   - Create a new game
   - Select **Ukraine** as your civilization

## 📋 What's Included

```
FogUnciv/
├─ mod.hjson                    # Mod metadata and configuration
├─ README.md                    # This file
├─ jsons/
│  ├─ Nations.json             # Ukraine civilization definition
│  ├─ Units.json               # Shahed unit definition
│  ├─ Buildings.json           # Empty (no unique buildings)
│  └─ Translations/
│     ├─ English.properties    # English localization
│     └─ Russian.properties    # Russian localization
└─ Images/                      # Directory for custom textures (currently empty)
```

## 📝 Confirmed Implementation Details

The following features are implemented using verified Unciv mechanics:

✅ **Civilization Definition:**
- National colors (outerColor, innerColor)
- Leader name and dialogue
- City names list
- Start bias (terrain preference)
- Unique unit designation
- Spy names for espionage missions

✅ **Unit Implementation:**
- Movement speed (10 tiles per turn)
- Combat strength values (40 melee, 75 ranged)
- Attack range (3 tiles)
- Production cost (60)
- Required technology (Radar)
- Unit type classification (Ranged)
- Basic unit uniques (ocean restriction, setup requirement)

✅ **Localization:**
- English and Russian translations
- Proper .properties format

## ⚠️ Implementation Limitations & Design Decisions

### Features NOT Implemented

The following features are **intentionally omitted** because they cannot be reliably confirmed in current Unciv documentation or require features not guaranteed in all Unciv versions:

❌ **Unique Bonuses/Penalties:**
- Tech cost reduction mechanics (exact implementation varies by version)
- Defense bonuses or regional effects
- Trade route bonuses
- Culture/Gold/Science multipliers specific to this civ

❌ **Unit Mechanics:**
- Self-destruct/kamikaze behavior (not a standard Unciv mechanic)
- Special bonuses against cities or defensive structures
- One-time attack limit per turn
- Suicide attack mechanics

❌ **Buildings:**
- Unique Ukrainian buildings (would require confirmed syntax)

❌ **Graphics & Audio:**
- Custom unit sprites/icons (currently uses default ranged unit graphics)
- Unique tile set graphics
- Leader portrait
- Civilization banner
- Sound effects

### Why These Limitations?

Unciv modding documentation and available resources don't provide sufficient verification for these features. To ensure stability and compatibility across different Unciv versions, only confirmed and well-documented mechanics were implemented.

**Future versions** of this mod can add these features once:
1. Unciv version is specified and locked
2. Official documentation confirms the exact syntax
3. Testing confirms functionality across target versions

## 🔧 Technical Notes

- **Format:** HJSON for metadata, JSON for game data, Properties for localization
- **Encoding:** UTF-8
- **Compatibility:** Tested with Unciv 4.0.0+
- **No External Dependencies:** Pure Unciv mod (no programming required)

## 🎮 Gameplay Tips

- **Shahed units** are powerful ranged attackers but vulnerable in close combat
- Ukraine's preference for **Scientific victory** suggests a technology-focused playstyle
- Use the extended movement range (10) to explore and attack from safe distances
- Radar technology is mid-game, so Shahed units become available in mid-game

## 🐛 Known Issues

None reported. Please file an issue if you encounter problems.

## 📚 Contributing

To contribute improvements:

1. Fork this repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Test thoroughly in Unciv
5. Commit and push (`git push origin feature/improvement`)
6. Create a Pull Request with detailed description

## 📜 License

This mod is created for the Unciv project and follows Unciv's modding community guidelines.

**Note:** Historical figures and names are used for educational and entertainment purposes.

## 🔗 Resources

- **Unciv GitHub:** https://github.com/yairm210/Unciv
- **Unciv Wiki:** https://unciv.fandom.com/
- **Unciv Mods Directory:** https://github.com/yairm210/Unciv/wiki/Mods

## 📞 Support

For issues, questions, or suggestions:
1. Check existing issues on GitHub
2. Review Unciv mod documentation
3. Create a new GitHub issue with detailed description

---

**Last Updated:** June 15, 2025  
**Version:** 1.0  
**Author:** FogUnciv Team