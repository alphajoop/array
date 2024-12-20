### **Cours sur les Tableaux en JavaScript pour Débutants**

Un tableau (ou **array** en anglais) est une structure de données utilisée pour stocker plusieurs valeurs dans une seule variable. Les tableaux sont très utiles pour organiser et manipuler des ensembles de données.

---

## **1. Pourquoi utiliser des tableaux ?**

Supposons que tu veux stocker les noms de trois amis : "Ali", "Marie" et "Fatou". Sans tableau, tu devrais créer trois variables distinctes :

```javascript
let ami1 = "Ali";
let ami2 = "Marie";
let ami3 = "Fatou";
```

Avec un tableau, tu peux tout mettre dans **une seule variable** :

```javascript
let amis = ["Ali", "Marie", "Fatou"];
```

---

## **2. Comment créer un tableau ?**

Voici comment déclarer un tableau en JavaScript :

### **Méthode 1 : Tableau avec des valeurs**
```javascript
let fruits = ["Pomme", "Banane", "Mangue"];
```

### **Méthode 2 : Tableau vide**
Tu peux aussi créer un tableau vide et y ajouter des valeurs plus tard :
```javascript
let animaux = [];
animaux.push("Chat"); // Ajoute "Chat"
animaux.push("Chien"); // Ajoute "Chien"
```

---

## **3. Accéder aux éléments d’un tableau**

Les éléments d’un tableau sont accessibles via leur **index**.  
⚠️ **L’index commence toujours à 0** (le premier élément est à l’index 0).

### **Exemple :**
```javascript
let fruits = ["Pomme", "Banane", "Mangue"];
console.log(fruits[0]); // Affiche : Pomme
console.log(fruits[1]); // Affiche : Banane
console.log(fruits[2]); // Affiche : Mangue
```

---

## **4. Modifier les éléments d’un tableau**

Tu peux changer la valeur d’un élément en utilisant son index :
```javascript
let fruits = ["Pomme", "Banane", "Mangue"];
fruits[1] = "Orange"; // Change "Banane" en "Orange"
console.log(fruits); // Affiche : ["Pomme", "Orange", "Mangue"]
```

---

## **5. Longueur d’un tableau**

La propriété `.length` donne le nombre d’éléments dans un tableau :
```javascript
let fruits = ["Pomme", "Banane", "Mangue"];
console.log(fruits.length); // Affiche : 3
```

---

## **6. Ajouter ou supprimer des éléments**

### **Ajouter des éléments**
- **`push`** : ajoute un élément à la fin.
  ```javascript
  let fruits = ["Pomme", "Banane"];
  fruits.push("Mangue"); // Ajoute "Mangue" à la fin
  console.log(fruits); // ["Pomme", "Banane", "Mangue"]
  ```
- **`unshift`** : ajoute un élément au début.
  ```javascript
  fruits.unshift("Orange"); // Ajoute "Orange" au début
  console.log(fruits); // ["Orange", "Pomme", "Banane", "Mangue"]
  ```

### **Supprimer des éléments**
- **`pop`** : supprime le dernier élément.
  ```javascript
  fruits.pop(); // Supprime "Mangue"
  console.log(fruits); // ["Orange", "Pomme", "Banane"]
  ```
- **`shift`** : supprime le premier élément.
  ```javascript
  fruits.shift(); // Supprime "Orange"
  console.log(fruits); // ["Pomme", "Banane"]
  ```

---

## **7. Parcourir un tableau**

Tu peux utiliser une boucle pour parcourir tous les éléments d’un tableau.

### **Exemple avec une boucle `for` :**
```javascript
let fruits = ["Pomme", "Banane", "Mangue"];

for (let i = 0; i < fruits.length; i++) {
    console.log(fruits[i]); // Affiche chaque fruit
}
```

### **Exemple avec une boucle `for...of` :**
```javascript
for (let fruit of fruits) {
    console.log(fruit); // Affiche chaque fruit
}
```

---

## **8. Fonctions utiles pour les tableaux**

### **`indexOf`**
Renvoie l’index d’un élément dans le tableau (ou -1 si l’élément n’est pas trouvé) :
```javascript
let fruits = ["Pomme", "Banane", "Mangue"];
console.log(fruits.indexOf("Banane")); // Affiche : 1
console.log(fruits.indexOf("Orange")); // Affiche : -1 (pas trouvé)
```

### **`slice`**
Crée une copie d’une partie du tableau :
```javascript
let fruits = ["Pomme", "Banane", "Mangue", "Orange"];
let nouveauxFruits = fruits.slice(1, 3); // Copie de l’index 1 à 2
console.log(nouveauxFruits); // ["Banane", "Mangue"]
```

### **`join`**
Convertit un tableau en chaîne de caractères, avec un séparateur :
```javascript
let fruits = ["Pomme", "Banane", "Mangue"];
console.log(fruits.join(", ")); // Affiche : "Pomme, Banane, Mangue"
```

### **`reverse`**
Inverse l’ordre des éléments du tableau :
```javascript
let fruits = ["Pomme", "Banane", "Mangue"];
fruits.reverse();
console.log(fruits); // ["Mangue", "Banane", "Pomme"]
```

---

## **9. Exemple complet**
Voici un petit exemple pratique :
```javascript
let fruits = ["Pomme", "Banane", "Mangue"];

// Ajouter un fruit
fruits.push("Orange");

// Afficher tous les fruits
for (let fruit of fruits) {
    console.log(fruit);
}

// Trouver la position de "Banane"
let index = fruits.indexOf("Banane");
console.log("Banane se trouve à l'index : " + index);

// Supprimer le dernier fruit
fruits.pop();
console.log(fruits);
```

---

Avec ces bases, tu es prêt(e) à manipuler des tableaux en JavaScript ! Veux-tu des exercices pratiques ?