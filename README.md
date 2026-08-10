# Castle Yeet 🏰💥

A physics-based web arcade game inspired by classic castle defense flash games. Hordes of invading stickmen are marching toward your fortress—grab them with your cursor, fling them high into the sky, drop them onto your castle to convert them into loyal defenders, and build powerful tower upgrades to survive endless waves!

![Castle Yeet Gameplay](https://img.shields.io/badge/Status-Live-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue)

🎮 **Play Live:** [https://castle-yeet.vercel.app](https://castle-yeet.vercel.app)

---

## 🌟 Key Features

* **Physics-Based Flinging Mechanics**: Click, drag, and throw enemy stickmen into the stratosphere! Drop them from lethal heights to turn them into bloody splats and crater the battlefield.
* **Special Enemy Types**:
  * **Soldiers**: Standard foot units.
  * **Runners**: Fast, agile shock troops.
  * **Knights / Armored**: Heavy armor that drops swords, helmets, and shields on death.
  * **Ram Bearers**: Carry massive wooden rams to smash castle walls.
  * **Shield Bearers**: Carry heavy scutum tower shields that protect frontline units.
  * **Berserkers**: Fast, aggressive melee attackers.
  * **Brutes & Titan Giants**: Massive bullet-sponge giants that deal devastating wall damage.
* **Conversion System**: Grab enemies and drop them directly onto your castle gate to convert them into troops.
* **Castle Towers & Unit Management**:
  * **Guys With Bows (Archers)**: Auto-shoot whizzing arrows at incoming invaders. Includes drawn archer units stationed on bastions that animate when drawing back their bows.
  * **Suspicious Wizard Stuff (Wizards)**: Auto-cast persistent lightning spell zones that fry enemy hordes into smoldering charcoal. Includes animated wizard units with glowing magic staves.
  * **Boom School (Bombers)**: Auto-deploy suicide bombers that run into crowds and explode.
  * **Unpaid Maintenance Crew (Craftsmen)**: Automatically repair castle wall HP between rounds.
* **Dynamic Battlefield Destruction**: Craters, dirt explosion debris, blood splats, stuck arrows, and persistent body/gear chunks that stay on the field until the **Stickman Cleaner** sweeps through.
* **Bonus Rewards**: Score **TRIPLE MONEY** when throwing an enemy into another enemy to crush them!
* **Global Leaderboard**: Integrated Supabase backend with local storage fallback to track the top castle defenders worldwide.

---

## 🎮 How to Play

1. **Defend the Wall**: Click & drag enemy stickmen and fling them upwards into the air.
2. **Convert Troops**: Once you build a **Temple**, drop grabbed enemies on your castle gate to start converting them.
3. **Assign Converts**: Open the **Between Waves** menu to assign converts as Archers, Wizards, or Bombers.
4. **Speed Toggle**: Press `F` or click the HUD speed button to cycle between 1x, 2x, and 3x game speed.

---

## 🛠️ Tech Stack

* **Frontend**: HTML5 Canvas, Vanilla JavaScript (ES6+), Web Audio API
* **Backend / Database**: Supabase (PostgreSQL with Row Level Security)
* **Deployment**: Vercel

---

## 🚀 Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/AaronC1992/castle-yeet.git
   cd castle-yeet
   ```

2. Open `castle-yeet.html` directly in any web browser, or serve it using a local dev server (e.g. Live Server for VS Code).

3. *(Optional)* Configure your own Supabase leaderboard:
   - Run the SQL setup script located in [`supabase/leaderboard-schema.sql`](supabase/leaderboard-schema.sql) in your Supabase SQL editor.
   - Update `leaderboard-config.js` with your project URL and anon public key:
     ```javascript
     window.SUPABASE_URL = 'https://YOUR_PROJECT.supabase.co';
     window.SUPABASE_ANON_KEY = 'YOUR_SUPABASE_ANON_KEY';
     ```

---

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.
