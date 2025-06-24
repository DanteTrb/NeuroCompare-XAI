# NeuroCompare-XAI
Compare neurological patients using embedding, clustering and explainable AI

🔍 Powered by SHAPSet plots, radar clustering, and narrative explanations for clinical interpretability.

## Dato un nuovo soggetto con dati da sensori, l’agente AI identifica i soggetti più simili in un database clinico, visualizza somiglianze biomeccaniche e fornisce una spiegazione narrativa interpretabile del profilo.

🧩 Architettura logica del progetto
Fase 1 — Embedding clinico
Input: dataset pulito (EMG/IMU/clinical gait features)

Tecnica: riduzione dimensionale (UMAP/PCA)

Output: mappa dello spazio clinico in cui ogni punto è un soggetto

🔁 Vantaggio: visualizzazione intuitiva e clustering automatico

Fase 2 — Similarità e confronto soggetti
Dato un nuovo soggetto, trova i K più simili (es. 5) usando distanza euclidea o cosine

Output: lista soggetti simili + distanza + classe clinica prevalente

🔁 Use case clinico: “a chi assomiglia il mio paziente?”

Fase 3 — Explainability avanzata
Calcolo SHAP (anche SHAPSet plot)

Radar Plot delle feature più impattanti nella similarità

Generazione narrativa del risultato:

“Questo soggetto mostra una marcata riduzione della variabilità ML, simile al cluster dei soggetti con triade prodromica RBD + hyposmia + depressione.”

🔁 Outcome: spiegazione interpretabile e leggibile da un medico

Fase 4 — Webapp interattiva
Interfaccia Streamlit elegante

Input: parametri clinici del nuovo soggetto

Output: mappa dei simili, radar plot, spiegazione testuale

🔁 Demo pubblica: una UX da conference o pitch investor

Fase 5 — Deploy & GitHub polish
Push completo con struttura da pro, badge, GIF animata

README storytelling-oriented

Possibile paper/demo da presentare a congresso SIAMOC o Frontiers

📂 Moduli tecnici
Modulo Python	Funzione
preprocessing.py	Pulizia, scaling, normalizzazione
clustering.py	Embedding, UMAP, KMeans
similarity.py	Calcolo distanza, KNN
explainability.py	SHAP, SHAPSet plot, radar, narrativa
app/app.py	Frontend Streamlit

🚀 Timeline suggerita (30 giorni, stile Sprints)
Giorni	Obiettivo
1–3	EDA, embedding, radar UMAP
4–6	KNN + sistema di confronto
7–10	SHAP, radar plot, narrative
11–15	Streamlit: input → visualizzazione
16–20	Polishing: grafica, filtri, UX
21–25	Testing + documentazione
26–30	Deploy finale, GitHub repo ✨
