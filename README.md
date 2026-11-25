# Program

**A computer-science themed base ruleset for [Unciv](https://github.com/yairm210/Unciv).**

Choose a programming language as your civilization and guide it from the first `Hello World`
to **Future Tech**. Along the way you will research data structures, operating systems,
processor architecture, networking, AI and quantum computing — and turn all of it into
units, buildings and improvements on the map.

> [!NOTE]
> This is a **base ruleset** mod (`"isBaseRuleset": true`). It replaces the vanilla ruleset
> entirely, including the tech tree, units, buildings, terrains, nations and policies.

## Status

- Developed and validated against **Unciv 5.0.0**.
- The ruleset passes Unciv's built-in mod checker (`java -jar Unciv.jar mod-ci`) with no errors.
- Languages: English content, Simplified Chinese translation included.

## Contents

| Content | Count | Notes |
| --- | --- | --- |
| Eras | 5 | Stage I–V |
| Technologies | 96 | 15 columns, from `Hello World` to the repeatable **Future Tech** |
| Playable nations | 4 | C++, Java, Python, C# |
| Unit types | 7 | Number, Character, Function, Object, Network and two civilian types |
| Units | 19 | Civilian, melee, ranged, siege, armored and naval lines |
| Buildings | 26 | Software applications, including 3 World Wonders, 2 National Wonders and 3 civilization-specific buildings |
| Policies | 4 branches / 20 policies | **Algorithm**, **Frontend**, **Backend** and **Agent**, 5 policies each |
| Resources | 6 | 3 Bonus, 3 Luxury |
| Terrains | 7 base + 3 features | Land, water, hills, mountains, GPU plains and features |
| Promotions | 10 | Memory access, Overclock and Bandwidth lines, plus the barbarian water-unit restriction |
| Difficulties | 5 | Freshman → Developer |
| Victory types | 1 | Domination |

## Nations

| Nation | Leader | Unique ability | Unique assets |
| --- | --- | --- | --- |
| **C++** | Bjarne Stroustrup | *Memory management* — +1 Gold and +2 Production in cities on RAM tiles; free STL in every city after discovering Pointer | **STL** (replaces Database), **Smart Pointer** (replaces Array-variables) |
| **Java** | James Gosling | *Write once, run anywhere* — units ignore terrain costs when moving into Hills | **JVM** (settler), **ArrayList** (replaces Vector) — two unique units |
| **Python** | Guido van Rossum | *Batteries included* — +15% Science in all cities; free Jupyter in every city after discovering Sequential Structure | **Jupyter** (replaces Notebook), **Generator** (replaces Recursion) |
| **C#** | Microsoft | *Managed code* — +10% Production in all cities; new Object units start with 15 XP | **CLR** (replaces Virtual Machine), **Delegate** (replaces Recursion) |

Every civilization's city list is named after that language's most common libraries and
frameworks. A **Spectator** nation is included for multiplayer observation, and a
**Barbarians** nation is included for the standard barbarian gameplay.

## Buildings

All buildings represent software: applications, kernels, operating systems, developer
tools or famous websites. Most of them require a technology, and wonders are unique
software projects:

- **World Wonders**: **Luogu** (online judge), **Linux** (operating system) and
  **ChatGPT** (conversational AI).
- **National Wonders**: **Kernel** (capital) and **VScode** (code editor).
- **Technology-linked buildings**: **Blender** (computer graphics) and **TensorFlow**
  (machine learning).
- **Civilization-specific buildings** replace a generic building for their civilization:
  **STL** for C++, **Jupyter** for Python and **CLR** for C#.

Each civilization follows the mod's design rule of either one unique unit plus one
unique building, or two unique units: Java has two unique units and no unique building.

## Units

Land combat units follow the four language primitives: **Number** (melee), **Character**
(ranged), **Function** (siege) and **Object** (armored). Water combat units belong to the
**Network** type and represent network services: **Server** (melee) and **Client** (ranged).
**Worker**, **Compiler** and **Subscriber** are the civilian units.

Civilization-specific units are language constructs: **Smart Pointer** for C++, **JVM** and
**ArrayList** for Java, **Generator** for Python and **Delegate** for C#.

## Eras and the tech tree

The tech tree has **96 technologies in 15 columns**, three columns per stage:

| Stage | Chinese name | Theme |
| --- | --- | --- |
| Stage I | 似懂非懂 | Mathematical foundations, programming frameworks and basic concepts |
| Stage II | 初现端倪 | Data structures, algorithms and digital design |
| Stage III | 渐入佳境 | Computer networks, object orientation and computer architecture |
| Stage IV | 大彻大悟 | Parallel computing, IoT, blockchain and large models |
| Stage V | 炉火纯青 | Frontier computing theory and technology |

Every branch converges on the final, repeatable **Future Tech**. Each technology column
unlocks a consistent set of units, buildings, improvements or bonuses. A few milestones
matter early:

- **Website** enables embarkation for land units and opens the **Frontend** policy branch.
  You cannot cross water before it.
- **Pointer** unlocks Roads, the Database building and +1 Production on RAM tiles.
- **Basic Algorithm** opens the **Algorithm** policy branch.
- **Operating System** opens the **Backend** policy branch.
- **Artificial Intelligence** opens the **Agent** policy branch.
- **Computer Graphics**, **Machine Learning** and **Artificial Intelligence** unlock
  Blender, TensorFlow and ChatGPT respectively.

## Policies

There are four policy trees, each with exactly five policies (four regular policies and
one finisher). Each tree is themed around a development domain and its structure mirrors
a classic Civ V tree:

- **Algorithm** (Tradition-like) — algorithms and optimization.
- **Frontend** (Liberty-like) — browser and UI development.
- **Backend** (Honor-like) — servers, APIs and databases.
- **Agent** (Commerce-like) — prompt engineering, tool use and multi-agent systems.

## The world

The map is built from computer hardware instead of terrain:

| Terrain | Civ V analogue | Role |
| --- | --- | --- |
| Cache | Grassland | Fertile flat land |
| RAM | Plains | Flat land with Production; DDR4/DDR5 deposits |
| GPU | Plains | Flat land; units move at double speed here |
| Hard-drive | Hill | Rough elevated land; cities gain defensive strength |
| System occupancy | Mountain | Impassable mountain-like terrain with turn damage |
| Mobile-storage | Coast | Coastal water; preferred water start locations |
| Cloud-storage | Ocean | Deep water |
| Worn-Hard-drive | Marsh | Rare, unbuildable low-yield feature on Hard-drive |
| Encrypted-Hard-drive | Forest | Rough, defensive feature on Hard-drive |
| 404 | Ice | Rare, impassable cold-water feature |

Resources and their improvements:

- **DDR4 / DDR5** (Bonus, RAM) → **Program**
- **SanDisk** (Bonus, Hard-drive) → **HDD-box**
- **Cloud-storage-VIP** (Luxury, Cloud-storage) → **Account**
- **Office / Photoshop** (Luxury, Hard-drive) → **Project**

The **Worker** builds land improvements and Roads. The **Subscriber** is the water worker
that builds **Account** on Cloud-storage — it becomes available with the Internet technology.

## Installation

1. Copy this folder into the `mods` directory used by your Unciv installation
   (on desktop this is next to `Unciv.jar`).
2. Start Unciv, open **Mods**, and enable **Program**.
3. Start a new game and select the mod. Because it is a base ruleset, the mod's nations,
   tech tree and rules replace the vanilla ones.

## Development

The mod follows the standard Unciv mod layout:

```
Images/                 icons and tile art (packed into game.atlas)
jsons/                  ruleset definitions
  translations/         mod translations
fonts/                  optional fonts
game.atlas, game.png    packed image atlases
```

To validate the ruleset after editing, run the mod checker **from the mod folder**
(the checker loads `jsons/` from the current directory and also repacks `Images/`):

```bash
cd "path/to/mods/Program"
java -jar "path/to/Unciv.jar" mod-ci
```

A non-zero exit code means there is at least one error. Warnings and `OK` notes are
listed in the output as well. See the Unciv documentation under
`docs/Modders/` for the full JSON reference.

### Editing notes

- Building and wonder costs are derived automatically from the `buildingCost` /
  `wonderCost` of the technology column if a building has no explicit `cost`.
- Units and buildings should reference technologies that exist; promotions used by a
  unit type must list that type in `unitTypes`.
- Terrain features need a generation unique (`Occurs in groups around high elevations`,
  `Rare feature`, `Vegetation`, or `Occurs at temperature between …`) to appear on
  generated maps.
- `game.atlas` and `game.png` are generated by the image packer. Re-run `mod-ci` (or
  pack images from the game) after adding or changing files under `Images/`.

## Roadmap / known limitations

- Only the Domination victory is implemented. Scientific, Cultural and Diplomatic
  victories are not available.
- More programming-language nations (JavaScript, Rust, Go, …) would need new nation icons.
- `Encrypted-Hard-drive`, `GPU`, `404`, `ChatGPT`, `Blender`, `TensorFlow`, the
  **Frontend / Backend / Agent** policy icons, the civilization-specific buildings/units
  and the two Network units currently use tinted variants of existing art as placeholders;
  dedicated artwork is welcome.
- Quotes for the newly added Stage IV / Stage V technologies are English-only at present;
  the older technologies and all building names are translated.
- Religion, Great People, espionage and city-state quests are not customized.

## Contributing

Anyone can contribute. Please keep the ruleset valid by running the mod checker before
opening a pull request, and include a translation entry for any new player-facing text
in `jsons/translations/Simplified_Chinese.properties`.

## Credits

- [Unciv](https://github.com/yairm210/Unciv) — the game and modding API.
- HexaRealm tileset — base tile art used by the mod's terrain set.
- JetBrains Mono and YaHei Consolas Hybrid — bundled font files.
- All named programming languages and their creators belong to their respective owners;
  this mod is an educational fan project.
