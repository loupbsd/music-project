# Projet de piano virtuel pour Strudel

Ce dépôt héberge les fichiers audio d'un piano personnalisé (37 notes, de C3 à C6). Ces échantillons sont destinés à être utilisés comme instrument dans l'environnement de live coding [Strudel](https://strudel.cc/).

## Fonctionnement

Les fichiers `.wav` sont hébergés publiquement via GitHub Pages. Chaque note dispose ainsi de sa propre URL, ce qui permet à Strudel de charger les sons directement depuis le navigateur. Il n'est donc plus nécessaire de configurer ou d'exécuter un serveur local pour utiliser cet instrument.

## Utilisation

Pour intégrer ce piano dans un projet Strudel, copiez le dictionnaire d'échantillons suivant au début de votre script :

```javascript
samples({
  'mon_piano': {
    'c3': '[https://loupbsd.github.io/music-project/1.wav](https://loupbsd.github.io/music-project/1.wav)', 
    'c#3': '[https://loupbsd.github.io/music-project/2.wav](https://loupbsd.github.io/music-project/2.wav)', 
    'd3': '[https://loupbsd.github.io/music-project/3.wav](https://loupbsd.github.io/music-project/3.wav)', 
    'd#3': '[https://loupbsd.github.io/music-project/4.wav](https://loupbsd.github.io/music-project/4.wav)', 
    'e3': '[https://loupbsd.github.io/music-project/5.wav](https://loupbsd.github.io/music-project/5.wav)', 
    'f3': '[https://loupbsd.github.io/music-project/6.wav](https://loupbsd.github.io/music-project/6.wav)',
    'f#3': '[https://loupbsd.github.io/music-project/7.wav](https://loupbsd.github.io/music-project/7.wav)', 
    'g3': '[https://loupbsd.github.io/music-project/8.wav](https://loupbsd.github.io/music-project/8.wav)', 
    'g#3': '[https://loupbsd.github.io/music-project/9.wav](https://loupbsd.github.io/music-project/9.wav)', 
    'a3': '[https://loupbsd.github.io/music-project/10.wav](https://loupbsd.github.io/music-project/10.wav)', 
    'a#3': '[https://loupbsd.github.io/music-project/11.wav](https://loupbsd.github.io/music-project/11.wav)', 
    'b3': '[https://loupbsd.github.io/music-project/12.wav](https://loupbsd.github.io/music-project/12.wav)',
    
    'c4': '[https://loupbsd.github.io/music-project/13.wav](https://loupbsd.github.io/music-project/13.wav)', 
    'c#4': '[https://loupbsd.github.io/music-project/14.wav](https://loupbsd.github.io/music-project/14.wav)', 
    'd4': '[https://loupbsd.github.io/music-project/15.wav](https://loupbsd.github.io/music-project/15.wav)', 
    'd#4': '[https://loupbsd.github.io/music-project/16.wav](https://loupbsd.github.io/music-project/16.wav)', 
    'e4': '[https://loupbsd.github.io/music-project/17.wav](https://loupbsd.github.io/music-project/17.wav)', 
    'f4': '[https://loupbsd.github.io/music-project/18.wav](https://loupbsd.github.io/music-project/18.wav)',
    'f#4': '[https://loupbsd.github.io/music-project/19.wav](https://loupbsd.github.io/music-project/19.wav)', 
    'g4': '[https://loupbsd.github.io/music-project/20.wav](https://loupbsd.github.io/music-project/20.wav)', 
    'g#4': '[https://loupbsd.github.io/music-project/21.wav](https://loupbsd.github.io/music-project/21.wav)', 
    'a4': '[https://loupbsd.github.io/music-project/22.wav](https://loupbsd.github.io/music-project/22.wav)', 
    'a#4': '[https://loupbsd.github.io/music-project/23.wav](https://loupbsd.github.io/music-project/23.wav)', 
    'b4': '[https://loupbsd.github.io/music-project/24.wav](https://loupbsd.github.io/music-project/24.wav)',

    'c5': '[https://loupbsd.github.io/music-project/25.wav](https://loupbsd.github.io/music-project/25.wav)', 
    'c#5': '[https://loupbsd.github.io/music-project/26.wav](https://loupbsd.github.io/music-project/26.wav)', 
    'd5': '[https://loupbsd.github.io/music-project/27.wav](https://loupbsd.github.io/music-project/27.wav)', 
    'd#5': '[https://loupbsd.github.io/music-project/28.wav](https://loupbsd.github.io/music-project/28.wav)', 
    'e5': '[https://loupbsd.github.io/music-project/29.wav](https://loupbsd.github.io/music-project/29.wav)', 
    'f5': '[https://loupbsd.github.io/music-project/30.wav](https://loupbsd.github.io/music-project/30.wav)',
    'f#5': '[https://loupbsd.github.io/music-project/31.wav](https://loupbsd.github.io/music-project/31.wav)', 
    'g5': '[https://loupbsd.github.io/music-project/32.wav](https://loupbsd.github.io/music-project/32.wav)', 
    'g#5': '[https://loupbsd.github.io/music-project/33.wav](https://loupbsd.github.io/music-project/33.wav)', 
    'a5': '[https://loupbsd.github.io/music-project/34.wav](https://loupbsd.github.io/music-project/34.wav)', 
    'a#5': '[https://loupbsd.github.io/music-project/35.wav](https://loupbsd.github.io/music-project/35.wav)', 
    'b5': '[https://loupbsd.github.io/music-project/36.wav](https://loupbsd.github.io/music-project/36.wav)',

    'c6': '[https://loupbsd.github.io/music-project/37.wav](https://loupbsd.github.io/music-project/37.wav)'
  }
});
