# Workflows: trabajar con Cursor sin perder el control ⚙️

Cómo se ve un día real, no solo "autocompletar".

## 1. El loop diario: Planear → Delegar → Revisar

```
┌─ PLANEAR ──────┐   ┌─ DELEGAR ──────┐   ┌─ REVISAR ──────┐
│ Defines tarea  │ → │ Das contexto   │ → │ Lees el diff   │
│ + criterios    │   │ + dejas a la IA│   │ + firmas merge │
└────────────────┘   └────────────────┘   └────────────────┘
        ↑                                          │
        └──────────── ajustas y repites ───────────┘
```

## 2. Niveles de delegación (cuánto control sueltas)

| Nivel | Cuándo usarlo | Tu rol |
|---|---|---|
| **Asistido** | Código crítico, seguridad, dinero | Tú escribes; la IA sugiere línea a línea |
| **Delegado** | Features estándar, boilerplate | La IA propone; tú revisas el diff completo |
| **Autónomo** | Prototipos, scripts desechables | La IA ejecuta varios pasos; tú validas el resultado |

> Regla: a mayor riesgo, menor delegación. Nunca delegues lo que no puedas revisar.

## 3. Conecta con tu flujo ágil

- **Refinamiento** → escribe la historia con criterios claros *antes* de abrir Cursor.
- **Sprint** → usa el modo Agente para los incrementos; revisa cada PR como revisarías el de un compañero junior.
- **Retro** → pregúntate qué prompts/rules funcionaron y guárdalos en este kit.

## 4. Errores comunes en LATAM (y cómo evitarlos)

- ❌ Pedir "hazme la app" sin contexto → ✅ una historia + criterios + restricciones.
- ❌ Aceptar diffs sin leerlos → ✅ tú eres responsable del merge, siempre.
- ❌ No usar `rules` → ✅ define tus reglas una vez y Cursor las respeta en todo el repo.
