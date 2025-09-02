Ants vs. SomeBees (Python)
A tower-defense simulation in Python inspired by Plants vs. Zombies. As the ant queen, you deploy different ant types to stop invading bees moving through linked tunnels. The project emphasizes object-oriented design, class hierarchies, and stateful simulation.

🧠 Concepts & Topics Used
Object-Oriented Programming (OOP): classes, inheritance, method overriding, class vs. instance attributes
Polymorphism & Composition: Insect → Ant/Bee; container ants wrap other ants (BodyguardAnt, TankAnt)
State Machines: turn-based simulation loop; cooldown timers (e.g., HungryAnt chewing), reflective damage (FireAnt)
Linked Structures / Graphs: Place nodes linked by exit/entrance pointers (bees traverse a tunnel)
Search/Traversal Patterns: “nearest bee” lookup walks along entrance links (bounded for ShortThrower/LongThrower)
Resource Management: food costs per ant; deployment strategy
Game/GUI Integration: simple web GUI served from gui.py using static/ assets and templates/


🌳 Class Hierarchy (Overview)
Insect (base)
├── Ant
│   ├── HarvesterAnt
│   ├── ThrowerAnt
│   │   ├── ShortThrower
│   │   ├── LongThrower
│   │   └── ScubaThrower
│   ├── FireAnt
│   ├── WallAnt
│   ├── HungryAnt
│   ├── ContainerAnt
│   │   ├── BodyguardAnt
│   │   └── TankAnt
│   └── QueenAnt
└── Bee

World / Layout
GameState
├── Places (linked like a tunnel)
│   ├── Place (entrance ⇄ exit)
│   ├── Water (special Place)
│   ├── Hive (bee source)
│   └── AntHomeBase (lose when a bee reaches here)
└── Ant roster, Bee waves, time, food

📁 Project Structure
ants.py           # main game logic 
ants_plans.py     # difficulty presets
gui.py            # runs the GUI 
static/           # images & GUI assets 
templates/        # HTML templates for GUI





# Editors/OS
.vscode/



