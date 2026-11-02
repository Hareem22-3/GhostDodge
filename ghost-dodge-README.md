# 👻 Ghost Dodge Game

This is a survival game where you play as a little pumpkin person trying to dodge a bunch of ghosts bouncing around the screen. The longer you survive, the higher your score.

## What This Game Is

You're trapped in a room with 5 ghosts that bounce off the walls and move in different directions. You can move in all four directions to avoid them. Touch a ghost and it's game over. Your score is how many seconds you stayed alive.

## How to Play

1. Open `ghost-dodge.html` in any browser
2. Use the **Arrow Keys** to move your character around
3. Avoid touching any of the white ghosts
4. Survive as long as possible
5. When you die, press **SPACE** to restart

## Controls

- **↑ Up Arrow** - Move up
- **↓ Down Arrow** - Move down
- **← Left Arrow** - Move left
- **→ Right Arrow** - Move right
- **SPACE** (when dead) - Restart game

## Game Features

**Your character:**
- Orange pumpkin-headed person with a face
- Black eyes and a smile
- Moves in all 4 directions
- Can't go off the edges of the screen

**The ghosts:**
- 5 white semi-transparent ghosts
- Each one moves at different speeds
- They bounce off the walls when they hit edges
- Have eyes and a wavy bottom (classic ghost shape)
- They NEVER stop moving

**Scoring:**
- Time survived is your score (shown in seconds)
- Every frame you're alive adds to your score
- Try to beat your personal best

**Game over:**
- Happens when you touch any ghost
- Shows your final survival time
- Press SPACE to play again

**Visuals:**
- Dark blue/purple background
- Small stars scattered around (not moving)
- Purple color scheme for UI text

## What I Learned

This game taught me:
- How to handle 4-directional movement
- Managing multiple objects with different speeds (the ghosts)
- Making objects bounce off walls (reversing velocity)
- Distance calculation for collision detection
- Using arrays to store multiple similar objects
- Game state management (playing vs game over)

## The Code Structure

**Variables:**
- `playerX`, `playerY` - your position
- `ghosts` array - holds all 5 ghosts with their positions and speeds
- `score` - frames survived (divided by 60 to show seconds)
- `gameOver` - boolean to track if you're alive or dead

**How ghosts work:**
Each ghost has:
- x and y position
- speedX and speedY (can be positive or negative)
- When they hit a wall, their speed flips direction

**Collision detection:**
- Uses `dist()` function to measure distance between player and each ghost
- If distance is less than 35 pixels, collision happened

## Want to Modify It?

**Make it easier:**
- Reduce number of ghosts (change the loop that creates them)
- Make ghosts slower (reduce the `random()` range for speed)
- Make your character smaller
- Make the play area bigger

**Make it harder:**
- Add more ghosts
- Make them faster
- Make your character bigger
- Make the ghosts speed up over time
- Add obstacles you can't pass through

**Add features:**
- Power-up that makes you invincible for 3 seconds
- Score multiplier for close calls
- Ghosts that chase you instead of random movement
- Different colored ghosts that move differently
- Sound effects
- Lives system (3 hits before game over)

**Change the look:**
- Different character (maybe a bat or witch)
- Change ghost colors or shapes
- Add more background details
- Make the ghosts fade in and out

## Technical Details

**Built with:**
- HTML/CSS for page structure
- JavaScript for game logic
- p5.js library for graphics

**Canvas size:** 600px × 400px

**Frame rate:** 60 FPS (p5.js default)

## Strategy Tips

- Stay near the center at first to see where ghosts are coming from
- Keep moving - don't stay still too long
- Watch all ghosts, not just the closest one
- Corners are dangerous because you can get trapped
- Sometimes it's better to dodge toward a ghost that just passed you

## Troubleshooting

**Character won't move:**
- Click on the game screen first
- Check you're using arrow keys

**Game feels laggy:**
- Close other programs
- Try a different browser
- Your computer might be slow

**Can't restart after dying:**
- Make sure you're pressing SPACE, not ENTER

## Why This Game Is Hard

The randomness makes it tough. You can't memorize patterns because the ghosts move unpredictably. Every game is different. Sometimes you get lucky and survive a long time, sometimes you die in 5 seconds because ghosts spawn near you.

That's what makes it fun though - it's all about quick reflexes and situational awareness.

---

Good luck surviving! My personal best is about 23 seconds. Can you beat that? 👻
