# Explication de l'Analyse en Composantes Principales (ACP)

1. **Chargement des données** :
   - Nous avons chargé les données depuis un fichier CSV contenant des variables numériques et textuelles.
   - Nous avons extrait les variables numériques (PAO, PAA, VIO, etc.) pour les analyses suivantes.

2. **Standardisation des données** :
   - Avant d'appliquer l'ACP, nous avons standardisé les données à l'aide du `StandardScaler` de `sklearn`.
   - La standardisation transforme les données de manière à ce que chaque variable ait une moyenne de 0 et un écart-type de 1.
   - Cela permet d'éviter que les variables avec des plages de valeurs plus larges (comme PAO) n'influencent de manière disproportionnée le modèle.

3. **Application de l'ACP** :
   - Nous avons appliqué l'ACP (Analyse en Composantes Principales) sur les données standardisées.
   - L'ACP permet de réduire la dimensionnalité tout en conservant l'essentiel de la variance dans les données.

4. **Calcul des valeurs propres et de la variance expliquée** :
   - Nous avons calculé les **valeurs propres** (eigenvalues) qui indiquent l'importance de chaque composante principale.
   - Ensuite, nous avons calculé le **pourcentage de variance expliquée** par chaque composante, ce qui nous aide à comprendre l'impact de chaque composante sur les données.
   - Nous avons également calculé la **variance cumulée** pour voir combien de variance est expliquée par les premières composantes principales.

5. **Résultats** :
   - Les **valeurs propres** indiquent combien de variance chaque composante principale capte.
   - Le **pourcentage de variance** montre la proportion de variance expliquée par chaque composante.
   - La **variance cumulée** nous permet de savoir combien de variance totale est expliquée par un certain nombre de composantes.

6. **Interprétation** :
   - Les premières composantes principales expliquent la majeure partie de la variance (plus de 77% pour la première composante).
   - Cela montre que quelques composantes principales suffisent pour représenter une grande partie de l'information contenue dans les données.

Ces étapes permettent de réduire la complexité des données tout en conservant l'essentiel de l'information.
