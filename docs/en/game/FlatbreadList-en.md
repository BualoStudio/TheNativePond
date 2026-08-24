# The Native Pond Feature Roadmap

![flatbreadlist_background](/background/en/FBL-docs-bg-en.png)

> [!WARNING]
> 1. All content on this list is pie-in-the-sky — it does not represent the final presentation or actual implementation.
> 2. Some content on this list was not discussed in production team meetings.
> 3. Some content on this list has not been through a feasibility study.
> 4. This list may serve as guidance for fan works and derivative creations.
> 5. The production team reserves all rights to take further measures regarding this list, as well as the final interpretation of it.

---

## 🎮 Controls

Smooth movement and a good camera are an important part of ensuring the game is playable. **The character must be able to move!**

### Movement

- The player controls the character moving across the **map**, and at special locations (such as the fishing platform), the player **triggers** the animation of entering that **special location** by pressing a key or by moving into the special location's small coordinate coverage range.
- The player **interacts** with the game through touch buttons (mobile), keyboard (desktop) and gamepad, and the keybinds can be customised.

### Camera

- Use a **third-person** camera in non-special areas of the map.
- Use a **first-person** camera in special areas of the map (such as the fishing platform), showing the interior of that special area (if any).
- The map **moves** along with the camera.

---

## 🗺️ Map System

Crouch over the table and make a **map** — the map really has everything!

### Zoom and Orientation

- The map cannot **rotate** with the camera.
- The map can be **zoomed**.
- The map follows the orientation logic of "**north at the top, south at the bottom, west on the left, east on the right**".

### Borders

- The game map has **borders**, meaning the player cannot pass through the **edge of the map**.
- When the player tries to cross the border, the game will **pull the player back** by force and show the message "* A familiar feeling wells up — you seem to hear: 'Let's explore the area ahead of us later!' Although you know you'll never be able to explore it later, you still want to give it a try."
- The borders may be obvious **natural obstacles** (such as great mountains), or **man-made fences** (such as the walls of Huizhou-style architecture).

### Weather

- The **kinds** of weather are as follows:
	- Sunny.
	- Rain.
	- Thunderstorm.
	- Snow.
- Weather **changes** may be decided by:
	1. Manual adjustment by the player.
	2. Similarity to the climate characteristics of a certain place.
	3. Completely random probability.

### Seasons

- Seasons switch every **90 hours**.
- The **kinds** of seasons are as follows:
	- Spring.
	- Summer.
	- Autumn.
	- Winter.

### Camera

- The player can take **photos** at any location (except GUI screens) by pressing a keyboard key, clicking a button, or pressing a controller key.
- When **taking a photo**, the game will display a full-screen **white flash** to represent the photograph. This may require adding a **photosensitive epilepsy** warning screen at the game's startup screen.
- When **taking a photo**, the game will automatically **capture** all elements on screen (except GUI elements) and add a **photo frame**.
- The game will **save** the photos to the **designated folder** for sharing.

### Fishing Pond

- The fishing pond is the game's most central special area, comprising the **fishing platform**, the **pond** and the **little boat**.

#### Fishing Platform

- Located at the **southernmost** end of the pond.
- When the player **enters** this special area, the camera automatically zooms in and switches to a first-person view, the character enters a seated state, and the visual interface of this special area is shown.
- The fishing platform is used for **fishing**.

#### Pond

- Located at the **northernmost** end of the map.
- When the player **enters** this special area, the character enters a **swimming** state.

#### Little Boat

- Located at **any position** in the pond (determined by where the player last parked the boat).
- When the player **enters** this special area, the character enters a **driving** state, and the visual interface of this special area is shown.
- The player can drive the little boat to sail across the **pond**.

### Tent

- Located to the **southwest** of the centre of the map.
- When the player **enters** this special area, the camera automatically zooms in and switches to a first-person view, and the visual interface of this special area is shown.
- The tent is the core of the **camp**.
- The tent's **interior** and **size** may reference the design of the tent in *Robinson Crusoe*.

### Farmland

- The farmland is located to the **southeast** of the tent.
- When the player **enters** this special area, the camera automatically zooms in and switches to a first-person view, and the visual interface of this special area is shown.
- The farmland is used for **planting**.

### Market

- The market is located in the **east** of the map.
- When the player **enters** this special area, the camera automatically zooms in and switches to a first-person view, and the visual interface of this special area is shown.
- The market is used for **trading**.

### Tree

- Located to the **southeast** of the tent.
- When the player **enters** this special area, the camera automatically zooms in and switches to a first-person view, and the character enters a seated state.
- **Apples** sometimes appear on the tree (e.g. in autumn). The player can knock them down with a **long wooden stick** and **collect** them.
- When the player stays under the **tree** for a while (about 1 minute), the game shows a floating button "Hold [W] to meditate". When the player presses W, clicks the button, or presses a controller key, the player enters **meditation**. While the player is **meditating**, the game displays full-screen **visual effects** (various physics formulas), and there is a chance of being hit by an **apple**.

### Campfire

- Located not far to the **east** of the tent.
- When the player **enters** this special area, the camera automatically zooms in and switches to a first-person view, and the visual interface of this special area is shown.
- The campfire can be **lit** and provides light.
- The campfire can be used for **cooking**.

### Magic Conch

- The player can pick up the **Magic Conch** on the **beach** by the water.
- When the player **picks up** the Magic Conch, the character enters a blowing state and the camera automatically zooms in. During this time the player cannot move. The visual interface of this special item is shown at the same time.
- The Magic Conch has 7 **notes** the player can blow.
- The Magic Conch has multiple **variants**, and different variants have different **timbres**.

### Mailbox

- Located to the **south** of the tent.
- When the player **enters** this special area, the camera automatically zooms in and switches to a first-person view, and the visual interface of this special area is shown.
- The mailbox is used for **sending and receiving mail**.

---

## 🎣 Fishing System

At the **fishing platform**, the player can fish using the **fishing rod**.

### Species

- The game's **fishing pond** can catch both **saltwater fish species** and **freshwater fish species**. Apart from fish, **collectibles** can also be caught.
	1. This may be determined by the **fishing platform** the player chooses (for example, a platform by the seaside can only catch saltwater species, while a platform by a lake can only catch freshwater species).
	2. This may be determined by the **probability** of catching each species (that is, at the same seaside platform, both saltwater and freshwater species can be caught according to probability).
- The **probability** of catching each species may be decided by:
	1. The probability of catching each species in **real life**. This may be a range of values, adjusted according to various factors (such as weather and seasons) rather than being fixed.
	2. A completely **random** probability.
- The **probability** of catching collectibles may be decided by:
	1. The player's historical **bite rate**.
	2. A random **probability** within a fixed range.
	3. A completely **random** probability.

### Bite Rate

It is worth mentioning that the bite rate refers to the probability of a fish **taking the hook**, not the probability of finally catching the fish.

- The game's **bite rate** is jointly decided by the following factors:
	- Whether there is bait on the player's hook.
	- Whether the player has applied groundbait.
	- The kind of bait on the hook.
	- Game time (such as day or night).
	- Whether the headlamp is switched on at night.
	- Game weather.
	- Game season.
- The bite rate in the game may also be decided by:
	1. The player's historical bite rate.
	2. A completely random probability.

### Catch Rate

As the name suggests, the catch rate refers to the probability of finally catching the fish.

- The game's **catch rate** is jointly decided by the following factors:
	- Whether the fish has taken the hook.
	- The timing of the player lifting the rod (neither too early nor too late).
	- The breaking rate of the fishing line.
	- The size of the hook.

### Fishing Rod

- The fishing rod is composed of the **rod**, the **float**, the **hook** and the **line**.
- Every part of the fishing rod has **durability**. The lower the durability, the higher the chance of the rod breaking. When the rod breaks, the broken part needs to be **replaced**.

#### Rod

- The **rod** is a component of the **fishing rod**.
- The player can purchase rods through the **trade system**, such as a 2.7-metre rod and a 3.6-metre rod.
- Rods of different lengths have different casting and lifting times.

#### Float

- The **float** is a component of the **fishing rod**. The player can decide whether to lift the rod based on the **movement of the float**.
- The player can purchase floats through the **trade system**, such as an ordinary float and a glow-in-the-dark float.
- The float movement when different fish species take the hook is different, referenced from the float movement of real fish taking the hook.
- The number of "marks" on the float can be adjusted (that is, by adjusting the weight of the lead) to make it easier for the player to observe.

#### Hook

- The **hook** is a component of the **fishing rod** and the foundation for catching fish.
- The player can purchase hooks through the **trade system**, such as small hooks and large hooks.
- The size of the hook is the decisive factor in whether the player can catch big or small fish.
- The hook can be baited.

#### Line

- The **line** is a component of the **fishing rod**.
- The player can purchase lines through the **trade system**, such as an ordinary 0.8 line and a premium 2.0 line.
- Different lines have different **breaking rates**, which may be jointly decided by the following factors:
	- The quality of the line.
	- The usage time or durability of the line.

### Bait

- The player can purchase bait through the **trade system**, such as ordinary bait and red earthworms.
- If the purchased bait is powdered, the powdered bait needs to be made into bait by adding water, kneading the dough, and so on.
- Different baits have different **bite rates**.
- As a consumable, when the player has no bait and the shells they own (including shells gained from selling catches) are not enough to buy a pack of bait, the game will deliver a free supply to the **mailbox** the next day.

### Groundbait

- The player can purchase groundbait through the **trade system**, such as fermented bean dregs and old corn soaked in wine.
- Different groundbait has different **bite rates**.
- Groundbait can greatly increase the bite rate.

### Headlamp

- The player can purchase headlamps through the **trade system**, such as an ordinary headlamp and a blue-light night fishing lamp.
- Different headlamps have different **bite rates** and different visual effects.
- At night, the headlamp lets the player see the water surface and the float.
- At night, the headlamp may disturb the fish and lower the bite rate.

### Collectibles

- Collectibles are mainly divided into **drift bottles**, **souvenirs** and **story fragments**.
- The player can **obtain** collectibles through the following channels:
	- Fishing.
	- Gifts from Cat.

#### Drift Bottles

- Drift bottles contain **letters**.
- Most letters are **chicken soup for the soul** to encourage the player.

#### Souvenirs

- Some souvenirs can be **displayed** in the **tent**.

#### Story Fragments

- Story fragments can guide the player to learn about the **villagers'** stories.
- When all story fragments are collected, the player can unlock a long story to fully and thoroughly understand the **villagers'** stories.

---

## 🍳 Cooking System

Make **food** and try eating it!

### Cooking Utensils

- The cooking utensils consist of three parts: the **stove**, the **chopping board** and the **cookware**.

#### Stove

- The stove is used for **heating** food.
- The stove may be **located**:
	1. Inside the tent.
	2. Outside the tent but close to it.
- The stove allows the player to place some **cookware** (such as a frying pan).
- Fuel must be added to the stove before use.
- The player needs to **control the heat** to ensure the food made is edible.

#### Chopping Board

- The chopping board is used for **chopping** food.
- The chopping board allows the player to place some **ingredients** (such as Chinese cabbage) and **semi-finished foods**.
- The player can use some **cookware** (such as a kitchen knife) to cut on the chopping board.

#### Cookware

- Cookware allows the player to conveniently **process** ingredients.
- Cookware includes:
	- A large pot.
	- A frying pan.
	- A steaming rack.
	- Porcelain bowls.
	- A kitchen knife.
	- A rolling pin.

### Recipes

- The player can make food according to **recipes**. Generally speaking, as long as the player follows the recipe, the food will be made successfully.
- The player can also **ignore** the recipe and improvise.

### Food

- When the player completes the entire **food-making process**, they will obtain **food**.
- The player can make the following foods:
	- Plain noodles (obtained through the whole process from flour, kneading the dough, cutting the strips, to boiling them in the pot).
	- Steamed buns (obtained through the whole process from flour, kneading the dough, rolling out the wrappers, making the filling, wrapping the buns, to steaming them).
	- Fried egg (obtained through the whole process from cracking the egg, lighting the fire, to flipping it).
	- Grilled fish (obtained by grilling fish at the campfire).
	- Indescribable thing (obtained when food-making fails).
	- Charcoal (obtained when making food without following a recipe and failing).

### Eating

- After the player makes **food**, they can try eating it.
- When eating, the player can click on the **food** or the **components of the food** to eat it.
- When the player eats **food**, there will be a comfortable **sound effect**, healing **text**, and the food or its components will **disappear** through an animation to represent eating.
- In particular, when the player eats an **indescribable thing**, the following may occur with a certain probability:
	1. The character faints and wakes up after a while.
	2. The character has a nauseating visual effect for a period of time.
	3. Nothing happens.

---

## ⛺️ Camp System

Only the **tent** can bring a sense of security!

### Storage

- In the **tent**, the player can view the **items** they own.
- The **items** the player **owns** include:
	- Fish.
	- Collectibles.
	- Fishing gear.
	- Crops.
- Some items (such as some collectibles) can be **displayed**.

### Achievements

- In the **tent**, the player can view the **achievements** they have earned.

### Bed

- During **sunset** and **night**, the player can **sleep** by clicking the bed to skip the night.
- The player will wake up at the next day's **sunrise** or **morning**, or may choose to **sleep a little longer** and keep sleeping.

### Emotion Recycling Bin

- This recycling bin, similar to a recyclable trash bin, allows the player to write down unhappy things they encounter in **real life**, then crumple them into a ball and throw them into the emotion recycling bin!

### Diary

- The player can write down what happens each day in the **diary** (whether in-game or in real life).
- The game allows the player to export **specific pages** of the **diary** to the **designated folder** for sharing.

### Album

- The album will display all the **works** the player has drawn on **drawing paper**.
- The album can be exported entirely as a single file to the **designated folder** for sharing.

---

## 🐚 Trade System

Is this melon ripe?

### Purchasing

- The player can buy goods at the **market**.
- At the market, the player can talk to **villagers** of various professions.
- When the player **talks** to villagers, there is a chance of triggering **special storylines**; after completing them, the price can be **reduced**.
- The player can buy the following **kinds** of goods at the market:
	- Fishing gear (such as fishing rods).
	- Crop seeds (such as wheat seeds).
	- Processed crops (such as flour).
	- Vegetables (such as Chinese cabbage).
	- Fuel (such as charcoal).
	- Seasonings (such as salt).
	- Drawing paper (such as 1:1 drawing paper).
	- Stamps.

### Selling

- The player can sell goods at the **market**.
- The player can sell the following **kinds** of goods at the market:
	- Fish.
	- Some collectibles.
- When selling fish, the **today's fish price** will be used as the pricing standard.
- **Today's fish price** is divided into **fresh fish** and **stocked fish** prices; neither price stays the same forever, and today's fish price may be jointly decided by the following factors:
	- Game weather.
	- Game season.
	- A random value within a fixed range.

### Currency

- The game uses **shells** as currency.
- The player can **obtain** shells through the following channels:
	- Trading.
	- Fishing them up.
	- Gifts from Cat.

---

## 🌽 Crop System

**Plant crops**, **water and fertilise**, and **harvest**.

### Planting

- Planting crops requires **crop seeds**.
- The **process** of planting is as follows: levelling the soil, sowing the seeds, covering with soil, watering, fertilising.
- The conditions for seeds to germinate: **adequate moisture**, **suitable temperature** and **sufficient oxygen**.
- When planting, the player needs to **consider**:
	- Game weather.
	- Game season.

### Growth

- During crop growth, the player must keep **watering** and **fertilising** without interruption.
- Crops **switch** their **growth state** every period of time (about 90 hours).

### Harvest

- When crops are **fully mature**, the player can harvest the **crops** and **crop seeds**.

---

## 🐱 CatGPT

**Chat** with the little cat or **pet** it ฅ՞•ﻌ•՞ฅ.

### Chatting

- The player can **send messages** to Cat.
- Cat will **reply** to the player according to certain weights, which may be decided by:
	1. The number of characters the player sends.
	2. A completely random probability.
- Cat will reply with "**Meow**" in various tones and timbres to provide emotional value to the player.

### Petting

- The player can pet Cat by gently touching its **head**.
- When petting, "**Meow**" bullet comments will fly out from Cat, accompanied by "**Meow**" in various tones and timbres to provide emotional value to the player.

### Gifts

- Cat may give the player a **gift** when the player wakes up the next morning.
- Whether Cat gives the player a **gift** may be decided by:
	1. The number of times the player chatted with or petted Cat yesterday.
	2. The total number of times the player has chatted with or petted Cat historically.
	3. A completely random probability.
- The **kinds** of gifts may include:
	- Fish.
	- Shells.
	- Some collectibles (extremely rare).

### And More…

- Apart from Cat, the player can also choose **other objects** to talk to or pet. These **other objects** may be **production team members** appearing in the **introductory storyline**.

---

## 🖌️ Drawing System

**Paint** with incredibly realistic paper and paints, and save.

### Drawing Paper

- Drawing paper is no different from real paper, allowing **bleeding**, **re-colouring** and **colour mixing**.
- The player can purchase drawing paper through the **trade system**, such as 1:1 paper and 3:4 paper.

### Palette

- 8 basic colours are provided by default. The player can dip the **brush** into the paints and mix colours on the **palette**.
- The mixing scheme may be **watercolour** or **gouache**.
- When mixing, the paints of two colours are blended with the **brush**; unmixed paint will remain its original colour, and the mixed colour will be determined by how much the player mixes.

### Brush

- The brush can apply paint or water onto the drawing paper.

### Saving

- The works the player draws will be **saved** in the **album**.
- The player can **export** the works to the **designated folder** for sharing.

---

## 📬 Mailbox System

Send and receive **mail**.

### Receiving

- The player may **receive** the following mail:
	- Letters the player sent to themselves.
	- Free bait supplies.
	- Festival greetings.
	- Birthday greetings.

### Sending

- The player can **send** the following mail:
	- Letters to their future self.
- When sending, a **stamp** must be affixed to the mail.

---

## 📺 Visual Interface

Smooth **non-linear animations** always bring players a good visual experience.

### Controls

- Controls can **trigger** interaction behaviours and events.
- Controls should maintain the same design style as *Today@PolarBay*.
- Controls should shrink instantly when **pressed**, then bounce back non-linearly.
- Controls can have customisable **positions** and **sizes**.

### Cards

- Cards cannot be **interacted with**.
- Cards should maintain the same design style as *Today@PolarBay*.
- Cards are used to display relatively **clean** backgrounds, such as the backpack interface.

### Eye-care Green Screen

- Because the player must **stare at** the **float** for a **long time** while **fishing**, a special **eye-care green screen** has been designed.
- The eye-care green screen will **cover the full screen** at intervals to **force the player to rest**.
- The **interval time** and **coverage time** of the eye-care green screen can be adjusted or toggled in the settings.
- The eye-care green screen will display the content of the **letters** from the **drift bottles** the player has collected.

### Colour Schemes

- The game may come with **two** colour schemes built in: a white theme and a black theme.
- The white theme and black theme may **switch** according to the following conditions:
	1. Day and night conditions in real life.
	2. Day and night conditions in the game.
	3. Manual adjustment by the player in the settings interface.

### Particle Effects

- Particle effects are produced by **special events**, such as a boat sailing on the water.
- The number of particle effects can be adjusted or toggled in the **settings** to avoid performance issues.

### Advanced Materials

- Advanced materials, i.e. **acrylic** materials.
- The player can enable or disable advanced materials in the **settings**.
- When advanced materials are enabled, the **blank areas** of the player's controls, cards and other GUI elements will become translucent frosted materials.

---

## 🕒 Time System

**Time** always flies by so fast that we miss many things.

### Time Conversion

- **One day** in the game is **one hour** in real life.
- The conversion ratio between game time and real time is **1:24**.

### Time Periods

- Both the **daytime** and **night-time** in the game are **30 minutes**.
- Within **one day** (60 minutes), the game's time periods are divided as follows:
	- Sunrise: minutes 1–2.
	- Morning: minutes 2–10.
	- Noon: minutes 11–20.
	- Afternoon: minutes 21–28.
	- Sunset: minutes 29–30.
	- Night: minutes 31–60.

---

## 💾 Save System

**Save** the current **game progress**, so that our fish and salt are safe.

### Save

- On the **save** page, the player can click the **get save** button to **save** the current progress.
- On the **save** page, the player can click the **load save** button to **load** a saved save.
