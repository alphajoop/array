Voici les solutions aux exercices sur les tableaux en JavaScript :

---

### **Correction de l'Exercice 1 : Création d’un tableau**

```javascript
let fruits = ["Pomme", "Banane", "Mangue"];
console.log(fruits); // Affiche : ["Pomme", "Banane", "Mangue"]
```

---

### **Correction de l'Exercice 2 : Accès aux éléments**

```javascript
console.log(fruits[0]); // Affiche : "Pomme"
console.log(fruits[fruits.length - 1]); // Affiche : "Mangue"
```

---

### **Correction de l'Exercice 3 : Modifier un élément**

```javascript
fruits[1] = "Orange";
console.log(fruits); // Affiche : ["Pomme", "Orange", "Mangue"]
```

---

### **Correction de l'Exercice 4 : Ajouter et supprimer des éléments**

```javascript
fruits.push("Ananas");
fruits.unshift("Fraise");
fruits.pop();
console.log(fruits); // Affiche : ["Fraise", "Pomme", "Orange"]
```

---

### **Correction de l'Exercice 5 : Longueur d’un tableau**

```javascript
console.log(fruits.length); // Affiche : 3
```

---

### **Correction de l'Exercice 6 : Parcourir un tableau**

**Avec une boucle `for` classique** :

```javascript
for (let i = 0; i < fruits.length; i++) {
    console.log(fruits[i]); // Affiche chaque fruit
}
```

**Avec une boucle `for...of`** :

```javascript
for (let fruit of fruits) {
    console.log(fruit); // Affiche chaque fruit
}
```

---

### **Correction de l'Exercice 7 : Trouver un élément**

```javascript
let index = fruits.indexOf("Mangue");
console.log(index); // Affiche : 2
```

---

### **Correction de l'Exercice 8 : Copier une partie du tableau**

```javascript
let nouveauxFruits = fruits.slice(0, 2);
console.log(nouveauxFruits); // Affiche : ["Fraise", "Pomme"]
```

---

### **Correction de l'Exercice 9 : Trier un tableau**

```javascript
let nombres = [5, 2, 9, 1, 6];
nombres.sort((a, b) => a - b); // Tri dans l’ordre croissant
console.log(nombres); // Affiche : [1, 2, 5, 6, 9]
```

---

### **Correction de l'Exercice 10 : Inverser un tableau**

```javascript
fruits.reverse();
console.log(fruits); // Affiche : ["Orange", "Pomme", "Fraise"]
```

---

### **Correction de l'Exercice 11 : Fusionner deux tableaux**

```javascript
let legumes = ["Carotte", "Courgette"];
let aliments = legumes.concat(fruits);
console.log(aliments); // Affiche : ["Carotte", "Courgette", "Orange", "Pomme", "Fraise"]
```

---

### **Correction de l'Exercice 12 : Retirer les doublons**

```javascript
let valeurs = [1, 2, 3, 1, 4, 2];
let uniqueValeurs = [...new Set(valeurs)];
console.log(uniqueValeurs); // Affiche : [1, 2, 3, 4]
```

---