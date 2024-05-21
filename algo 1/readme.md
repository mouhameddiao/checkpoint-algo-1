// Initialiser les compteurs
longueur <- 0
nombre_mots <- 0
nombre_voyelles <- 0

// Définir les voyelles
voyelles <- "aeiouAEIOU"

// Variable pour suivre si nous sommes dans un mot
dans_mot <- FAUX

// Lire la phrase caractère par caractère
Pour chaque caractère dans la phrase FAIRE
longueur <- longueur + 1 // Incrémenter le compteur de longueur pour chaque caractère

    // Compter les voyelles
    Si caractère EST DANS voyelles ALORS
      nombre_voyelles <- nombre_voyelles + 1


    // Compter les mots
    Si caractère = ' ' ALORS
      Si dans_mot EST VRAI ALORS
        nombre_mots <- nombre_mots + 1
        dans_mot <- FAUX

    SINON SI caractère = '.' ALORS
      Si dans_mot EST VRAI ALORS
        nombre_mots <- nombre_mots + 1

      Sortir de la boucle
    SINON
      dans_mot <- VRAI
