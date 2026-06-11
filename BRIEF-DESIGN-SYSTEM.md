# Brief Design System — Ornetti Data Services

> Document de référence pour générer un design system dans **Claude Design**.
> Identité verrouillée : **bleu marine + pêche**. Source des tokens : `index.html`.

---

## 1. ADN de marque

**Ornetti Data Services** — conseil indépendant en **data & IA** (data engineering,
dataviz, ateliers IA), au service du secteur public comme privé.

### Le positionnement en une phrase
> *« La donnée, au service de ce qui compte vraiment. »*

La rigueur technique de la data, réchauffée par une approche **artisanale et humaine**.

### Les 3 piliers de personnalité

| Pilier | Ce que ça veut dire | Traduction visuelle |
|--------|--------------------|--------------------|
| **Expertise de terrain** | Un praticien qui met les mains dans la donnée, pas un cabinet hors-sol. Concret, opérationnel, « ça marche pour de vrai ». | Maquettes de projets réels visibles, chiffres tangibles, captures de dataviz, pas d'abstraction gratuite. |
| **Ancrage & solidité** | Fiable, posé, institutionnel. On confie ses données sensibles (Éducation Nationale, régions) à quelqu'un de sérieux. | Le bleu marine comme socle, typographie serif assise, mises en page aérées et stables, ombres douces (jamais clinquant). |
| **Relationnel & humain** | Sur-mesure, proximité, on parle à une personne — pas à une marque. Chaleur, écoute, accessibilité. | La pêche comme accent chaleureux, le « je » assumé, ton direct, photo/médaillon humain, langage clair sans jargon. |

### Tensions à tenir (l'équilibre de la marque)
- **Sérieux institutionnel** ⟷ **chaleur artisanale** → ni froid corporate, ni amateur.
- **Pointu techniquement** ⟷ **accessible** → on vulgarise sans simplifier à outrance.
- **Indépendant / petite structure** ⟷ **crédible sur de gros enjeux** → la preuve par les réalisations.

### Ton éditorial
- **Direct et incarné** : le « je », pas le « nous » corporate.
- **Clair avant d'être technique** : on explique la valeur (« ce que ça change »)
  avant la mécanique.
- **Concret** : des verbes d'action, des résultats, des cas d'usage — pas de
  promesses vagues.
- **Chaleureux mais pro** : accessible et humain, jamais familier ni survendeur.

---

## 2. Couleurs

Identité tirée du logo. Le **marine est le socle**, le **pêche est l'accent
signature** (jamais une surface dominante).

| Token | Hex | Usage |
|-------|-----|-------|
| `navy` | `#1B2A6B` | **Couleur principale** — texte foncé, titres, accents |
| `navy-dark` | `#101A50` | Fonds de sections sombres (hero, services, contact) |
| `navy-light` | `#2D3F8A` | Variantes, hovers, badges secondaires |
| `peach` | `#D4956A` | **Accent signature** — CTA, liens, highlights |
| `peach-light` | `#E8B48A` | Hover des éléments pêche |
| `peach-pale` | `#F5EBE0` | Fonds doux, médaillons |
| `white` | `#FFFFFF` | Fond principal |
| `gray-light` | `#F7F7F8` | Fonds de sections alternés |
| `text-medium` | `#4A5568` | Corps de texte |
| `text-light` | `#718096` | Texte secondaire, légendes |

**Règles d'usage**
- Alternance des sections : `blanc → marine foncé → blanc → gris clair → marine foncé`.
- Le pêche en surface = toujours en transparence douce : `rgba(212,149,106, 0.08 → 0.15)`.
- Jamais de noir pur : les ombres et textes profonds sont teintés marine.

---

## 3. Typographie

- **Titres :** `DM Serif Display` (serif éditorial, italique disponible) → la chaleur.
- **Corps & UI :** `Inter` (sans-serif) → poids 300 / 400 / 500 / 600 / 700.

| Rôle | Taille | Détails |
|------|--------|---------|
| Hero title | `clamp(2.8rem, 6vw, 5rem)` | line-height `1.08`, DM Serif |
| Titre de section | `clamp(1.9rem, 3.5vw, 2.75rem)` | line-height `1.18`, DM Serif |
| Corps | `1rem – 1.05rem` | line-height `1.6 – 1.8`, Inter |
| Eyebrow / label | `0.7 – 0.78rem` | poids 700, **UPPERCASE**, letter-spacing `0.08 – 0.14em`, en pêche |

---

## 4. Formes & élévation

- **Boutons / pills :** `border-radius: 50px` (entièrement arrondis), poids 600.
- **Cartes :** `border-radius: 14 – 20px`.
- **Médaillons / avatars :** cercles (`border-radius: 50%`).
- **Ombres** — toujours teintées marine :
  - Carte au repos : `0 6px 24px rgba(27,42,107,0.07)`
  - Carte au survol : `0 16px 48px rgba(27,42,107,0.13)`
  - CTA pêche : `0 10px 28px rgba(212,149,106,0.4)`

---

## 5. Interactions & mouvement

- Transitions douces `0.2s – 0.35s` (background, transform, box-shadow).
- Hover = légère élévation (`translateY`) + ombre renforcée.
- **Hero signature :** animation canvas — réseau de nœuds (particules pêche sur
  fond marine). Métaphore : la donnée connectée, vivante.
- Révélations au scroll via `IntersectionObserver`.
- Nav sticky, fond translucide `rgba(255,255,255,0.94)`.

---

## 6. Bibliothèque de composants à dériver

Bouton primaire (pêche) · Bouton secondaire (outline) · Pill-label uppercase ·
Carte service (sur fond sombre) · Carte projet (header dégradé pastel) ·
Badge techno · Carte contact · Switch de langue FR / EN · Médaillon logo ·
Stat / chiffre-clé.

---

## 7. Do / Don't

| ✅ Do | ❌ Don't |
|-------|---------|
| Marine en socle, pêche en accent ponctuel | Pêche en aplat sur de grandes surfaces |
| Ombres douces teintées marine | Ombres noires, contrastes durs |
| Coins arrondis, formes posées | Angles vifs, look « tech froid » |
| Chiffres et réalisations concrètes | Promesses abstraites sans preuve |
| Ton direct, « je », humain | Jargon corporate, « nous » impersonnel |
| Espace, respiration, lisibilité | Densité, surcharge d'effets |
