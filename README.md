# Kiron CDG

Kiron CDG supporta il controllo di gestione raccogliendo dati gestionali e contabili da più sistemi e trasformandoli in una base unica, coerente e verificabile.

Il prodotto ha due finalità principali:

- produrre il **consuntivo mensile** di ricavi e costi, chiamato Actual;
- costruire il **Forecast**, cioè una previsione aggiornata dell'andamento economico.

Le informazioni vengono organizzate per periodo, prodotto, rete e istituto. Il risultato alimenta le dashboard direzionali e permette di confrontare dati gestionali e contabili, applicare regole di calcolo, distribuire valori aggregati e gestire eventuali differenze o conguagli.

## A cosa serve

Kiron CDG permette di:

- ridurre le elaborazioni manuali;
- usare regole di calcolo più chiare e tracciabili;
- avere una vista comune dei dati economici;
- riconciliare i dati gestionali con quelli contabili;
- aggiornare le previsioni partendo dai dati effettivi;
- rendere più semplice il controllo delle anomalie e delle rettifiche.

## Fonti e risultati

Il prodotto utilizza dati provenienti principalmente da:

- **Campus** e **Campus 2.0**, per le informazioni gestionali;
- **Zucchetti Infinity**, per le informazioni contabili.

Produce basi dati dedicate ad Actual e Forecast, utilizzate dalle dashboard direzionali Monitor Actual e Monitor Forecast.

## Documentazione

- [`docs/product-overview.md`](docs/product-overview.md): descrizione funzionale del prodotto per utenti e business owner;
- `docs/input/`: documentazione originale e file di supporto;
- `ai-workflows/`: strumenti utilizzati per analizzare e confrontare i requisiti;
- `ai-runs/`: risultati delle singole analisi.

La documentazione originale sotto `docs/input/` non deve essere modificata.

## Collegamento seriale al Developer Workspace

L’adozione documentale di [Homelab #1265](https://github.com/skunklabs-uk/homelab/issues/1265)
usa un consumer seriale e un checkout isolato, con repository e thread,
branch, head e prompt vincolati all’incarico.

Il child restituisce un report senza modificare file. Il coordinatore verifica
il risultato e ne registra l’accettazione con RETURN. La proposta revisionata
viene applicata separatamente su una normale PR discendente da main;
lo snapshot senza parent non viene integrato.

Questa nota non analizza il prodotto, i dati gestionali o contabili né la
documentazione cliente. Non modifica gli originali o i risultati delle analisi.
La preview HTTP non si applica all’incarico documentale e il report non attesta
un’applicazione o un servizio esposto.

Per il funzionamento del collegamento, consultare il [runbook Developer Workspace](https://github.com/skunklabs-uk/developer-workspace/blob/main/docs/WORKSPACE-HANDOFF.md)
e il [README del deployment Homelab](https://github.com/skunklabs-uk/homelab/blob/main/gitops/apps/developer-workspace/README.md).
