# Hero Wars Playable Rework Plan

## Goal

Rework the playable into a fast, readable Hero Wars battler with a simple rescue story:

**Galahad starts alone, saves Thea, then Thea and Artemis form a three-hero squad that reaches and defeats the boss.**

Target experience:

- Duration: about 2-3 minutes.
- Format: vertical 720x1280, with a 21:9 horizontally scrolling battlefield.
- Genre promise: battler gameplay, not a puzzle, runner, or fake mechanic.
- Core emotion: lone hero under pressure -> rescue -> full squad -> power growth -> boss victory.
- Main ad hook: the player feels team progression through direct battle actions.

## Core Gameplay Loop

1. Enemy pressure creates danger.
2. Player swipes to trigger a hero skill.
3. Skill solves the immediate problem.
4. XP/progress reward appears.
5. The squad moves forward to the next fight.

Every interaction should create a visible change: rescue, heal, wave clear, upgrade, boss defeat.

## Story Flow

### Beat 1: Galahad Alone

Duration: 15-25 seconds.

- Start on the far-left part of the 21:9 road.
- Galahad enters alone or is already standing in combat stance.
- Spawn 2 weak enemies.
- Galahad auto-attacks, but takes visible damage.
- Prompt appears: `SWIPE UP`.
- Player swipes Galahad.
- Galahad casts a strong slash and clears the enemies.
- Progress bar moves to the first milestone.

Purpose: teach the player the only required input and show that Galahad is strong but not invincible.

### Beat 2: Rescue Thea

Duration: 25-35 seconds.

- Camera/background scrolls forward to a small ambush scene.
- Thea is visible on the battlefield, trapped or low HP.
- 2-3 enemies are attacking her.
- Galahad runs in from the left.
- Galahad fights, but Thea's HP keeps dropping.
- Prompt appears on Galahad: `SAVE HER`.
- Player swipes.
- Galahad uses a rescue strike, kills or knocks back enemies.
- Thea survives and moves into the party formation.
- Show a short join banner: `THEA JOINS`.
- Artemis runs in from outside the left edge, joins the formation, and immediately becomes the ranged damage dealer.
- Show a second short join banner: `ARTEMIS JOINS`.

Purpose: make the first new hero feel earned instead of just spawned.

### Beat 3: First Squad Fight

Duration: 30-40 seconds.

- Galahad, Thea, and Artemis move forward together.
- Spawn 3 enemies: 2 melee + 1 ranged.
- Enemies pressure Galahad.
- Thea auto-heals Galahad once so her role is clear.
- Prompt appears on Thea: `HEAL`.
- Player swipes Thea.
- Thea casts a big heal wave.
- Artemis pressures ranged enemies while Galahad finishes the frontline.
- XP orbs fly across the full squad.

Purpose: show clear team roles: Galahad tanks, Thea heals, Artemis deals ranged damage.

### Beat 4: Power Spike

Duration: 25-35 seconds.

- Background scrolls into a darker mid-road combat zone.
- Spawn 3-4 stronger demon enemies.
- Galahad starts losing HP faster.
- Thea heals, but not enough to instantly solve the fight.
- Galahad levels up or upgrades weapon.
- Prompt appears: `POWER STRIKE`.
- Player swipes Galahad.
- Galahad performs upgraded slash and clears the wave.
- Progress reaches boss milestone.

Purpose: create a strong growth moment before the final boss.

### Beat 5: Boss Fight

Duration: 35-50 seconds.

- Background scrolls to the right-side fortress/boss area.
- Boss enters with roar, screen shake, and HP bar.
- Boss hits Galahad hard once.
- Thea heals automatically once, barely stabilizing him.
- Galahad and Thea counter together.
- Boss HP drops in large readable chunks.
- Final prompt appears on Galahad: `FINISH HIM`.
- Player swipes.
- Galahad ultimate kills the boss.
- Chest appears, opens, reward burst plays, final CTA appears.

Purpose: one clean climax with immediate conversion moment.

## Timing Target

Approximate pacing:

- Beat 1: 20 seconds.
- Beat 2: 30 seconds.
- Beat 3: 35 seconds.
- Beat 4: 30 seconds.
- Beat 5: 45 seconds.

Total: about 160 seconds.

This is close to 2:40. If it feels slow, reduce travel pauses and enemy HP before cutting story beats.

## Balance Targets

- Heroes:
  - Galahad starts at level 1 or 5, but should visibly grow.
  - Thea starts as rescued NPC, then becomes controllable/support.
- Total enemies before boss: 10-12.
- Max enemies visible at once: 4.
- Player prompts: 5 total max.
  - Galahad first slash.
  - Galahad rescue strike.
  - Thea heal.
  - Galahad power strike.
  - Galahad final strike.
- Boss sequence:
  - 1 big boss hit.
  - 1 Thea save/heal.
  - 1 team counter.
  - 1 final Galahad ultimate.
- No dead time longer than 1 second unless it is a dramatic impact moment.
- Every wave should end quickly after the player's swipe.

## Combat Feel And Balance Problems To Fix

Current combat problem:

- Fights are too long.
- Auto-attacks feel weak.
- The player watches units trade small hits for too much time.
- HP bars move too slowly.
- Skill moments do not feel decisive enough.
- There is not enough visible cause and effect: danger -> swipe -> huge payoff.

New combat rule:

**Auto-combat creates tension. Player skill resolves the fight.**

That means:

- Auto-attacks should last only 2-4 exchanges before a prompt.
- Small hits should be readable, but not become the main entertainment.
- Every prompted skill should remove enemies, save a hero, or chunk the boss HP heavily.
- If the player has already understood the situation, do not keep showing more of the same attacks.

## New Damage Model

### Regular Waves

- Weak enemy HP: 24-35.
- Strong enemy HP: 45-65.
- Galahad auto-hit: 10-14.
- Enemy hit on Galahad: 8-14.
- Thea small heal: 14-20.
- Galahad skill hit: 45-90, usually enough to kill weak enemies.
- Thea ultimate heal: restore 45-60% of current missing team HP.

Design intent:

- Before the prompt, HP should visibly move.
- After the prompt, the wave should resolve within 1-2 seconds.
- No regular enemy should survive more than one major skill unless it is deliberately elite.

### Boss

- Boss HP should be low enough for visible chunks, not a long raid bar.
- Suggested boss HP: 180-240.
- Boss big hit: 30-40 damage to Galahad.
- Team counter: 50-70 boss damage.
- Thea contribution: small magic hit or heal, not a long spell sequence.
- Final Galahad strike: remaining boss HP, guaranteed kill.

Design intent:

- Boss fight should feel dangerous, but not slow.
- Boss HP should drop in 3-4 meaningful chunks.
- The final swipe must be the biggest moment in the playable.

## Timing Rules

- Enemy entrance: 300-600 ms.
- First auto exchange after spawn: within 500 ms.
- Time from wave start to player prompt: 3-6 seconds.
- Time from player swipe to wave solved: 1-2.5 seconds.
- Travel between beats: 500-900 ms.
- Boss intro: max 1.5 seconds.
- Final reward after boss death: within 1 second.

Avoid:

- 10+ seconds of idle auto-combat.
- Repeated equal-damage hits.
- Long pauses after a wave is already decided.
- Multiple enemies waiting around with tiny HP.
- Long boss back-and-forth after the player is ready to finish.

## Impact Rules

- Every heavy hit needs visible target feedback:
  - quick flash,
  - hit pause for 80-120 ms,
  - impact burst,
  - HP bar chunk drop,
  - small screen shake for large hits.
- Damage numbers should be used sparingly:
  - big crits,
  - boss chunks,
  - heal moments.
- For normal auto-attacks, rely more on animation, HP movement, and impact FX.
- Skills should have bigger silhouettes than basic attacks:
  - wider slash,
  - brighter trail,
  - enemy knockback,
  - faster death/fade.

## Visual Direction

### Battlefield

- Use the new 21:9 panorama as a horizontal journey.
- Keep the three-hero squad visually locked to the left/mid-left side of the viewport.
- Let the background scroll to imply movement through the world.
- Place enemies on the right side with clear lane spacing.
- Avoid putting units directly over high-detail ruins whenever possible.
- Stage every entrance outside the viewport; no unit may fade in at its combat position.
- Goblins use their authored walk cycle, Artemis and Thea use `run`, and demons use a procedural heavy gait because their asset has no walk clip.

### Formation

- Beat 1:
  - Galahad only, front-left lane.
- Beat 2:
  - Thea starts ahead/right of Galahad as a rescue target.
  - After rescue, she moves behind Galahad.
- Beat 3 onward:
  - Galahad front-left.
  - Thea back-left/upper-left.
  - Artemis back-left/lower-left with a clear firing lane.
  - Enemies mid-right/right.
- Boss:
  - Boss large on right.
  - Galahad closer to boss.
  - Thea safely behind.

### Prompt UI

- Remove huge prompt text across the middle of the fight.
- Use compact prompt near the active hero:
  - animated upward arrow,
  - short label,
  - no long sentence.
- Suggested labels:
  - `SWIPE UP`
  - `SAVE HER`
  - `HEAL`
  - `POWER STRIKE`
  - `FINISH HIM`
- Prompt must never cover hero faces, HP bars, or enemy bodies.

### HUD

- Shrink top progress bar.
- Milestones should match story:
  - rescue,
  - power-up,
  - boss.
- Hide permanent `INSTALL` button during combat or make it much smaller.
- Show strong CTA only after boss/chest reward.
- Remove debug text before final delivery.

### HP And Labels

- Galahad: HP + level.
- Thea before rescue: HP only or `THEA` + low HP.
- Thea after rescue: HP + level.
- Enemies: HP bars only, no names.
- Boss: name + big HP bar.

### FX

- Galahad first slash: clean bright sword arc.
- Rescue strike: knockback or enemy pop with dust.
- Thea heal: green/blue wave with visible HP refill.
- Power strike: larger slash plus brief upgrade glow.
- Boss attack: red impact + screen shake.
- Final strike: strongest slash, boss fade/death, chest reward burst.

## Implementation Plan

### Phase 1: Flow Rewrite

- Replace current multi-wave flow with the five beats above.
- Remove Ginger from the main playable flow.
- Use Artemis as the lightweight third hero from the supplied asset pack.
- Add Thea as a rescue NPC state before she joins the party.
- Make `joinThea()` move her into final formation.
- Make `joinArtemis()` run her in from outside the frame after the rescue.

### Phase 2: Layout Cleanup

- Reposition Galahad, Thea, Artemis, enemies, boss, and chest for the new panorama.
- Cap enemies at 4 visible units.
- Stop text from crossing the combat lane.
- Tune z-index by y-position so units read as standing on the ground.

### Phase 3: Balance Pass

- Reduce enemy HP and wave count.
- Make Galahad take enough damage to need Thea.
- Make Thea heal meaningful but not spammy.
- Make boss HP drop in clear chunks.
- Keep all swipe payoffs immediate.

### Phase 4: HUD And CTA

- Update progress milestones to rescue/power/boss.
- Hide or minimize install button during gameplay.
- Remove debug status.
- Improve final chest + CTA screen.
- Keep `clickTag` behavior.

### Phase 5: Polish And Verification

- Check full run duration.
- Check file size.
- Check 360x640, 390x844, 414x896, 720x1280.
- Check no text overlaps actors.
- Check all prompts are understandable without instructions.
- Check the new 21:9 background scrolls from start to boss cleanly.

## Current Decisions

- Use battler, not dungeon.
- Use 21:9 scrolling background.
- Start with only Galahad.
- Thea is rescued and then joins.
- Boss is the final climax.
- Ginger is removed from the core flow for clarity.

## Open Questions

- Should Galahad start visibly weak at level 1, or already recognizable at level 5?
- Should Thea be locked in a cage/trap visually, or simply surrounded and low HP?
- Should the player control Thea once, or should Thea remain auto-support after joining?
- Should the always-visible install button be hidden completely until the end?
- Do we want the full run closer to 2:00 or closer to 2:40?
