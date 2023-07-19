 <style>
    .tips {
        background-color: #0374fc;
        padding: 10px;
        border: 2px solid black;
    }

    .warn {
        background-color: #ed5f00;
        padding: 10px;
        border: 2px solid black;
    }

    .note {
        background-color: #4aa859;
        padding: 10px;
        border: 2px solid black;
    }
    code {
        margin: 20px;
    }
</style>


# Guide LaTex 

LaTeX est un langage et un système de composition de documents. 
Pour faciliter l'usage du "processeur de texte", il existe de nombreuses macrocommandes. 

Une fois le texte rédigé dans un fichier `.tex`, l'utilisateur n'a plus qu'à compiler le fichier pour qu'un PDF sois généré. 

### Quel éditeur utiliser pour écrire avec LaTex ? 

Vous pouvez écrire en LaTex avec n'importe quel éditeur, y compris un simple Bloc-Note. 
Toutefois, utiliser un éditeur compatible voir fait pour le LaTex vous simplifiera la tâche, notamment grâce à une autocomplétion du code, ou encore la compilation avec un simple bouton. 
Quelques exemples d'éditeurs : 
- Overleaf 
- Texmaker
- Visual Studio Code, couplé à l'extention [...]

<div class="note">
    ℹ️ Information <br>
    Ce repositories contient plusieurs documents : 
    - Un guide sous format Latex (guideLaTex.tex)
    - Un guide sous format Markdown (Il s'agit de ce document)
    - Un guide sous format PDF, complié à partir du document LaTex
    - Un guide sous format PDF, issu du Markdown
</div>

## 1. Commandes de base 


- `\begin\{document\}` : Commence le document. 

- `\end\{document\}` : Termine le document.

- `\title\{Titre\}` : Définit le titre du document.

- `\author\{Auteur\}` : Définit l'auteur du document.

- `\date\{Date\}` : Définit la date du document.

- `\maketitle` : Crée le titre du document.

<div class="warn">
⚠️ Attention ⚠️ <br>
Vous devez indiquer systématiquement à LaTex l'encodage que vous souhaitez utiliser (par exemple : UTF-8). <br>
Sinom, des caractères tel que le "é" n'apparaitront pas. <br>
Voici la façon d'indiquer l'encodage à LaTex, à placer au début du documment : <br> 
<code>\usepackage[utf8]{inputenc}</code>
</div>


Voici un exemple de structure de base d'un documment : 

```tex
\documentclass{article}
\usepackage[utf8]{inputenc}

\title{Guide des commandes utiles pour LaTeX}
\author{Wolfyz}
\date{\today}

\begin{document}

% Ici se trouve le contenu de votre document

\end{document}
```

## 2. Commandes de mise en forme

- `\textebf{exemple}` : Met le texte en **gras**
- `textit{texte}` : Met le texte en *italique*.
- `underline{texte}` : Souligne le texte.
- `texttt{texte}` : Met le texte en police à chasse fixe (typewriter font).
- `emph{texte}` : Met en évidence le texte (généralement en italique).
- `textsc{texte}` : Met le texte en petites capitales.


<div class="tips">
    💡 Astuce 💡<br> Vous pouvez placer un commentaire dans un fichier avec le caractère %
</div>


Voici maintenant un petit exemple : 
```tex

\begin{document}

\textbf{Ce texte est en gras} tandis que \textit{celui là est en italique} et \underline{celui là est souligné} .
\end{document}

```

## 3. Commandes de mise en forme 




Paquets

Pour complémenter les fonctions de LaTeX, l’utilisateur peut charger des paquets tiers. Ceux-ci, à l'instar des bibliothèques logicielles, fournissent des commandes supplémentaires, qui vont de simples symboles jusqu’à des fonctionnalités complexes, pouvant impliquer une modification du processus de compilation du document.

Voici quelques exemples de paquets parmi les plus communs :

    babel prend en charge la langue du document, en adaptant la typographie et en fournissant des commandes spécifiques à chaque langue ;
    amsmath, développé par la Société américaine de mathématiques, étend considérablement les possibilités d'édition de formules mathématiques ;
    tikz permet la création d’illustrations vectorielles, telles que des graphiques ;
    graphicx est utilisé pour insérer des images ;
    listings permet l’affichage de code source avec coloration syntaxique ;
    calc fournit un mécanisme de calcul.