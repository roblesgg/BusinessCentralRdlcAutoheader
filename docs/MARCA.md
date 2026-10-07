# RDLC Auto Header Pro · Identidad

> Revisado el 7 de octubre de 2026 contra el código del repositorio.
> **Observado** = está en el código o en los recursos. **Propuesta** = cambio sugerido, pendiente de aprobar.
>
> Este proyecto **no forma parte de DripDev**. Es una herramienta nacida en el trabajo y co-firmada con **bitec** (su logo está en el icono). Se presenta en el perfil personal de Álvaro Robles.

---

## 1. Esencia

**Qué es:** una extensión de VS Code que arregla, con un clic, el problema de los encabezados en los informes RDLC de Business Central. Al imprimir facturas por lotes, el encabezado repite los datos del primer documento en todas las páginas; la extensión aplica el patrón SetData / GetData para que cada página muestre los suyos.

**Para quién:** desarrolladores de Microsoft Dynamics 365 Business Central que mantienen informes RDLC.

**Promesa:** lo que a mano son veinte minutos de copiar expresiones y crear un Tablix invisible, en un clic y sin errores.

**Personalidad:** herramienta técnica, precisa y seria, con un toque de "magia" (el rayo del icono). Bilingüe español / inglés.

## 2. Nombre

| Uso | Forma |
|---|---|
| **Nombre oficial** (Marketplace) | **RDLC Auto Header Pro** |
| Interfaz (cabecera del panel) | RDLC AUTO HEADER PRO, en mayúsculas por estilo |
| Identificador | `rdlc-autoheader` |

*Observado:* el README del Marketplace lo escribe "RDLC Auto Header PRO" y el panel "RDLC AUTO HEADER PRO".
*Propuesta:* en textos corrientes, siempre **RDLC Auto Header Pro**.

## 3. Icono

Archivo: `RDLCAutoHeader/icon.png` (1024 × 1024).

- *Observado:* un escudo con un rayo **azul eléctrico** con brillo, sobre un fondo de **metal cepillado oscuro**. Debajo, "RDLC" en blanco y "Auto Header" en gris. Arriba a la izquierda, el logo de **bitec · simplifica.**
- Se usa tal cual: no se recorta el logo de bitec ni se cambian sus colores.

## 4. Color

### Icono (marca)

| Nombre | Hex | Uso |
|---|---|---|
| Rayo | `#01B9F7` | Color de marca: portadas, insignias, enlaces destacados |
| Azul profundo | `#046CC0` | Sombras y degradados del rayo |
| Hielo | `#AFEDF9` | Brillos |
| Metal | `#1B1F22` | Fondo de portadas |

### Interfaz del panel (Catppuccin Mocha)

| Variable | Hex | Uso |
|---|---|---|
| `--bg` | `#1E1E2E` | Fondo del panel |
| `--card` | `#313244` | Tarjetas de ajustes y botones |
| `--text` | `#CDD6F4` | Texto |
| `--text-dim` | `#A6ADC8` | Texto secundario |
| `--accent` | `#CBA6F7` | Malva: pestaña activa, títulos, interruptores |
| `--accent-dim` | `#89B4FA` | Azul: secciones y botón principal |
| — | `#A6E3A1` | Verde: registro de éxito |
| — | `#F38BA8` | Rosa: quitar archivo, errores |
| — | `#6C7086` | Texto apagado |
| — | `#11111B` | Fondo del registro |

*Observado:* el icono (azul eléctrico sobre metal) y el panel (malva y azul pastel de Catppuccin) usan paletas distintas. Las dos funcionan: el panel se integra en VS Code, y el icono destaca en el Marketplace.
*Propuesta:* portadas y README con la paleta del **icono**; el panel se queda con **Catppuccin**.

## 5. Tipografía

- *Observado:* **Segoe UI**, la letra del sistema, igual que VS Code. Títulos y pestañas en mayúsculas con espacio entre letras. El registro, en monoespaciada.
- Para portadas fuera de VS Code: **Inter** (800 en títulos), por ser equivalente y gratuita.

## 6. Forma

- *Observado:* tarjetas con esquinas de 8–10 px; botones grandes en mayúsculas; zona de arrastre con borde discontinuo azul; interruptores redondos en malva. Etiquetas bilingües "ES / EN".

## 7. Voz y tono

- *Observado:* técnico y formal. El README del Marketplace trata de usted ("Abra la pestaña…") y usa "Enterprise".
- *Propuesta para GitHub:* claro y directo, con el problema primero y la solución después. Se mantiene el vocabulario de Business Central (informe, encabezado, DataSet, Tablix, SetData / GetData) y se añade un resumen en inglés.

## 8. Imagen

- Capturas reales del panel dentro de VS Code.
- Para explicar el problema, un esquema de **antes / después** con páginas de factura. Se presenta como esquema, nunca como captura.
- Nunca informes reales con datos de clientes ni de la empresa.

## 9. Pendientes

- **Decisión:** ¿se pueden mantener en el repositorio público los informes de ejemplo de la raíz (`BTCSalesInvoice_MOD.rdlc`, `PackingList*.rdlc`) y el script `RDLCAutoHeader.pyw`? No contienen datos, pero el prefijo "BTC" identifica a la empresa.
- **Pendiente:** unificar el nombre a "RDLC Auto Header Pro" en el README del Marketplace y en el panel.

## Fuentes

- `RDLCAutoHeader/package.json`
- `RDLCAutoHeader/src/extension.ts` (estilos del panel)
- `RDLCAutoHeader/icon.png`
- `RDLCAutoHeader/README.md`
- Ficha del Marketplace (v1.7.2)
