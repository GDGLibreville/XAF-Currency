# Guide de Contribution - XAF Currency Library

Merci de votre intérêt pour contribuer au projet XAF Currency ! Ce guide vous aidera à bien commencer.

## 🤝 Comment contribuer

### Types de contributions

- 🐛 **Corrections de bugs**
- ✨ **Nouvelles fonctionnalités**
- 📚 **Documentation**
- 🧪 **Tests**
- 🎨 **Améliorations UI/UX**
- 🌐 **Traductions**

### Avant de commencer

1. Consultez les [issues existantes](https://github.com/gdg-libreville/xaf-currency/issues)
2. Ouvrez une nouvelle issue pour discuter des changements majeurs
3. Rejoignez notre [Discord GDG Libreville](https://discord.gg/gdg-libreville) pour échanger

## 🚀 Configuration de l'environnement

### Prérequis

- Node.js ≥ 16.0.0
- npm ≥ 7.0.0 ou yarn ≥ 1.22.0
- Git

### Installation

```bash
# 1. Forker le projet sur GitHub

# 2. Cloner votre fork
git clone https://github.com/VOTRE_USERNAME/xaf-currency.git
cd xaf-currency

# 3. Ajouter le remote upstream
git remote add upstream https://github.com/gdg-libreville/xaf-currency.git

# 4. Installer les dépendances
npm install

# 5. Créer une branche pour votre contribution
git checkout -b feature/ma-nouvelle-fonctionnalite
```

### Scripts disponibles

```bash
# Développement avec watch
npm run dev

# Tests
npm test
npm run test:watch
npm run test:coverage

# Linting et formatage
npm run lint
npm run lint:fix
npm run format

# Build
npm run build

# Types checking
npm run type-check
```

## 📝 Standards de développement

### Structure du projet

```
xaf-currency/
├── src/
│   ├── core/           # Logique métier principale
│   ├── utils/          # Utilitaires
│   ├── types/          # Définitions TypeScript
│   └── index.ts        # Point d'entrée
├── tests/              # Tests unitaires
├── docs/               # Documentation
└── examples/           # Exemples d'utilisation
```

### Conventions de code

#### TypeScript/JavaScript

- Utiliser **TypeScript** strict
- **ESLint** + **Prettier** pour le formatage
- **CamelCase** pour les variables et fonctions
- **PascalCase** pour les classes et interfaces
- **SCREAMING_SNAKE_CASE** pour les constantes

```typescript
// ✅ Bon
const exchangeRate = 655.957;
class CurrencyConverter { }
interface FormatOptions { }
const DEFAULT_LOCALE = 'fr-GA';

// ❌ Mauvais
const exchange_rate = 655.957;
class currencyConverter { }
interface formatoptions { }
const default_locale = 'fr-GA';
```

#### Tests

- Utiliser **Jest** pour les tests
- Couverture de code ≥ 90%
- Tests unitaires pour chaque fonction publique
- Nommage des tests : `should [action] when [condition]`

```typescript
describe('XAFCurrency.format', () => {
  it('should format amount with default options', () => {
    expect(XAFCurrency.format(150000)).toBe('150 000 FCFA');
  });
  
  it('should format amount without currency symbol when showCurrency is false', () => {
    expect(XAFCurrency.format(150000, { showCurrency: false })).toBe('150 000');
  });
});
```

#### Documentation

- **JSDoc** pour toutes les fonctions publiques
- Exemples d'utilisation dans les commentaires
- README à jour avec les nouvelles fonctionnalités

```typescript
/**
 * Formate un montant en FCFA avec les options spécifiées
 * 
 * @param amount - Montant à formater
 * @param options - Options de formatage
 * @returns Montant formaté
 * 
 * @example
 * ```typescript
 * XAFCurrency.format(150000); // "150 000 FCFA"
 * XAFCurrency.format(150000, { showCurrency: false }); // "150 000"
 * ```
 */
```

### Git Workflow

#### Messages de commit

Format : `type(scope): description`

**Types :**
- `feat`: Nouvelle fonctionnalité
- `fix`: Correction de bug  
- `docs`: Documentation
- `style`: Formatage, point-virgules manquants, etc.
- `refactor`: Refactoring de code
- `test`: Ajout de tests
- `chore`: Tâches de maintenance

**Exemples :**
```bash
feat(core): add currency conversion from USD
fix(format): handle negative amounts correctly  
docs(readme): update installation instructions
test(utils): add tests for rounding functions
```

#### Pull Requests

1. **Titre clair** : Résumez le changement en une ligne
2. **Description détaillée** : Expliquez le pourquoi et le comment
3. **Tests** : Ajoutez/mettez à jour les tests
4. **Documentation** : Mettez à jour si nécessaire
5. **Screenshots** : Si pertinent (UI/UX)

**Template de PR :**
```markdown
## 📝 Description
Brève description du changement

## 🔄 Type de changement
- [ ] Bug fix
- [ ] Nouvelle fonctionnalité  
- [ ] Breaking change
- [ ] Documentation

## ✅ Checklist
- [ ] Tests ajoutés/mis à jour
- [ ] Documentation mise à jour
- [ ] Code formaté (npm run format)
- [ ] Tests passent (npm test)
- [ ] Build fonctionne (npm run build)

## 🧪 Comment tester
Instructions pour tester le changement
```

## 🏆 Reconnaissance

### Hall of Fame

Les contributeurs seront ajoutés au README avec leurs contributions !

### Récompenses GDG

- Stickers GDG Libreville
- Mentions sur nos réseaux sociaux
- Invitations aux événements spéciaux
- Opportunités de speaker aux meetups

## 📞 Support

- **Issues GitHub** : Pour les bugs et demandes de fonctionnalités
- **Discord GDG** : Pour les discussions et questions
- **Email** : gdg.libreville@gmail.com

## 📋 Checklist avant soumission

- [ ] Code formaté avec Prettier
- [ ] Linting passé sans erreurs  
- [ ] Tests unitaires ajoutés/mis à jour
- [ ] Tests passent (couverture ≥ 90%)
- [ ] Documentation mise à jour
- [ ] Build fonctionne
- [ ] Messages de commit suivent les conventions
- [ ] PR template rempli

---

**Merci de contribuer à XAF Currency ! Ensemble, créons la meilleure librairie monétaire pour l'Afrique centrale ! 🚀**