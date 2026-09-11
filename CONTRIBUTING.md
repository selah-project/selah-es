# Cómo contribuir a la versión española de Selah

Gracias por ayudar a que esta versión sea más exacta, clara y natural. No hace
falta ser especialista para señalar un problema: explica lo que observas,
aporta la evidencia que tengas y distingue una certeza de una sugerencia.

## Informe o solicitud de cambio

- Abre un **issue** cuando la lectura necesite discusión, haya varias opciones
  posibles o no sepas cómo debe cambiar el registro alineado.
- Abre un **pull request** cuando el error y el reemplazo exacto estén claros.
- Para errores de la aplicación, o asuntos privados de seguridad, cuentas o
  datos personales, usa [el soporte de Selah](https://selahproject.com/support).

## Qué debes incluir

Indica el libro, capítulo, versículo y token hebreo; el texto actual; el texto
propuesto; la razón del cambio; y la fuente léxica, gramatical, contextual o
publicada que lo apoya. Di también si eres hablante nativo de español y si lees
directamente el hebreo.

## Cómo editar un registro

Los archivos están en `<libro>/<capítulo>/<versículo>.json`.

- Cambia `translation` y el `gloss` del token correspondiente cuando ambos
  resulten afectados.
- Conserva `book`, `chapter`, `verse`, `ref`, los valores hebreos `surface`, el
  orden y el número de tokens, salvo que informes un defecto de alineación.
- No cambies los campos de modelo, nivel, fecha u otra procedencia solo para
  presentar la corrección como una generación nueva.
- Conserva las convenciones de los corchetes, los Nombres divinos y `⟨את⟩`.
- Evita cambios solo de formato y correcciones no relacionadas.

Comprueba el JSON editado:

```bash
python3 -m json.tool genesis/1/1.json >/dev/null
```

El hebreo viene primero. Cuando dos lecturas sean defendibles, explica la
diferencia en vez de presentar una preferencia como certeza. No copies una
traducción moderna protegida por derechos de autor.

## Trabajo asistido por IA

Declara el uso sustancial de modelos de lenguaje o traducción automática,
incluido el control humano realizado. No envíes reescrituras masivas sin
revisión. Quien contribuye responde por cada palabra propuesta.

## Licencia, atribución y revisión

Al contribuir, declaras que tienes derecho a hacerlo y aceptas que el material
incorporado se distribuya bajo [CC BY-SA 4.0](LICENSE.md). El historial de Git
conserva el registro público y la atribución. El equipo mantenedor compara la
propuesta con el hebreo, las convenciones, las fuentes y la alineación. Puede
aceptarla, revisarla contigo, esperar más evidencia o rechazarla explicando la
razón. Critica la lectura, no a la persona.

## Conduct

Be honest, be kind, show your evidence. Distinguish certainty from
suggestion. The maintainers weigh and decide.
