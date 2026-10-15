# Servidor de Hytale

Servidor dedicado con mods usando [ginco-org/hytale-server](https://github.com/ginco-org/hytale-server).

## Arrancar

1. Copiar los mods listados en [MODS.md](MODS.md) a `mods/`.
2. Levantar el servidor y aprobar los 2 códigos de autorización que aparecen en los logs:

   ```bash
   docker compose up -d
   docker compose logs -f
   ```

Los tokens quedan en `data/` y se reutilizan en los siguientes arranques. Puerto: `5520/udp`.
