# 🌿 Ecosystem: Packs, Hunting, and Disease

🧬 A living world in a single HTML file: a true drama of survival unfolds on Canvas. Plants grow, herbivores flock, predators stalk prey, and disease can change the balance of the entire ecosystem in seconds.

## 🦁 Who Lives in the World

- 🌱 **Plants** are the basis of the food chain and are constantly replenished.
- 🐐 **Herbivores** are in packs, escape predators, and reproduce when energy levels are sufficient.
- 🐅 **Hunters** are fast and aggressive, pursuing herbivores and omnivores.
- 🕷 **Ambushers** are slow but powerful; they prefer to lie in wait. - 🦝 **Omnivores** — flexible: they eat both plants and other creatures; they flee from large predators.
- 🦠 **Disease** — a random infection, transmitted through close contact, reduces speed and accelerates energy expenditure.
 
## ⚡ Key Mechanics

- **Boys**: Cohesion, alignment, and collision avoidance—the swarm moves as a single unit.
- **Food Chains**: Each species has its own list of acceptable prey.
- **Population Dynamics**: Energy, hunger, reproduction, and death all affect balance.
- **Diseases**: Purple borders indicate infected individuals; illness changes behavior and survival.
- **Real-time Statistics**: Species and disease counters are updated every frame.

## 🎮 How to Play

1. Simply open `index.html` in any modern browser.
2. Watch the ecosystem develop.
3. Click **"Restart"** to reset the world and try new conditions.

## ⚙️ Configuration and Experimentation

All parameters are located in the CONFIG object—change them to explore different scenarios:
 
```js
const CONFIG = {
spawnRate: 0.04, // plant spawn rate
energyLoss: 0.12, // energy consumption per unit of time
eatValue: 30, // energy yield from food
reproduceEnergy: 80, // energy required for reproduction
reproduceChance: 0.3, // chance of reproduction with sufficient energy
maxPopulation: 400, // population limit
hungerThreshold: 70, // hunger threshold
fleeDistance: 90, // distance at which prey begins to flee
fleeSpeedBoost: 1.8, // acceleration when fleeing
flockRadius: 80, // radius at which individuals in a flock sense each other
flockStrength: 0.03, // force of attraction to the center of the flock
flockSeparation: 25, // distance at which individuals begin to avoid collisions
flockSeparationStrength: 0.08,
diseaseChance: 0.001, // Chance of random infection
diseaseSpreadDist: 35, // Disease transmission distance
diseaseEnergyDrain: 0.3, // Additional energy expenditure for sick individuals
diseaseSpeedMult: 0.6 // Speed multiplier for sick individuals (slowdown)
};

# 🌿 Экосистема: Стаи, охота и болезни

🧬 Живой мир в одном HTML-файле: на Canvas разворачивается настоящая драма выживания. Растения растут, травоядные сбиваются в стаи, хищники выслеживают добычу, а болезнь может за считанные секунды изменить баланс всей экосистемы.

## 🦁 Кто живёт в мире

- 🌱 **Растения** — основа пищевой цепи, постоянно восполняются.
- 🐐 **Травоядные** — держатся стаями, убегают от хищников, размножаются при достатке энергии.
- 🐅 **Охотники** — быстрые и агрессивные, преследуют травоядных и всеядных.
- 🕷 **Засадники** — медленные, но мощные; предпочитают выжидать в засаде.
- 🦝 **Всеядные** — гибкие: едят и растения, и других существ; убегают от крупных хищников.
- 🦠 **Болезнь** — случайное заражение, передаётся при близком контакте, снижает скорость и ускоряет расход энергии.

## ⚡ Ключевые механики

- **Стайное поведение (Boids)**: когезия, выравнивание и избегание столкновений — стая двигается как единое целое.
- **Цепи питания**: у каждого вида свой список допустимой добычи.
- **Динамика популяций**: энергия, голод, размножение и смерть — всё влияет на баланс.
- **Болезни**: фиолетовые ободки показывают заражённых; болезнь меняет поведение и выживаемость.
- **Статистика в реальном времени**: счётчики по видам и больным особям обновляются каждый кадр.

## 🎮 Как играть

1. Просто откройте `index.html` в любом современном браузере.
2. Наблюдайте за развитием экосистемы.
3. Нажмите **«Перезапустить»**, чтобы сбросить мир и попробовать новые условия.

## ⚙️ Настройка и эксперименты

Все параметры вынесены в объект `CONFIG` — меняйте их, чтобы исследовать разные сценарии:

```js
const CONFIG = {
    spawnRate: 0.04,           // скорость появления растений
    energyLoss: 0.12,          // расход энергии в единицу времени
    eatValue: 30,              // сколько энергии даёт еда
    reproduceEnergy: 80,       // энергия, нужная для размножения
    reproduceChance: 0.3,      // шанс размножения при достаточной энергии
    maxPopulation: 400,        // лимит популяции
    hungerThreshold: 70,       // порог голода
    fleeDistance: 90,          // дистанция, на которой жертва начинает убегать
    fleeSpeedBoost: 1.8,       // ускорение при бегстве
    flockRadius: 80,           // радиус, на котором особи чувствуют друг друга в стае
    flockStrength: 0.03,       // сила притяжения к центру стаи
    flockSeparation: 25,       // дистанция, при которой особи начинают избегать столкновений
    flockSeparationStrength: 0.08,
    diseaseChance: 0.001,      // шанс случайного заражения
    diseaseSpreadDist: 35,     // дистанция передачи болезни
    diseaseEnergyDrain: 0.3,   // дополнительный расход энергии у больных
    diseaseSpeedMult: 0.6      // множитель скорости у больных (замедление)
};
