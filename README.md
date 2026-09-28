# Legends of Eldoria

A terminal-based fantasy RPG written in Python. Explore dangerous regions, fight enemies, defeat powerful bosses, collect loot, purchase equipment, and save Eldoria from the Ancient Demon King.

## Features

- Four playable classes:
  - Warrior
  - Mage
  - Archer
  - Assassin
- Turn-based combat system
- Normal enemies and boss battles
- Level progression up to Level 100
- Experience, gold, score, and stat progression
- Unlockable skills
- Weapons and armor with different rarity ranks
- Health, mana, and buff potions
- Multiple regions to explore
- Loot drops after battles
- Shop for weapons, armor, and potions
- Inventory management
- Save and load functionality
- Final victory screen with game statistics

## Requirements

- Python 3.8 or newer
- No external packages are required

The game uses only Python's standard library modules:

- `json`
- `random`
- `time`
- `os`

## Installation

Clone the repository:

```bash
git clone https://github.com/Nadish001/Legends-of-Eldoria-terminal-based-game-.git
cd Legends-of-Eldoria-terminal-based-game-
```

## Running the Game

The main game file is named `Game .py`, including a space before `.py`.

Run it with:

```bash
python "Game .py"
```

On some systems, you may need to use:

```bash
python3 "Game .py"
```

## How to Play

When the game starts, choose one of the following options:

1. New Game
2. Continue
3. Instructions
4. Exit

When creating a character, enter a name and choose a class.

## Character Classes

### Warrior

A durable melee fighter with high health and defense.

- High HP
- Strong defense
- Moderate attack
- Lower mana and critical chance

### Mage

A powerful spellcaster with high mana and strong skill damage.

- High mana
- Powerful skills
- Moderate attack
- Lower defense

### Archer

A balanced ranged fighter with good attack and critical chance.

- Balanced health and mana
- Good critical chance
- Reliable attack and defense

### Assassin

A fast, high-damage class focused on critical hits and burst damage.

- High attack
- Very high critical chance
- Low defense and health
- Includes an Instant Kill skill at higher levels

## Combat

During battle, you can choose from the following actions:

1. **Attack**  
   Deal physical damage to the enemy.

2. **Skills**  
   Use an unlocked skill by spending mana.

3. **Heal**  
   Restore some health.

4. **Use Potion**  
   Use a health, mana, mixed, or buff potion.

5. **Defend**  
   Reduce incoming damage for the next enemy attack.

6. **Inventory**  
   View equipment, use potions, unequip items, or drop items.

7. **View Stats**  
   Display your current character statistics.

8. **Run**  
   Attempt to escape from a normal battle. Boss battles cannot be escaped.

## Skills

Skills unlock automatically as your character levels up.

Each skill has:

- A name
- A mana cost
- A power value
- An effect
- An unlock level

Skill effects include:

- Direct damage
- Healing
- Mana restoration
- Instant-kill attempts

## Regions

The game includes the following regions:

1. Village
2. Forest
3. Cave
4. Desert
5. Ruins
6. Castle
7. Volcano
8. Frozen Mountain
9. Sky Temple
10. Demon Realm

New regions become available after defeating the appropriate boss.

## Boss Battles

A boss appears at every tenth level. Defeating a boss:

- Grants additional experience and gold
- Increases your score
- Counts toward your boss total
- Unlocks the next region
- Provides a guaranteed high-rarity reward

The final objective is to reach Level 100 and defeat the Ancient Demon King.

## Equipment

### Weapons

Weapons improve:

- Attack damage
- Critical-hit chance

Weapons are divided into the following ranks:

- Common
- Uncommon
- Rare
- Super Rare
- Epic
- Mythical
- Legendary

### Armor

Armor improves:

- Defense
- Maximum HP
- Maximum mana
- Critical resistance

Higher-level equipment requires a higher player level.

## Potions

The game includes several potion categories:

- Health potions
- Mana potions
- Mixed health and mana elixirs
- Strength tonics
- Defense tonics
- Critical-hit tonics

Buff potions provide temporary bonuses during combat.

## Shop

The shop allows you to purchase:

- Weapons
- Armor
- Potions

You can also sell items from your inventory for gold.

## Saving and Loading

Select **Save Game** from the main menu to save your progress.

The save file is stored as:

```text
savegame.json
```

The save file may contain:

- Player name and class
- Level and experience
- Health and mana
- Equipment
- Inventory
- Potions
- Defeated enemies and bosses
- Unlocked regions
- Active buffs
- Score
- Elapsed play time

Do not manually edit `savegame.json` unless you know how the save data is structured.

## Project Structure

```text
.
├── Game .py
├── README.md
└── savegame.json        # Created automatically after saving
```

## Development

To check the file for syntax errors without starting the game, run:

```bash
python -m py_compile "Game .py"
```

To remove the generated Python cache directory, use:

```bash
rm -rf __pycache__
```

On Windows PowerShell:

```powershell
Remove-Item -Recurse -Force __pycache__
```

## Troubleshooting

### Python command not found

Install Python from [python.org](https://www.python.org/downloads/) and ensure it is added to your system PATH.

### Save file not found

The game displays a message when no `savegame.json` file exists. Start a new game and save your progress before selecting **Continue**.

### The game does not start

Make sure to include quotation marks around the filename because it contains a space:

```bash
python "Game .py"
```

## Contributing

Contributions are welcome. You can improve the game by adding:

- New character classes
- Additional enemies and bosses
- More regions
- New weapons and armor
- More skills and potion effects
- Automated tests
- A cleaner user interface
- Improved save-file validation

When contributing, please test the game before submitting changes.

## License

No license has currently been specified for this project.
