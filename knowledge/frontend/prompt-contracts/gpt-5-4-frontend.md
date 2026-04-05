
# 🎨 GPT-5.4 Frontend Design — Agent Knowledge

## 📌 Context

Este documento convierte el artículo de OpenAI sobre frontend con GPT-5.4 en conocimiento operativo para agentes.

No es una guía conceptual: es un **contrato de diseño + prompting + ejecución**.

---

# 🧠 1. PRINCIPIOS BASE

## 1.1 El modelo necesita dirección explícita

El modelo no diseña bien sin:

* constraints claros
* sistema de diseño
* referencias visuales
* narrativa
* datos reales

---

## 1.2 La primera viewport es una composición

* No debe parecer un dashboard
* Debe leerse como una idea única
* Tiene una jerarquía clara

---

## 1.3 Brand > Headline

* La marca es el elemento principal
* Si quitas el nav y no se reconoce → fallo

---

## 1.4 La imagen debe trabajar

* Mostrar producto / contexto / ambiente
* No decorativa
* Si quitarla no cambia nada → mala imagen

---

## 1.5 Menos razonamiento puede ser mejor

* Para UI simples → bajo reasoning funciona mejor
* Evita sobreingeniería visual

---

## 1.6 Datos reales > placeholders

* Cambia layout, densidad y decisiones
* Evita diseños irreales

---

## 1.7 Referencias visuales son parte del prompt

* Screenshots
* Moodboards
* Diseños reales

---

## 1.8 Diseñar es definir sistema

Definir:

* colores (tokens)
* tipografía
* roles (headline, body, caption)

---

## 1.9 Diseñar incluye validar

* multi viewport
* navegación
* estados
* overlaps

---

# ⚙️ 2. FRONTEND DESIGN CONTRACT (SYSTEM PROMPT)

## 🔒 Reglas globales

* Evitar layouts genéricos
* Primera viewport = 1 composición
* Branding fuerte (hero-level)
* Tipografías no genéricas
* No fondos planos simples
* Hero full-bleed por defecto
* Hero sin overlays
* Hero con contenido mínimo:

  * marca
  * headline
  * frase corta
  * CTA
  * imagen dominante
* No cards por defecto
* Cards solo si son interacción
* Una sección = un objetivo
* Imagen debe ser ancla real
* Reducir clutter
* Motion útil (no ruido)
* Definir CSS variables
* Mobile + desktop correcto

---

## ⚠️ Anti-patrones

* Dashboard genérico
* Cards en hero
* Imagen decorativa
* Texto excesivo
* Múltiples ideas por sección
* Gradientes sin propósito
* UI basada en bloques sin jerarquía

---

## 🧩 Excepción

Si hay design system existente:
→ respetarlo SIEMPRE

---

# 🧠 3. WORKING MODEL (PRE-BUILD)

Antes de generar UI:

## 3.1 Visual Thesis

* Mood
* Energía
* Material

## 3.2 Content Plan

* Hero
* Support
* Detail
* CTA

## 3.3 Interaction Thesis

* 2–3 motions clave

---

# 🧱 4. BEAUTIFUL DEFAULTS

* Composición antes que componentes
* Hero full-bleed
* Marca dominante
* Copy corto
* Espacio y jerarquía antes que decoración
* Máximo 2 tipografías
* 1 color de acento
* No cards por defecto
* Primera pantalla = póster

---

# 🌐 5. LANDING PAGE PATTERN

## Flujo

1. Hero
2. Support
3. Detail
4. Final CTA

---

## Hero Rules

* 1 composición
* Full-bleed
* Brand > headline > body > CTA
* No cards
* No stats
* No clutter

---

## Viewport Budget

* Todo cabe en primera pantalla
* Header cuenta
* Evitar scroll inicial innecesario

---

## Tests

* Brand test
* Image test
* Scan test

---

# 🖥️ 6. PRODUCT UI PATTERN

## Reglas

* Utility copy
* Sin hero (por defecto)
* Workspace primero
* Layout:

  * navegación
  * contenido principal
  * contexto secundario
* Alta densidad clara
* Pocos colores
* Cards solo si interacción

---

## Anti-patrones

* Dashboard de cards
* Gradientes decorativos
* Colores compitiendo
* Iconos inútiles

---

# 🖼️ 7. IMAGERY RULES

* Imagen = narrativa
* Preferir fotos reales
* Evitar abstracción como principal
* Evitar texto dentro de imagen
* No collage → múltiples imágenes
* Debe existir ancla visual real

---

# ✍️ 8. COPY RULES

## Marketing

* Lenguaje de producto
* Headline fuerte
* Frase corta
* Sin repetición
* Cada sección tiene función

---

## Product UI

* Copy funcional
* Orientado a acción
* Nada aspiracional
* Nada de marketing

---

# 🎬 9. MOTION RULES

* 2–3 motions mínimos:

  * entrada
  * scroll
  * interacción
* Debe mejorar jerarquía
* Debe funcionar en móvil
* Debe ser eliminable

---

# 🔍 10. VALIDATION LOOP

* Render
* Multi viewport
* Overlaps
* Navegación
* Contraste
* Fidelidad visual

---

# 🧪 11. LITMUS CHECKS

* Marca clara
* Imagen fuerte
* Escaneable
* 1 objetivo por sección
* Cards justificadas
* Motion útil
* Sin sombras sigue siendo bueno

---

# 🧠 12. PROMPTS REUTILIZABLES

## 12.1 System Prompt (Base)

Aplicar siempre:

* design contract
* anti-patterns
* composición

---

## 12.2 Pre-build Prompt

```text
Define:
- visual thesis
- content plan
- interaction thesis
```

---

## 12.3 Constraints Prompt

```text
- 1 H1
- max 6 secciones
- 2 tipografías
- 1 color acento
- 1 CTA principal
```

---

## 12.4 Landing Prompt

```text
Estructura:
Hero → Support → Detail → CTA
```

---

## 12.5 Product UI Prompt

```text
- Utility copy
- Sin hero
- Workspace primero
```

---

## 12.6 Image Strategy Prompt

```text
- usar assets existentes
- si no, generar
- no usar imágenes web
```

---

## 12.7 Layout Safety Prompt

```text
No solapar elementos clave en ningún viewport
```

---

# 🧩 13. AGENT PATTERNS

## Pattern 1 — Design Contract

Sistema global de reglas

## Pattern 2 — Pre-Build Thinking

Planificación antes de generar

## Pattern 3 — Landing Generator

Narrativa estructurada

## Pattern 4 — Product Generator

UI funcional

## Pattern 5 — Visual Strategy

Gestión de imágenes

## Pattern 6 — Validation Loop

Test automático

---

# 🏷️ TAG

frontend/prompt-contracts

---

# 🚀 CONCLUSIÓN

Este sistema convierte frontend en:

👉 contrato
👉 narrativa
👉 sistema
👉 verificación

No es generación libre.

Es **dirección de arte programática para agentes**.

---
