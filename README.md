
> **Attention :** n'utilisez pas ces dispositifs sans avoir vous même vérifié
> leur code source. Vous risqueriez de transmettre involontairement des données
> personnelles.
> 
# Générateur d'attestation de déplacement dérogatoire

Les fichiers de ce dépôt proviennent pour tout ou partie, d'une analyse du site
[deplacement-covid-19](https://media.interieur.gouv.fr/deplacement-covid-19/)

Ils ont pour objectif de **permettre la comprehension** du fonctionnement du
générateur d'attestations.

## Les fichiers importants

### [certificate.js](certificate.js)

Ce fichier est une source re-générée par les outils de développement d'un
navigateur web, depuis le fichier map :  
`/deplacement-covid-19/certificate.xxxxxxxx.js.map`

C'est le script principal qui génère un fichier PDF en combinant :

- un PDF de fond pré-existant,
- les informations saisis dans un formulaire

## Liens externes

### Bibliothèques mises en oeuvre

- [bootstrap](https://www.npmjs.com/package/bootstrap)
- [pdf-lib](https://www.npmjs.com/package/pdf-lib)
- [qrcode](https://www.npmjs.com/package/qrcode)

### Autres exploitations du code source

- https://github.com/ghys/attestation-cmdline
- https://github.com/fix/covid-certificate

## Questionnements

La page html charge, en plus du script de génération d'attestation, plusieurs
fichiers JavaScript dont le rôle et le fonctionnement reste à déterminer.
Notemment :

- https://media.interieur.gouv.fr/_Incapsula_Resource
