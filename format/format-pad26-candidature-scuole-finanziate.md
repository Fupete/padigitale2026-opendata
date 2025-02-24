# PA digitale 2026 format "Candidature Finanziate"

## Aggiornamento dati
- Quotidiano, alle 2:00 (UTC). 

## Formato dati

**Reference file:** 
* candidature_scuole_finanziate.csv<br>
* candidature_scuole_finanziate.json<br>

Il dataset contiene la lista delle proposte di finanziamento, richieste da Scuole, che hanno superato i controlli di ricevibilità e ammissibilità e per le quali gli enti hanno provveduto alla comunicazione del codice CUP. 

Le candidature sono state separate in un file distinto per ogni cluster di pubbliche amministrazioni: Comuni, Scuole e altri enti.
I file sono tutti strutturati nella seguente maniera:

| Campo | Tipo di dati | Descrizione | Formato |
| --- | --- | --- | --- |
| codice_ipa | string | Codice identificativo estratto dall'Indice delle Pubbliche Amministrazioni | |
| ente | string | Nome descrittivo dell'ente | varchar(250) |
| tipologia_ente | string | Tipologia dell'ente tra le platee destinatarie degli avvisi  | Comune, Scuole, Altri Enti |
| comune | string | Comune associato alla PA, come riportato in IPA. | |
| cod_comune | string | Codice ISTAT del comune associata alla PA | |
| provincia | string | Provincia associata alla PA, come riportato in IPA. | |
| cod_provincia | string | Codice ISTAT della provincia associata alla PA | |
| regione | string | Regione associata alla PA, come riportato in IPA. | |
| cod_regione | string | Codice ISTAT della regione associata alla PA | |
| importo_finanziamento | float | Importo del voucher richiesto dalla PA nella candidatura | |
| avviso | string | Avviso a cui l'ente si è candidato | |
| data_invio_candidatura | datetime | Data in cui la PA ha trasmetto la sua candidatura al Dipartimento della Trasformazione Digitale.  | yyyy-MM-ddTHH:mm:ss.SSS Z|
| data_finanziamento | datetime | Data in cui è stato decretato l'assegnazione del voucher. | yyyy-MM-dd |
| codice_cup| string | Codice CUP, trasmesso dalla PA, associato al progetto della candidatura. | |
| numero_finestra_temporale | integer | Progessivo numerico indicativo della finestra temporale in cui la PA si è candidata al rispettivo avviso. | |
| decreto_finanziamento | string | Riferimento del decreto di finanziamento tramite cui sono state confermate le candidature assegnatarie di un finanziamento.| |
| numero_di_protocollo | integer | Progressivo numerico relativo al decreto di finanziamento in cui alla candidatura è stato assegnato il finanziamento.| |
| stato_candidatura | string | Stato aggiornato della candidatura. Al momento può assumere i seguenti valori: 'A', se la candidatura risulta assegnataria di un finanziamento; 'R', se è stata decretata la richiesta di rinuncia fatta dell'ente.  | |
| misura | string | Misura di riferimento a cui appartiene la candidatura | |

Questi dati sono disponibili anche in formato json.
