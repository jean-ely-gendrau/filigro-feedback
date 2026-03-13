---
name: Bug report
about: Create a report to help us improve
title: ''
labels: ''
assignees: ''

---

name: 🐛 Signaler un bug
description: Un problème avec filigro.fr ? Décris-le ici.
title: "[Bug] "
labels: ["bug"]
body:
  - type: markdown
    attributes:
      value: |
        Merci de prendre le temps de signaler ce bug. Toutes les informations ci-dessous nous aident à le reproduire et le corriger rapidement.

  - type: textarea
    id: description
    attributes:
      label: Décris le problème
      description: Que s'est-il passé ? Qu'est-ce qui devrait se passer à la place ?
      placeholder: "Ex : Quand je télécharge un PDF filigrané, le document est plus grand que l'original..."
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Étapes pour reproduire
      description: Comment reproduire le bug, étape par étape.
      placeholder: |
        1. Aller sur filigro.fr
        2. Charger un fichier PDF
        3. Cliquer sur "Télécharger"
        4. ...
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: Comportement attendu
      placeholder: "Ex : Le PDF téléchargé devrait avoir la même taille que l'original."
    validations:
      required: true

  - type: dropdown
    id: file_type
    attributes:
      label: Type de fichier concerné
      options:
        - PDF
        - Image (JPG, PNG...)
        - Les deux
        - Autre / Je ne sais pas
    validations:
      required: true

  - type: dropdown
    id: browser
    attributes:
      label: Navigateur utilisé
      options:
        - Chrome
        - Firefox
        - Safari
        - Edge
        - Chrome mobile (Android)
        - Safari mobile (iPhone)
        - Autre
    validations:
      required: true

  - type: textarea
    id: screenshots
    attributes:
      label: Captures d'écran (optionnel)
      description: Glisse une image ici si ça peut aider.

  - type: checkboxes
    id: confirm
    attributes:
      label: Vérification
      options:
        - label: J'ai vérifié que ce bug n'a pas déjà été signalé
          required: true
