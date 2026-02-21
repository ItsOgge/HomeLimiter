## Overview

HomeLimiter works with **EssentialsX** and **LuckPerms** to automatically enforce player home limits based on their highest active permission group.

When a player is promoted or downgraded, the plugin checks how many homes their new rank allows and adjusts their homes if necessary. This ensures players never exceed the number of homes permitted by their current group.

HomeLimiter also supports existing servers — players are checked on startup to make sure their home count matches their rank.

---

## How It Works

* Each permission group can allow a specific number of homes (configured in `config.yml`)
* The plugin reads the player’s highest weighted LuckPerms group
* When a player’s group changes, their new limit is applied instantly
* On server startup, all players are automatically validated
* If a player exceeds their limit, the **most recently created homes are removed automatically**

### Smart & Safe Removal

* Newest homes are removed first
* Older homes without timestamps (from before installation) are sorted Z → A
* Protected home names (like `home`) are never removed

Only the exact number of excess homes are removed — nothing more.

---

## Example

If the **VIP** rank allows 5 homes and the player is downgraded to a rank that allows only 2 homes, the plugin will automatically remove the 3 newest homes.

No manual action required.

---

## Why Use This Plugin?

* Prevents abuse of temporary ranks
* Fully automatic — no staff intervention needed
* Works on already established servers
* Keeps progression balanced and fair
* Lightweight and performance-friendly
* Designed specifically for EssentialsX home systems

Perfect for servers that use EssentialsX for rank-based perks and want reliable, hands-free home limit enforcement.

---

## Requirements

* EssentialsX 2.20+
* LuckPerms 5.4+
* Java 17+
* Spigot / Paper 1.20+
