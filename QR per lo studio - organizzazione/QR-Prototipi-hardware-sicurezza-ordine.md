---
title: "QR – Prototipi hardware: sicurezza & ordine"
version: "1.2"
autore: "<Classe/Studente>"
licenza: "CC BY 4.0"
ultimo_aggiornamento: "2025-10-05"
---

## 1) Preparazione dell’area
- [ ] **Banco pulito** (via liquidi/oggetti inutili), **luce buona**, sedia stabile.
- [ ] **Documenti a vista**: schema, pinout, datasheet (cartella o busta trasparente).
- [ ] PC/Notebook con IDE aperto e cavo **funzionante**.
- [ ] Foto “prima” del banco (torna utile per confronto e relazione).

## 2) Alimentazione (scelte & verifiche)
- [ ] Cabla **a cavo staccato**; alimenta **solo a fine controllo**.
- [ ] Tensione/ corrente **coerenti** con il carico (es. 5 V/2 A).
- [ ] **Polaritá marcata**: rosso = +V, nero = GND; niente fili volanti non isolati.
- [ ] Se possibile, **limite di corrente** sull’alimentatore o fusibile rapido.
- [ ] Con più sorgenti, **GND comune** (salvo isolamenti voluti).

## 3) Cablaggio e componenti
- [ ] **Cavi corti e fissati** (fascette/nastro); evitare anelli e incroci inutili.
- [ ] Breadboard ok per segnali/ piccole correnti; per >300 mA usa morsetti/stripboard.
- [ ] Sezione fili adeguata (motori ≠ jumper sottili).
- [ ] **Polarità**: LED/elettr. corretta; **diodo di ricircolo** con relè/motori.
- [ ] **ESD**: tocca GND prima di maneggiare IC/sensori; se possibile usa bracciale.

## 4) Strumentazione & misure
- [ ] Multimetro: scala corretta (V, A, Ω) e **sonde ben inserite**.
- [ ] **Prima di accendere**: continuità tra +V e GND (no corto).
- [ ] **Dopo**: misura V su pin chiave, **corrente assorbita**, temperatura (dito/IR).
- [ ] Logga dati e condizioni (V aliment., carico, ambiente).

## 5) Procedura di test (incrementale)
1. **Alimenta** → verifica solo la parte di potenza.
2. **Aggiungi** un modulo alla volta (sensore → attuatore).
3. **Stato noto** a ogni passo; se peggiori, **rollback** alla versione stabile.
4. Una modifica per volta (HW *o* SW), poi test.

## 6) Chiusura lavori
- [ ] **Spegni e scollega**.
- [ ] **Post-it** di stato: “sensore X instabile; rifare cablaggio domani”.
- [ ] Riponi componenti/attrezzi; avvolgi cavi.
- [ ] **Backup**: foto cablaggio, schema aggiornato, commit codice con messaggio chiaro.

## 7) Rischi tipici & prevenzione
- **Surriscaldamento** → dissipatori/pad; rispetta correnti massime; ventilazione.
- **Corto** → rifinisci stagnature; isola punti nudi; sostituisci breadboard usurate.
- **Rumore elettrico** → twist cavi segnale, **bypass 0.1 µF** vicino a Vcc, massa a stella.
- **Batterie Li-ion/LiPo** → carica **solo** con circuiti dedicati; non perforare/piegare; mai in corto; storage ~3.8 V.