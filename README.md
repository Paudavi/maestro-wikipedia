# Maestro – Tests E2E de la app de Wikipedia

> 🚧 **Proyecto en proceso.** La estructura y los flujos todavía están cambiando.

Proyecto de práctica de automatización de tests mobile end-to-end con [Maestro](https://maestro.mobile.dev/), usando como app bajo prueba Wikipedia para Android (`org.wikipedia`).

## Estructura

```
flows/       Flujos de test agrupados por funcionalidad (basic, search, auth…)
subflows/    Pasos reutilizables (p. ej. saltear el onboarding)
scripts/     Scripts JS para generar datos de prueba
samples/     Flujos de ejemplo oficiales de Maestro, como referencia
config.yaml  Configuración del workspace
```

## Cómo correrlo

1. Instalar [Maestro](https://maestro.mobile.dev/getting-started/installing-maestro).
2. Tener un emulador o dispositivo Android con la app de Wikipedia instalada (el APK no está en el repo).
3. Ejecutar:

```bash
maestro test .                     # todos los flujos
maestro test --include-tags smoke . # solo los smoke tests
```
