name: Report de bug
description: Report un bug du serveur
title: "[BUG] "
labels: 
  - bug
  - nouveau
assignees: []

body:
  - type: checkboxes
    id: searched
    attributes:
      label: Confirmation
      options:
        - label: "J'ai bien vérifié si le bug a déjà été report"
          required: true
  - type: input
    id: pseudo
    attributes:
      label: Pseudo en jeu
    validations:
      required: true
  - type: input
    id: discord
    attributes:
      label: Pseudo discord
    validations:
      required: true
  - type: textarea
    id: what-happened
    attributes:
      label: Que s'est-il passé ?
      description: Une description claire et concise de la nature du bug.
    validations:
      required: true
  - type: textarea
    id: step_to_reproduce
    attributes:
      label: Étapes à suivre pour reproduire le bug
      description: 1. Faire '...', 2. Cliquer sur '...' ...
    validations:
      required: true
  - type: textarea
    id: what-should-happened
    attributes:
      label: 'Qu''aurait-il dû arriver ?'
      description: 'Une description claire et concise de ce que ça doit faire si ce n''était pas un bug.'
    validations:
      required: true
  - type: input
    id: date
    attributes:
      label: Date et heure de la production du bug
    validations:
      required: true
  - type: dropdown
    id: server
    validations:
      required: true
    attributes:
      label: Serveur
      description: Sur quel serveur est-ce arrivé ?
      options:
        - Spawn
        - Hub
        - Island
        - Proxy
  - type: textarea
    id: video-screen
    attributes:
      label: 'Screen / vidéo'
      description: 'Le cas échéant, ajoutez des captures d''écran et/ou vidéos pour expliquer votre problème'
    validations:
      required: false  
  - type: textarea
    id: more-info
    attributes:
      label: 'Information supplémentaire'
      description: 'Ajoutez ici tout autre contexte relatif au problème.'
    validations:
      required: false      
