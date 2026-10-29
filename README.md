# SkyDailyTasks

A Paper/Spigot 1.16.5 plugin that gives players daily item-collection tasks with SkyCoin rewards.

## Features

- Daily tasks defined in `tasks.yml`: required items, amounts and rewards
- `/günlükgörev` menu to view and complete tasks
- Rewards paid through Vault

## Tech stack

- Java 11, Maven
- Paper API 1.16.5, Vault API, SmartInvs

## Getting started

Requirements: JDK 11, Maven, and `lib/spigot-1.16.5.jar`.

```bash
mvn package
```

Copy the jar from `target/` into the server's `plugins/` folder. Vault and an economy plugin must be installed on the server.

## Configuration

| File | Purpose |
|---|---|
| `config.yml` | General settings and menu text |
| `tasks.yml` | Task list: item type, required amount, reward, lore |

## Commands

| Command | Description |
|---|---|
| `/günlükgörev` | Open the daily tasks menu |

## Project structure

```
src/main/java/com/emre/skydailytasks/
├── DailyTaskMain.java   # plugin entry point
├── listeners/, menus/   # events and GUI
├── objs/                # player data
└── utils/
```

## License

[Apache License 2.0](LICENSE)
