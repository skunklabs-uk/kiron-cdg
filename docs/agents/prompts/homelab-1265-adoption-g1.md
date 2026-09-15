# Homelab #1265 — proposta tecnica README root per `kiron-cdg`

**Stato: Active**

## Autorità e incarico

Missione: [Homelab #1265](https://github.com/skunklabs-uk/homelab/issues/1265), adozione del collegamento seriale per i repository in scope.

Questo incarico è **parentless report-only**: prepara una proposta tecnica per una sezione del README root di `skunklabs-uk/kiron-cdg`. Il parent applicherà la proposta revisionata in una normale PR discendente da main. Il branch snapshot senza parent non viene mai integrato. Non introduce decisioni di prodotto e non modifica il comportamento del sistema descritto dal repository.

Leggi integralmente la RFC-0001 corrente fornita dal parent e le istruzioni applicabili già qualificate. Usa lo snapshot verificato, senza ricostruire head o contesto tramite rete.

## Provenienza e snapshot dell'incarico

- Repository: `skunklabs-uk/kiron-cdg`.
- Provenienza osservata in sola lettura: `main@c12ba485399417d7f185f0001216b184653d3a52`.
- Snapshot da usare per l'incarico: branch e head esatti forniti dal parent nella richiesta verificata. Non assumere che coincidano con `main` e non ricostruirli tramite rete.
- Root `AGENTS.md`: blob `a94899de7e7b3b96d384b1a440873d3ab6853b2e`, mode `100644`.
- Root `README.md`: blob `26477a101fb4af55705a48869a00c11d017eab53`, mode `100644`.

Il README root è la destinazione già esistente. La proposta deve riguardare soltanto il collegamento tecnico seriale: incarico, checkout isolato, report, pubblicazione affidata al parent, RETURN e limiti operativi.

## Fonti del collegamento già verificate

Usa soltanto il contesto fornito dal parent per i runbook proprietari:

- Developer Workspace [`WORKSPACE-HANDOFF.md`](https://github.com/skunklabs-uk/developer-workspace/blob/95ef023/docs/WORKSPACE-HANDOFF.md), revisione `95ef023`.
- Homelab [`README runtime Developer Workspace`](https://github.com/skunklabs-uk/homelab/blob/a4173754/gitops/apps/developer-workspace/README.md), revisione `a4173754`.

Queste fonti coprono enrollment, selezione GitOps, recupero e stato persistente. Il child senza rete deve usare questo contesto e non ricostruire le fonti.

## Perimetro della proposta

La proposta deve:

1. restare in italiano e riferirsi al README root;
2. distinguere incarico autorizzato, report, pubblicazione parent e RETURN;
3. indicare repository/thread, branch/head e prompt come vincoli dell’incarico quando pertinenti;
4. chiarire che il consumer è seriale e usa un checkout isolato;
5. mantenere fuori scope prodotto, dati gestionali/contabili, documentazione cliente, input, `ai-runs` e qualsiasi corpus;
6. classificare la preview HTTP come `N/A` perché l'attività riguarda una nota documentale di adozione; il solo snapshot non attesta un'applicazione o un servizio esposto;
7. rimandare ai runbook proprietari senza duplicare configurazioni operative, dati cliente o credenziali;
8. non modificare né reinterpretare `docs/product-overview.md` o `docs/architecture-overview.md`.

Non introdurre nuovi gate, stati, workflow, tool, controlli o obblighi. Il README root è la sola destinazione documentale qualificata per questa proposta; non sono necessarie altre fonti `Active` per il report tecnico minimo.

## Divieti

- Non modificare `README.md` o altri file.
- Non leggere `docs/input/`, `ai-runs/`, documentazione cliente, business analysis o altri corpus.
- Non creare branch, ref, PR, enrollment o richiesta al consumer.
- Non eseguire consumer, modello, rollout, API esterne, installazioni o tool applicativi.
- Non leggere credenziali e non inventare dati, risultati, URL o prove runtime.

Le letture locali necessarie per verificare il perimetro e il confronto testuale sono consentite. Applica una revisione tecnica e `humanize-writing` alla proposta, se disponibile, senza installare skill o fingere una review indipendente. Il report deve separare fatti osservati, proposta editoriale, limiti e gate spettanti al parent.

## Consegna

Restituisci in italiano un report breve e autosufficiente con:

- head e blob esaminati;
- fonti effettivamente usate;
- proposta di sezione README root, senza applicarla;
- motivazione `N/A` della preview HTTP basata sullo scope documentale;
- limiti: nessuna evidenza di prodotto implementato, dati cliente, deploy o runtime;
- gate parent: applicazione della proposta tramite PR ordinaria, review, readback SHA/diff, RETURN e closeout RFC-0001; il prompt temporaneo va rimosso quando le informazioni durevoli sono trasferite nella fonte corrente.

L'esito del processo non equivale ad accettazione, pubblicazione o merge.
