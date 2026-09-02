# HorseStamina

Horse racing with stamina management and minigames for Paper 1.21.x

## Features

- **Stamina system**: Horses have stamina bars tied to health; stamina depletes based on speed (pace)
- **Pace control**: 6 speed tiers (0-5) with configurable slowness and stamina drain
- **Collision detection**: Horses collide with other horses, dealing configurable damage
- **Block contact damage**: Horses take damage when touching designated block types
- **Stamina minigames**: Random timed challenges during races that reward stamina recovery
- **Emergency slowness**: Auto-applies slowness when stamina is critical
- **Stamina regen**: Configurable regeneration and slowness based on stamina ranges

## Commands

- `/race` - Activate race mode (`horsepower.race`)
- `/horsestamina reload` - Reload config (`horsepower.admin`)

## Installation

1. Download the JAR from releases
2. Drop into your plugins folder
3. Configure `config.yml` to tune stamina behavior, paces, and minigames
4. Restart server

## Configuration

Key settings in `config.yml`:

- **Stamina mode**: HP-based (stamina tied to horse health)
- **Paces 0-5**: Each pace has stamina drain and slowness levels
- **Collision**: Horse-to-horse damage, knockback, separation distance
- **Block contact**: Damage and stamina drain on specific blocks (logs, etc.)
- **Minigames**: Challenge types at each pace level with stamina rewards
- **Stamina ranges**: Regen rate and slowness by stamina thresholds

## Requirements

- Paper 1.21+
- Java 25+

## Build

```bash
mvn clean package
```
