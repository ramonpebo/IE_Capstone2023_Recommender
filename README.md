# **MIND (MIcrosoft News Dataset) News Recommendation**
### Capstone Project - IE School of Science and technology - 2023

- Gustavo Welsh
- Dilhan Tanir
- Pierre-Louis Berlemont
- Felipe Basurto
- Ramón Peláez
-----------------

MIcrosoft News Dataset (MIND) is a large-scale dataset for news recommendation research. It was collected from anonymized behavior logs of Microsoft News website. The mission of MIND is to serve as a benchmark dataset for news recommendation and facilitate the research in news recommendation and recommender systems area.

MIND contains about 160k English news articles and more than 15 million impression logs generated by 1 million users. Every news article contains rich textual content including title, abstract, body, category and entities. Each impression log contains the click events, non-clicked events and historical news click behaviors of this user before this impression. To protect user privacy, each user was de-linked from the production system when securely hashed into an anonymized ID.

----------------

| Mind - demo 
| Model   | group_auc | mean_mrr | ndcg@5 | ndcg@10 |
|----------|----------|----------|--------|---------|
| Random    |   -  |   -  | 0.2211 |  0.2823 |
| Popularity    |   -  |   -  | 0.2766 |  0.333 |
| NPA    |   0.5968   |   0.2718   | 0.2926  |  0.3601 |
| NMRS    |   0.6169  |   0.2729  | 0.2948 |  0.3659 |
| NAML    |   0.6187  |   0.2848  | 0.3098 |  0.3736 |
| LSTUR    |   0.6443  |   0.2961  | 0.327 |  0.3897 |

----------------------------

| Mind - small |
| Model | ndcg@5 | ndcg@10 | Precision |
|----------|--------|---------|-----------|
| Random    | 0.2243 |  0.2870 | 0.069 |
| Popularity    | 0.2819 |  0.338 | 0.076 |
| NPA	| 0.3288 |	0.3926 |	0.1314 |
| NAML    | 0.3408 |  0.4038 | 0.1326 |
| NAML + NPA    | 0.3414 |  0.4042 | 0.1331 |
| LSTUR    | 0.3474 |  0.4090 | 0.1395 |
| LSTUR + NPA | 0.3486 |  0.4103 | 0.1404 |
| NRMS    | 0.3451 |  0.4099 | 0.1434 |
| NRMS + NPA    | 0.3456 |  0.4101 | 0.1430 |
| NAML + LSTUR    | 0.3496 |  0.4116 | 0.1425 |
| NAML + LSTUR + NPA    | 0.3495 |  0.4116 | 0.1425 |
| NRMS + NAML    | 0.3483 |  0.4122 | 0.1396 |
| NRMS + NAML + NPA    | 0.3482 |  0.4121 | 0.1398 |
| NRMS + LSTUR    | 0.3505 |  0.4140 | 0.1452 |
| NRMS + LSTUR + NPA    | 0.3505 |  0.4141 | 0.1454 |
| NRMS + NAML + LSTUR | 0.3512 | 0.4142 | 0.1445 |

-------------------------

| Mind - large
| Model   | group_auc | mean_mrr | ndcg@5 | ndcg@10 |
|----------|----------|----------|--------|---------|
| Random    |   -  |   -  | 0.2235 |  0.2864 |
| Popularity    |   -  |   -  | 0.2815 |  0.338 |
| LSTUR    |   0.6806  |   0.3295  | 0.3629 |  0.427 |
