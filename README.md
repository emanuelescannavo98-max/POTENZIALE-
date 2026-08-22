# POTENZIALE 1.3

Sistema personale offline-first per task, continuità, progressi, check-in, obiettivi ed economia personale.

## Struttura
- Oggi: task del giorno, momentum, score e piano adattivo.
- Task: gestione delle attività e dei giorni successivi.
- Progressi: andamento settimanale e pilastri.
- Economia: movimenti, saldo e target mensili.
- Obiettivi: traguardi misurabili.
- Check-in: dati utilizzati dal motore adattivo.
- Aperte: cose da risolvere trasformabili in task.

## Dati
I dati restano nel browser tramite localStorage. Backup e ripristino permettono di esportare/importare lo stato.

## Migrazione
La prima apertura della 1.3 prova automaticamente a migrare `potenziale_v12` in `potenziale_v13`, mantenendo task, obiettivi, movimenti, check-in e metriche.
