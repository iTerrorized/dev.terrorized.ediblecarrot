# Edible Carrot System

An interactive edible carrot system for VRChat. Hold it, bite it, throw it!

## Features

- **Single Hand Mode**: Carrot spawns in your preferred hand (left, right or swap Between Hands)
- **Dual Hand Mode**: Independent carrots in both hands, each with their own enable toggle
- **Bite Detection**: Bring the carrot to your mouth to take a bite (contact-based)
- **Throwing**: Open your hand to toss the carrot (optional, can be toggled in-game and in the installer)
- **Quest Compatible**: Works on both PC and Quest platforms
- **Write Defaults options**: Auto, Off, or On

## Requirements

- Unity 2022.3
- VRChat Avatars SDK 3.10.0+
- Poiyomi 9.2+ (PC only)
- A valid license key ([purchase here](https://terrorized.dev))

## Installation

### Via VRChat Creator Companion (Recommended)

1. **Add to VCC** on the [listing page](https://iterrorized.github.io/Edible-Carrot-Installer/).

2. In VCC, open your avatar project and add **Edible Carrot System** from the packages list.

## Setup Guide

### Step 1: Add the Installer Component

1. Select your avatar's root GameObject in the Hierarchy
2. Go to **Terrorized/Installers/Edible Carrot Installer** at the top of your screen
3. The installer inspector will appear

### Step 2: Verify Your License

1. Enter your license key in the **License Key** field
2. Click **Verify**
3. Once verified, the setup options will appear

### Step 3: Configure Options

| Option | Description |
|--------|-------------|
| **Hand Mode** | Choose **Single Hand** or **Dual Hand** |
| **Preferred Hand** | Left, Right, or Swap Between Hands (Single Hand only) |
| **Throwing** | Enable or disable the throwing mechanic |
| **Platform** | PC or Quest |
| **Write Defaults** | Auto (recommended), On, or Off |
| **Menu Path** | Where to place the Edible Carrot submenu in your expressions menu |

### Step 4: Start Setup

1. Click **Start Setup**
2. The installer will create carrot target objects on your avatar
3. Use the installer script in the inspector to click edit positions, and using the handels in the scene move the carrot and mouth targets to the correct positions
4. Adjust scale using the sliders in the inspector if needed

### Step 5: Finish Setup

1. Once you're happy with the positioning, click **Finish Setup**
2. The installer will generate:
   - FX animator layers with all carrot logic
   - VRC Expression Parameters
   - VRC Expression Menu entries
   - Animation clips for all carrot states

## In-Game Controls

### Expressions Menu

| Control | Description |
|---------|-------------|
| **Enable** | Toggle the carrot on/off (Single Hand mode) |
| **Enable Left** | Toggle the left carrot on/off (Dual Hand mode) |
| **Enable Right** | Toggle the right carrot on/off (Dual Hand mode) |
| **Allow Throwing** | Toggle throwing on/off (if throwing is enabled) |

### Hand Gestures

| Gesture | Action |
|---------|--------|
| **Fist** | Spawn the carrot in your hand |
| **Open Hand** | Throw the carrot (if throwing is enabled) |
| **Fist again** | Respawn the carrot |

### Bite Mechanic

Bring the carrot close to your avatar's mouth to bite it. Each bite shrinks the carrot slightly. The carrot respawns at full size when you disable and re-enable it.

### Swap Mode (Single Hand)

When using **Swap Between Hands** mode:
1. Fist one hand to spawn the carrot there
2. Fist the other hand to swap it over (Right hand will always take priority over the left)
3. The carrot moves between hands with a smooth transition

## Uninstalling

1. Select your avatar and go to **Terrorized/Installers/Edible Carrot Installer** at the top of your screen
2. Click **Remove Setup** to cleanly remove all generated layers, parameters, menu entries, and objects
3. Remove the Edible Carrot Installer component

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Carrot doesn't appear | Make sure **Enable** is toggled on in your expressions menu and gestures are enabled |
| Bite not working | Check that the mouth target is positioned correctly on your avatar's mouth |
| Menu not showing | Verify the selected menu path has room (VRC max is 8 controls per menu) |
| Setup fails | Ensure your avatar has a VRC Avatar Descriptor with an FX layer slot |

## Support

- Discord: [Support Server](https://discord.gg/X9sgs7KCAv)

## Authors

Made by [@zenifyy](https://payhip.com/ZenifyyVR) and [@iterrorized](https://terrorized.dev) with love <3
