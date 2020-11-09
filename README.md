<p align="center">
    <img src="https://github.com/sl-samyazirou/git-academy-workshop/blob/main/img/logo.png?raw=true" alt="Logo" width="245" height="70">
</p>

##### Bienvenue dans la git academy special github. Nous allons effectuer quelques exercices pratiques afin de découvrir quelques commandes utiles afin d'utiliser git au mieux dans nos projets. Il est fondamental d'être à l'aise sur cet outil et j'espère que vous l'êtes déjà ou que vous le deviendrez très prochainement.

## Liste des branches

Chaque branches contient des commits nommé par des numéros. Ces numéros permettent de mieux s'y retrouver dans l'exercice qui va suivre.

![Branches Screen Shot](https://github.com/sl-samyazirou/git-academy-workshop/blob/main/img/gitbranches.PNG?raw=true "Branches screenshot")

## Pré-requis

Il est conseillé de fork le projet pour pour push le code ensuite sur son propre repository.

## Installation

1. Cloner le dossier

```sh
git clone git@github.com:sl-samyazirou/git-academy-workshop.git
```

2. Récupérer toutes les branches

```sh
cd git-academy-workshop; git checkout master ; remote=origin ; for brname in `git branch -r | grep $remote | grep -v master | grep -v HEAD | awk '{gsub(/^[^\/]+\//,"",$1); print $1}'`; do git branch -D $brname ; git checkout -b $brname $remote/$brname ; done ;
```

## Exercice

Voici les intructions, elles sont toutes accompagnés de la liste de commit attendu une fois résolue.

### 1) Rebase feature1 in master

- Resultat Attendu

![Exercice 1](https://github.com/sl-samyazirou/git-academy-workshop/blob/main/img/1.PNG?raw=true "Exercice 1")

### 2) Rebase feature2 in master

- Resultat Attendu

![Exercice 2](https://github.com/sl-samyazirou/git-academy-workshop/blob/main/img/2.PNG?raw=true "Exercice 2")

### 3) Keep only odd number

- Resultat Attendu

![Exercice 3](https://github.com/sl-samyazirou/git-academy-workshop/blob/main/img/3.PNG?raw=true "Exercice 3")

### 4) Rebase feature3 in master

- Resultat Attendu

![Exercice 4](https://github.com/sl-samyazirou/git-academy-workshop/blob/main/img/4.PNG?raw=true "Exercice 4")

### 5) Pick commit 42 into master

- Resultat Attendu

![Exercice 5](https://github.com/sl-samyazirou/git-academy-workshop/blob/main/img/5.PNG?raw=true "Exercice 5")

### 6) Rename commit 42 to 8

- Resultat Attendu

![Exercice 6](https://github.com/sl-samyazirou/git-academy-workshop/blob/main/img/6.PNG?raw=true "Exercice 6")

## License

Distributed under the MIT License. See `LICENSE` for more information.
