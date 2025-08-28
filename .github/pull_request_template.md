# 🔄 Pull Request - XAF Currency Library

## 📝 Description

<!-- Décrivez clairement ce que fait cette PR -->
Une brève description des changements apportés...

## 🔗 Issue associée

<!-- Référencez l'issue si applicable -->
Fixes #(numéro de l'issue)

## 🎯 Type de changement

<!-- Cochez les cases appropriées -->
- [ ] 🐛 Bug fix (changement non-breaking qui corrige un problème)
- [ ] ✨ Nouvelle fonctionnalité (changement non-breaking qui ajoute une fonctionnalité)
- [ ] 💥 Breaking change (fix ou fonctionnalité qui modifie l'API existante)
- [ ] 📚 Documentation (mise à jour de la documentation uniquement)
- [ ] 🎨 Refactoring (changement de code sans modification de fonctionnalité)
- [ ] ⚡ Performance (amélioration des performances)
- [ ] 🧪 Tests (ajout ou correction de tests)
- [ ] 🔧 Chore (maintenance, configuration, etc.)

## 🚀 Fonctionnalité ajoutée / Bug corrigé

<!-- Décrivez en détail -->
### Avant
<!-- Comment ça fonctionnait avant -->

### Après  
<!-- Comment ça fonctionne maintenant -->

## 💻 Code d'exemple

<!-- Montrez comment utiliser la nouvelle fonctionnalité -->
```typescript
import { XAFCurrency } from 'xaf-currency';

// Exemple d'utilisation
const result = XAFCurrency.newMethod(params);
console.log(result);
```

## 📊 Impact

<!-- Décrivez l'impact de vos changements -->
- **Performance** : ⚡ Amélioration / 🔄 Neutre / 🐌 Dégradation
- **Bundle size** : ⬇️ Diminution / 🔄 Neutre / ⬆️ Augmentation  
- **Breaking changes** : ❌ Non / ⚠️ Mineurs / 💥 Majeurs

## 🧪 Tests

<!-- Décrivez vos tests -->
- [ ] Tests unitaires ajoutés/mis à jour
- [ ] Tests d'intégration ajoutés/mis à jour
- [ ] Tests manuels effectués
- [ ] Couverture de code maintenue (≥ 90%)

### Scénarios testés
<!-- Listez les scénarios de test -->
- [ ] Cas nominal
- [ ] Cas d'erreur
- [ ] Cas limites
- [ ] Régression des fonctionnalités existantes

## 📱 Compatibilité

<!-- Testez sur différents environnements -->
- [ ] **Node.js** (versions LTS supportées)
- [ ] **Browsers** (Chrome, Firefox, Safari, Edge)
- [ ] **TypeScript** (version actuelle)
- [ ] **Frameworks** (React, Vue, Angular si applicable)

## 📋 Checklist

<!-- Vérifiez avant de soumettre -->
### Code
- [ ] Le code suit les conventions du projet
- [ ] Pas de console.log ou code de debug oublié
- [ ] Variables et fonctions bien nommées
- [ ] Code commenté si nécessaire (JSDoc)
- [ ] Pas de duplication de code

### Tests et qualité
- [ ] Tous les tests passent (`npm test`)
- [ ] Pas d'erreurs de linting (`npm run lint`)
- [ ] Pas d'erreurs TypeScript (`npm run type-check`)  
- [ ] Build fonctionne (`npm run build`)
- [ ] Couverture de tests ≥ 90%

### Documentation
- [ ] README mis à jour si nécessaire
- [ ] Documentation API mise à jour
- [ ] CHANGELOG.md mis à jour
- [ ] Exemples de code ajoutés si pertinent

### Git
- [ ] Commits atomiques et bien nommés
- [ ] Branche à jour avec main
- [ ] Pas de merge conflicts

## 📸 Screenshots / Vidéos

<!-- Si applicable, ajoutez des captures d'écran -->
<!-- 
### Avant
[Screenshot]

### Après  
[Screenshot]
-->

## ⚠️ Notes pour les reviewers

<!-- Informations importantes pour la review -->
- Points particuliers à vérifier
- Zones de code sensibles
- Décisions techniques prises
- Compromis effectués

## 🔄 Migration

<!-- Si breaking changes, expliquez comment migrer -->
<!-- 
### Migration depuis v1.x.x

```typescript
// Ancien code
XAFCurrency.oldMethod(params);

// Nouveau code
XAFCurrency.newMethod(params);
```
-->

## ✅ Résultats des tests

<!-- Collez les résultats des tests si pertinent -->
```
✅ All tests passed (XX tests, XX assertions)
✅ Coverage: 95.2% (statements: 95.1%, branches: 94.8%, functions: 96.1%)
```

---

## 🤝 Pour les mainteneurs

<!-- Section pour l'équipe de maintenance -->
- [ ] **Review approuvée** par au moins un mainteneur
- [ ] **Tests CI** passent
- [ ] **Documentation** validée
- [ ] **Breaking changes** documentés
- [ ] **Version bump** nécessaire (patch/minor/major)

### Merge checklist
- [ ] Squash and merge (commits atomiques)
- [ ] Update CHANGELOG.md
- [ ] Tag version si release
- [ ] Deploy documentation
- [ ] Communiquer les breaking changes

---

**Merci de contribuer à XAF Currency ! 🎉**

*Cette PR sera reviewée par l'équipe GDG Libreville dans les plus brefs délais.*