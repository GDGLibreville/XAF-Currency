# XAF Currency Library 💰

[![npm version](https://badge.fury.io/js/xaf-currency.svg)](https://badge.fury.io/js/xaf-currency)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-Ready-blue.svg)](https://www.typescriptlang.org/)

Une librairie TypeScript/JavaScript moderne pour gérer les conversions, arrondis et affichages de la monnaie XAF (Franc CFA).

> **Projet opensource de la communauté [Google Developers Group Libreville](https://gdg.community.dev/gdg-libreville/)**

## 🚀 Fonctionnalités

- ✅ **Conversion de devises** : Support des principales devises (EUR, USD, etc.)
- ✅ **Formatage intelligent** : Affichage localisé avec séparateurs
- ✅ **Arrondis précis** : Gestion des règles d'arrondi monétaire
- ✅ **TypeScript natif** : Types complets et sécurisés
- ✅ **Zéro dépendance** : Léger et performant
- ✅ **Extensible** : Architecture modulaire

## 📦 Installation

```bash
# npm
npm install xaf-currency

# yarn
yarn add xaf-currency

# pnpm
pnpm add xaf-currency
```

## 🔧 Utilisation rapide

```typescript
import { XAFCurrency } from 'xaf-currency';

// Formatage
XAFCurrency.format(150000); // "150 000 FCFA"

// Conversion
XAFCurrency.fromEUR(100); // Convertit 100€ en FCFA

// Arrondi
XAFCurrency.round(1234.56, 'nearest'); // Arrondi au plus proche
```

## 📋 API

### Méthodes principales

| Méthode | Description | Exemple |
|---------|-------------|---------|
| `format(amount, options?)` | Formate un montant | `format(1000) // "1 000 FCFA"` |
| `fromEUR(amount, rate?)` | Convertit depuis l'Euro | `fromEUR(100) // Montant en FCFA` |
| `fromUSD(amount, rate?)` | Convertit depuis le Dollar | `fromUSD(100) // Montant en FCFA` |
| `round(amount, method)` | Arrondit selon la méthode | `round(1.55, 'up') // 2` |

### Options de formatage

```typescript
interface FormatOptions {
  locale?: string;           // Locale (défaut: 'fr-GA')
  showCurrency?: boolean;    // Afficher "FCFA" (défaut: true)
  separator?: string;        // Séparateur milliers (défaut: ' ')
  decimals?: number;         // Nombre de décimales (défaut: 0)
}
```

## 🌍 Contribution

Nous encourageons les contributions de la communauté ! Consultez notre [guide de contribution](CONTRIBUTING.md).

### Développement local

```bash
# Cloner le projet
git clone https://github.com/GDGLibreville/XAF-Currency.git
cd xaf-currency

# Installer les dépendances
npm install

# Lancer les tests
npm test

# Build
npm run build
```

## 📊 Roadmap

- [ ] Support des crypto-monnaies
- [ ] API de taux de change en temps réel
- [ ] Plugin pour React/Vue/Angular
- [ ] CLI pour conversions rapides
- [ ] Support mobile (React Native)

## 🤝 Communauté

- **Discord**: [GDG Libreville](https://discord.gg/gdg-libreville)
- **Twitter**: [@GDGLibreville](https://x.com/gdglibreville?lang=fr)
- **Meetup**: [GDG Libreville Events](https://gdg.community.dev/gdg-libreville/)

## 📄 Licence

MIT © [Google Developers Group Libreville](https://gdg.community.dev/gdg-libreville/)

## 🙏 Remerciements

Merci à tous les contributeurs qui ont rendu ce projet possible !

---

**Fait avec ❤️ par la communauté GDG Libreville**