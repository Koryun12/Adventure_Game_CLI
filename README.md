Task: Adventure Quest - CLI RPG Game
Objective:
Design and implement a fully interactive Command-Line Interface (CLI) Role-Playing Game (RPG) named "Adventure Quest", leveraging C++ concepts such as abstract classes, interfaces (pure virtual functions), dynamic polymorphism, and Run-Time Type Identification (RTTI). The game should provide an engaging experience where players explore a fantasy world, interact with various characters, engage in turn-based combat, complete quests, and manage their character's progression.

Concept Overview:
The game will use object-oriented programming principles to create a modular and extensible RPG simulation. Key C++ concepts must be applied as follows:
Abstract Class: Use an abstract base class Character to define common attributes and behaviors for all game characters (Heroes, Monsters, NPCs).
Interfaces: Implement pure abstract interfaces (Interactable, Combatable) to define specific interaction and combat behaviors that can be dynamically applied to characters.
Dynamic Polymorphism: Utilize virtual functions and raw pointer-based polymorphism to handle different types of characters, interactions, and combat scenarios dynamically.
RTTI: Employ RTTI (e.g., dynamic_cast, typeid) to identify specific character types at runtime and apply type-specific behaviors (e.g., unique dialogue or combat effects).
Manual Memory Management: Use raw pointers for dynamic memory allocation and ensure proper cleanup with destructors to avoid memory leaks.

Game Description:
"Adventure Quest" immerses the player in a fantasy world filled with heroes, monsters, and non-playable characters (NPCs). The player takes on the role of a hero who explores different locations (e.g., forests, dungeons, villages), interacts with NPCs to uncover the storyline and receive quests, and engages in turn-based battles with monsters. Choices made by the player dynamically affect the game flow, storyline progression, and character development.
Detailed Task Explanation:
Game Entities:
Hero:
The player-controlled character who can interact, fight, level up, manage an inventory, and gain new skills.
Subtypes (optional): Warrior (high health, melee-focused), Mage (magic-focused, ranged attacks), Rogue (stealth and critical hits).
Attributes: Health, attack power, defense, experience points (XP), level, inventory (items like potions, weapons), and skills/spells.
Monster:
Hostile entities that the hero encounters and battles.
Subtypes: Goblin (weak but fast), Troll (high health, slow), Dragon (strong, with special abilities like fire breath).
Attributes: Health, attack power, defense, special abilities (e.g., poison attack, area damage).
NPC:
Non-hostile characters that provide story elements, quests, or items.
Subtypes: Villager (provides quests), Merchant (sells items), Healer (restores health).
Attributes: Name, dialogue, associated quest or items.
Gameplay Mechanics:
Exploration:
The game world consists of multiple textual environments (e.g., "Enchanted Forest", "Dark Dungeon", "Quiet Village").
Players navigate between locations via a CLI menu (e.g., "1. Move to Forest", "2. Move to Village").
Each location contains unique encounters (e.g., meeting an NPC, finding an item, or encountering a monster).
Interactions:
Players can interact with NPCs and certain objects (e.g., treasure chests) using textual prompts.
Use RTTI to vary interactions based on character types (e.g., a Merchant NPC might offer different dialogue to a Warrior than to a Mage).
Example Interaction: Talking to a Villager NPC might yield a quest like "Slay the Troll in the Dark Dungeon."
Combat:
Combat is turn-based, with the player selecting actions (e.g., "Attack", "Use Skill", "Defend", "Use Item") via a CLI menu.
    Use dynamic polymorphism to handle combat between heroes and monsters, allowing for diverse behaviors (e.g., a Troll might have a chance to counterattack).
RTTI can be used to apply type-specific effects (e.g., a Mage's spell deals bonus damage to a Dragon).
