# MythicMobs_CustomMobs

Custom mobs, skills and items from my personal Minecraft server. Most mobs are designed to be beatable with vanilla equipment between **1 and 4 players**.

## List of Mobs
<ul>
  <li>
    <a href="mobs/Cruzader.yml">Cruzader</a>
    <p>
      A boss-like skeleton with a regenerating shield, pull/teleport movement skills and an AoE implosion attack. Can summon multiple `CruzaderGolem` minions. Drops `CruzaderLeggings` (100%); other armor pieces are rare. Recommended group: **1–3 players**. Spawner: `spawners/FirstCruzader.yml` (world: 487,125,-63).
    </p>
  </li>

  <li>
    <a href="mobs/CruzaderGolem.yml">Cruzader Golem</a>
    <p>
      Iron Golem minion used as support by the Cruzader. Durable but low damage; typically summoned via `SummonGolem` skill and set to despawn.
    </p>
  </li>

  <li>
    <a href="mobs/ExampleMobs.yml">Skeletal Knight</a>
    <p>
      A dungeon infantry (WITHER_SKELETON) wearing iron gear and dropping gold nuggets. Used in `Dungeon1` spawners. Recommended group: **solo–2 players**.
    </p>
  </li>

  <li>
    <a href="mobs/ExampleMobs.yml">Skeleton King</a>
    <p>
      Example boss (500 HP) with summons and special attacks. Intended as a mid/late boss — **2–3 players** recommended.
    </p>
  </li>

  <li>
    <a href="mobs/ExampleMobs.yml">Statically Charged Sheep</a>
    <p>
      Sheep that periodically calls lightning in a radius — a good environmental hazard for solo or small groups.
    </p>
  </li>

  <li>
    <a href="mobs/ExampleMobs.yml">Angry Sludge</a>
    <p>
      Large slime boss with poison and terrain effects (block masks). Tough and best handled by groups.
    </p>
  </li>

  <li>
    <a href="mobs/VanillaMobs.yml">Vanilla tweaks</a>
    <p>
      Small tweaks to vanilla mobs (e.g., `CAVE_SPIDER`, `WITHER_SKELETON`, `GIANT`) — useful to balance encounters.
    </p>
  </li>

  <li>To be continued…</li>
</ul>

---

## Spawners & placement
- `spawners/FirstCruzader.yml` — single Cruzader spawn (world: X:487 Y:125 Z:-63). `UseTimer: true`, `Cooldown: 1800`, `MaxMobs: 1`.
- `spawners/Dungeon1Skeleton*.yml` — several spawners for the `Dungeon1` group spawning `SkeletalKnight` (MaxMobs: 6, Cooldown: 600).

## Items & Droptables
- `items/CruzaderItems.yml` — Cruzader armor and sword (unbreakable, custom model data, attribute bonuses and enchants).
- `droptables/CruzaderDrops.yml` — Cruzader gear drop chances (Leggings guaranteed, other pieces rare).

## Skills (quick)
- `skills/CruzaderSkills.yml` contains the Cruzader skillset: `CruzaderImplosion`, pulls, teleports, `SummonGolem`, stuns and movement mixes used as timers or on-damage triggers.

## Key config notes
- `config/config-mobs.yml`: Default drop method is `VANILLA`.
- `config/config-spawning.yml`: Vanilla spawns are **enabled** (`DisableVanillaSpawns: false`); spawn radii and limits configured here.

---

## How to edit & reload
1. Edit files under `mobs/`, `items/`, `skills/`, `droptables/`, or `spawners/`.
2. Reload MythicMobs or restart the server to apply changes (`/mythicmobs reload` or server restart).

---

## Notes & tips
- Use `ExampleMobs.yml`, `ExampleItems.yml` and `ExampleDropTables.yml` as templates for new content.
- Verify that skill names and targeters match when assigning skills to mobs.
- If you'd like, I can generate a per-mob detail sheet (skills, triggers, timers) or a short `CHANGELOG` file.
