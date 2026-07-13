# Ertenix

Český/slovenský PvP & SMP Minecraft server.

- **Web:** ertenix.net
- **Vyvíjeno týmem:** [Bythorn](https://bythorn.dev)

## O projektu

Ertenix je český/slovenský PvP a SMP Minecraft server běžící na vlastní infrastruktuře (Hexado VPS). Tento repozitář obsahuje veškerou konfiguraci, nástroje a assety potřebné k provozu a údržbě serveru — resource pack, konfigurace pluginů, pomocné skripty a další.

Server běží na architektuře Velocity proxy + Paper backendy, spravované přes Pterodactyl panel.

## Struktura repozitáře

```
ertenix/
├── resourcepacks/   # Resource packy (pack.zip, SHA1 hashe)
├── plugins/         # Konfigurace a seznam použitých pluginů
├── scripts/         # Pomocné skripty (nasazení, zálohy, automatizace)
├── configs/         # Konfigurace serveru, proxy, databází apod.
└── README.md
```

## Resource packy

Oficiální resource pack serveru je hostovaný přímo na ertenix.net a je vynucen přes plugin **ForcePack**. SHA1 hash je udržovaný spolu s packem, aby se předešlo problémům s cachováním na straně klienta.

## Použité pluginy

| Plugin | Účel |
|---|---|
| LuckPerms | Správa práv a skupin (sdílená MySQL napříč proxy/backendy) |
| ForcePack | Vynucení resource packu |
| PlaytimePlus | Odměny za odehraný čas na serveru |
| DiscordSRV | Propojení herního chatu s Discordem |
| ExcellentCrates | Herní bedny a loot systém |
| DecentHolograms | Interaktivní hologramy (menu, info tabule) |
| Animated Scoreboard | Dynamický scoreboard s PlaceholderAPI |

## Skripty

Ve složce `scripts/` najdeš pomocné nástroje pro nasazení, zálohy a automatizaci.

## Konfigurace

Ve složce `configs/` jsou uložené konfigurační soubory pro Velocity proxy, Paper backendy a další součásti infrastruktury.

## Tým

| Přezdívka | Role |
|---|---|
| chlebasmc | Frontend, infrastruktura |
| opecko14 | Backend, databáze |
| maxern_ytb | Administrace, komunita |

## Licence

Viz [LICENSE.md](./LICENSE.md).
