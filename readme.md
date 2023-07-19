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

### ℹ️ Information 
    Ce repositories contient plusieurs documents : 
    - Un guide sous format Latex (guideLaTex.tex)
    - Un guide sous format Markdown (Il s'agit de ce document)
    - Un guide sous format PDF, complié à partir du document LaTex
    - Un guide sous format PDF, issu du Markdown


## 1. Commandes de base 


- `\begin\{document\}` : Commence le document. 

- `\end\{document\}` : Termine le document.

- `\title\{Titre\}` : Définit le titre du document.

- `\author\{Auteur\}` : Définit l'auteur du document.

- `\date\{Date\}` : Définit la date du document.

- `\maketitle` : Crée le titre du document.


### ⚠️ Attention ⚠️ <br>
Vous devez indiquer systématiquement à LaTex l'encodage que vous souhaitez utiliser (par exemple : UTF-8). 
Sinom, des caractères tel que le "é" n'apparaitront pas. 
Voici la façon d'indiquer l'encodage à LaTex, à placer au début du documment :  
`\usepackage[utf8]{inputenc}`



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


### 💡 Astuce 💡
Vous pouvez placer un commentaire dans un fichier avec le caractère `%`



Voici maintenant un petit exemple : 
```tex

\begin{document}

\textbf{Ce texte est en gras} tandis que \textit{celui là est en italique} et \underline{celui là est souligné} .
\end{document}

```
