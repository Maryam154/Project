# 🧱 Block Craft Game

## 🎮 Game Controls & Mechanics

When you run the game, the player can move freely in any direction using the keys defined in the **Godot Input Map** (e.g., arrow keys(left, right, up, down)). This gives full control over movement across the game world.

* **Right Click** – Adds a block to your inventory by collecting it from the world.
* **Left Click** – Removes the selected block from your inventory and places it into the world.
* **P Key** – Switches to the **previous block** in your inventory.
* **N Key** – Switches to the **next block** in your inventory.

## 🛠️ Crafting System

Press **S** to open the crafting interface, which appears on the **right side of the screen**. This shows available recipes for crafting new blocks from collected items.

* Use **[** (left square bracket) to move to the **previous recipe**.
* Use **]** (right square bracket) to move to the **next recipe**.

Once you stop switching recipes, the current one becomes selected for crafting.

### ✅ Crafting a Block

After selecting a recipe and collecting the required resources, press **C** to craft the block.
For example:

* If a recipe requires **3 leaves**, collect them first.
* Then press **C** to craft **1 grass block**.
* The game will remove 3 leaves from your inventory and add 1 grass block.

## ⚙️ Development Challenge Faced

A major challenge was implementing the crafting logic. Initially, a separate script called `Crafting.gd` was planned. However, it couldn't be implemented independently due to integration complexity.

### 🧩 Solution

To resolve this, the crafting functionality was directly implemented inside `Player.gd`. This made the system more cohesive and allowed smoother interaction between player controls, inventory updates, and crafting logic.

