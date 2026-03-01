# MatchLocal Releases

Este repositorio contiene las actualizaciones de MatchLocal.

## Estructura

```
├── latest.json          # Metadata de la última versión
└── downloads/           # Archivos de instalación
    ├── MatchLocal_X.X.X_x64-setup.nsis.zip
    └── MatchLocal_X.X.X_x64-setup.nsis.zip.sig
```

## Proceso de actualización

1. Compilar nueva versión con `npm run tauri build`
2. Subir archivos `.nsis.zip` y `.nsis.zip.sig` a `downloads/`
3. Actualizar `latest.json` con la nueva versión y signature
4. Push a main

La app detectará automáticamente las actualizaciones.
