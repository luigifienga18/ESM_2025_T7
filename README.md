# ESM_2025_T7
Proggetto realizzato da Fienga Luigi [M63001733] e Andrea Roscigno [M63001778]

# Synthesis of Multiple Human Subjects

![](https://github.com/luigifienga18/ESM_2025_T7/blob/e0ed53cd9856b5f083f3157f4f9710fb4222d126/logo/logobw180.png)

Il seguente lavoro si presenta come un'esperienza ed un esperimento nell'uso di diverse tecniche per sintetizzare volti di due persone specifiche in una foto.
Nel repository sono presenti i folder:
- `dataset`: contentente le immagini usate per il lavoro; all'apertura del folder sono presenti diverse cartelle contenenti ognuna le immagini dei specifici soggetti; la cartella `person` contiene invece le immagini generate da stable diffusion per la classe persona, usando il prompt `a photo of a person` per quelle di sd1.5, e `a photo of a person, simple background, full body view, award winning photography, highly detailed` per sdxl. La cartella `Raccolte` contiene diverse combinazioni delle foto usate per diversi esperimenti, oltre alla cartella DatasetMudi che in più, presenta anche le maschere associate e il file jsonl.
- `dreambooth`: contiene il file per poter eseguire un addestramento di un modello mediante l'ononima tecnica, con i soggetti che vogliamo , oppure fare inferenza su un modello già addestrato. La realizzazione del seguente codice è stata possibile grazie alla fork di [Shivam Shirao](https://github.com/ShivamShrirao/diffusers/tree/main/examples/dreambooth) che ci ha permesso di implementare i Multi-Concepts mediante dreambooth.
- `mudi`: contenente tre file .ipynb, uno per creare le maschere dei soggetti e generare le immagini della classe dei soggetti con annesse maschere; uno per effettuare l'allenamento del modello; infine un ultimo per fare inferenza. Il seguente codice è stato possibile realizzarlo grazie all'implemeantazione ufficiale di [MuDI](https://github.com/agwmon/MuDI)
- `metriche`: contenente i tre notebook per testare le immagini generate, in particolare sono state usate: CLIP-I, CLIP-S e D&C (introdotta con MuDI).