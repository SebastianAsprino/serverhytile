# Servidor de Hytale

Servidor dedicado con mods usando [ginco-org/hytale-server](https://github.com/ginco-org/hytale-server).
Los mods están en `mods/` y se instalan solos en cada arranque.

## Arrancar

```bash
docker compose up -d
docker compose logs -f   # aprobar los 2 códigos de autorización la primera vez
```

Los tokens de autorización quedan en el volumen `hytale-data` y se reutilizan entre deploys.
Puerto: `5520/udp`.

## Agregar o quitar mods

Poner o sacar el `.jar`/`.zip` de `mods/`, hacer push y redeployar.
