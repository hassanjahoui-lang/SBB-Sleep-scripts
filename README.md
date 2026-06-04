# 💤 Advanced Sleep & Fatigue System - Standalone with iOS Notifications

## 📁 Struttura dei File / Directory Layout
```text
sleep_system/
├── fxmanifest.lua
├── client.lua
├── server.lua
└── html/
    └── index.html
```
🌎 Seleziona la Lingua / Select Language
<details>
<summary>🇮🇹 Italiano (Documentazione)</summary>
🌟 Caratteristiche Principali
Rilevamento Automatico del Framework: Rileva all'avvio se il server esegue ESX, QBCore o Qbox per interfacciarsi automaticamente con i moltiplicatori di fame e sete dei rispettivi core.
Sistema di Fatica Progressiva: La fatica del giocatore si accumula dinamicamente. Correre o sprintare aumenta il valore rapidamente; guidare o camminare lo aumenta in modo moderato.
Colpo di Sonno Forzato (Emote Sleep): Al raggiungimento del 90% di fatica, il giocatore perde i sensi. Lo schermo va in dissolvenza nera e il personaggio viene costretto a terra riproducendo lo scenario nativo di sonno (WORLD_HUMAN_SUNBATHE_BACK) per ricaricare le forze sul posto.
Comando di Riposo /dormi: Consente di riposare intenzionalmente in qualunque momento (a piedi), attivando l'animazione di sonno e velocizzando la rigenerazione dell'energia.
Notifiche in stile iOS 17: Banner di notifica animati che replicano fedelmente l'interfaccia degli iPhone (sfondo Glassmorphism sfocato, icone dinamiche con gradienti colorati in base alla gravità e visualizzazione temporale "adesso").
📥 Installazione
Copia la cartella sleep_system nella directory resources del tuo server.
Apri il file server.cfg e aggiungi la risorsa scrivendo:
code
Cfg
ensure sleep_system
Riavvia il server o avvia la risorsa tramite console scrivendo start sleep_system.
⌨️ Comandi & Interazioni
/dormi (Comando Chat): Avvia o interrompe l'animazione di sonno a terra e lo stato di rigenerazione.
Spia di Allarme (iOS): Viene inviata automaticamente al superamento del 75% di stanchezza per avvisare il giocatore di trovare un luogo idoneo in cui riposare.
📊 Prestazioni (Resmon)
Inattivo (A piedi/Riposo): 0.00ms (Nessun impatto sulle prestazioni).
Durante lo svenimento/animazione: 0.01ms.
</details>
<details>
<summary>🇬🇧 English (Documentation)</summary>
🌟 Key Features
Automated Framework Detection: Automatically detects upon server boot whether it is running on ESX, QBCore, or Qbox to interface with standard food and thirst decline rates.
Progressive Fatigue System: Exertion is monitored in real-time. Sprinting and running increase exhaustion quickly, driving increases it slowly, while standing still reduces it.
Forced Blackouts (Emote Sleep): Upon reaching 90% fatigue, the screen fades to black and the player is forced to lay flat on the ground, automatically starting the native sleep scenario (WORLD_HUMAN_SUNBATHE_BACK) to regenerate energy on the spot.
Manual /dormi Command: Allows players to intentionally rest anywhere on foot, playing a lying-down animation and rapidly recovering their physical stamina.
iOS 17 Styled Notifications: Beautifully animated iOS-style alert banners with a smooth bounce transition, featuring a blurred Glassmorphism background and dynamic app icons that change based on the alert category (Emergency, Health, Sleep).
📥 Installation
Drag and drop the sleep_system folder into your server's resources directory.
Open your server.cfg file and add the resource:
code
Cfg
ensure sleep_system
Restart your server or start the resource by typing start sleep_system in the console.
⌨️ Commands & Keybindings
/dormi (Chat Command): Initiates or cancels the sleep state and forces the character to lay down.
Flashing Red Notification (iOS): Automatically triggers when fatigue exceeds 75% to warn the player to find rest.
📊 Performance (Resmon)
Idle (Walking/Resting): 0.00ms (Zero CPU impact).
During fainting/active loop: 0.01ms.
</details>
