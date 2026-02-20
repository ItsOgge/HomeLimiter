## Overview

This plugin works with **EssentialsX** to automatically enforce player home limits based on their current rank or permission group.

When a player is promoted or downgraded, the plugin checks their allowed home limit in EssentialsX and adjusts it if necessary. This ensures players never exceed the number of homes permitted by their active rank in EssentialsX.

---

## How It Works

* Each rank in EssentialsX can allow a specific number of homes
* When a player loses a rank, their new limit is applied instantly
* If they exceed the new limit, the **most recently created homes are removed automatically**

### Example

If the **VIP** rank allows 5 homes in EssentialsX and the player is downgraded to a rank that allows only 2 homes, the plugin will remove the 3 newest homes. No manual action required.

---

## Why Use This Plugin?

* Prevents abuse of temporary ranks in EssentialsX
* Fully automatic - no staff intervention needed
* Keeps progression balanced and fair
* Lightweight and performance-friendly
* Works seamlessly with EssentialsX permission systems

Perfect for servers that use EssentialsX for rank-based perks and want reliable, hands-free home limit enforcement.
