# Projet de TicTacToe

Ceci est un jeu en CSharpe, reproduisant le jeu physique du meme nom. Le principe etant d'alligner 3 meme forme (rond ou carre) pour gagner!

## Prérequis:

* Visual Studio (ici version 2019)

## Documentation:

A la suite vous trouverez une documentation detaille de la programmation de ce projet:


### Le netoyage de la grille de jeu:

```
private void recommencer()
        {
            for (int i = 0; i <= tblbtn3X3.GetUpperBound(0); i++)
            {
                for (int l = 0; l <= tblbtn3X3.GetUpperBound(1); l++)
                {
                    if (tblbtn3X3[i,l] == "X" || tblbtn3X3[i, l] == "O")
                    {
                        tblbtn3X3[i, l] = "";
                    }
                    
                }
            }
            
        }
```

..* Premiere boucle FOR:
  Elle sert ici a se deplacer entre les lignes de la grilles de jeu (tblbtn3x3).
..* Deuxieme boucle FOR:
  Elle sert ici a se deplacer entre les colonnes de la grilles de jeu (tblbtn3x3).
..* Resultat:
  La conbinaison de ces deux boucles permette de passer par toute les cases du tableau afin de leur entrer une valeur vide ("```tblbtn3X3[i, l] = "";```") pour recommencer le jeu.
  
#### Cheat Sheet utiliser pour la redaction de cette documentation:

  [CheatSheet Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "Wiki Markdown")
