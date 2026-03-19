# Edible Carrot System

An interactive edible carrot avatar accessory for VRChat. Hold it, bite it, throw it!

## Features

- **Single Hand Mode**: Carrot spawns in your preferred hand (left or right)
- **Dual Hand Mode**: Independent carrots in both hands, each with their own enable toggle
- **Swap Between Hands**: Fist one hand to spawn, fist the other to swap the carrot over
- **Bite Detection**: Bring the carrot to your mouth to take a bite (contact-based)
- **Throwing**: Open your hand to toss the carrot (optional, can be toggled in-game)
- **Quest Compatible**: Works on both PC and Quest platforms
- **Write Defaults Auto-Detect**: Automatically matches your avatar's existing WD setting

## Requirements

- Unity 2022.3
- VRChat Avatars SDK 3.10.0+
- A valid license key ([purchase here](https://terrorized.dev))

## Installation

### Via VRChat Creator Companion (Recommended)

1. Add the package listing to VCC:
   ```
   https://iterrorized.github.io/Edible-Carrot-Installer/index.json
   ```
   Or click **Add to VCC** on the [listing page](https://iterrorized.github.io/Edible-Carrot-Installer/).

2. In VCC, open your avatar project and add **Edible Carrot System** from the packages list.

3. Open your Unity project. The package will be imported automatically.

## Setup Guide

### Step 1: Add the Installer Component

1. Select your avatar's root GameObject in the Hierarchy
2. Click **Add Component** and search for **Edible Carrot Installer**
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
| **Platform** | PC, Quest, or Both |
| **Write Defaults** | Auto (recommended), On, or Off |
| **Menu Path** | Where to place the Edible Carrot submenu in your expressions menu |

### Step 4: Start Setup

1. Click **Start Setup**
2. The installer will create carrot target objects on your avatar
3. Use the Scene view handles to position the carrot where you want it on each hand
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

Bring the carrot close to your avatar's mouth to bite it. Each bite shrinks the carrot slightly. The carrot respawns at full size when you re-fist.

### Swap Mode (Single Hand)

When using **Swap Between Hands** mode:
1. Fist one hand to spawn the carrot there
2. Fist the other hand to swap it over
3. The carrot moves between hands with a smooth transition

## Uninstalling

1. Select your avatar and open the Edible Carrot Installer inspector
2. Click **Remove Setup** to cleanly remove all generated layers, parameters, menu entries, and objects
3. Remove the Edible Carrot Installer component

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Carrot doesn't appear | Make sure **Enable** is toggled on in your expressions menu |
| Bite not working | Check that the mouth target is positioned correctly on your avatar's head |
| Menu not showing | Verify the selected menu path has room (VRC max is 8 controls per menu) |
| Setup fails | Ensure your avatar has a VRC Avatar Descriptor with an FX layer slot |

## Support

- Website: [terrorized.dev](https://terrorized.dev)
- Discord: [Support Server](https://discord.gg/X9sgs7KCAv)
- Issues: [GitHub Issues](https://github.com/iTerrorized/dev.terrorized.ediblecarrot/issues)

## Authors

Made by [@zenifyy](https://payhip.com/ZenifyyVR) and [@iterrorized](https://terrorized.dev) with love <3
