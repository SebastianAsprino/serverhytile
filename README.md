# Servidor de Hytale

Servidor dedicado con mods usando [ginco-org/hytale-server](https://github.com/ginco-org/hytale-server).

## Arrancar

1. Copiar los mods listados en [MODS.md](MODS.md) a `../files/mods/` (en Dokploy:
   `/etc/dokploy/compose/<appName>/files/mods/`; esa carpeta persiste entre deploys).
2. Levantar el servidor y aprobar los 2 códigos de autorización que aparecen en los logs:

   ```bash
   docker compose up -d
   docker compose logs -f
   ```

Los tokens quedan en el volumen `hytale-data` y se reutilizan en los siguientes arranques. Puerto: `5520/udp`.
