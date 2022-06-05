# Comparison-of-Clustering-Algorithms-for-Speaker-Diarization

Весь пайплайн диаризации реализован в `clustering-algorithms-comparison.ipynb`. 

1. Importing: импортируются нужные библиоеки и функции.
2. Voice activity and overlapped speech detection: создаются словари uri2vad, uri2osd, uri2ann_ref с информацией о сегментах с речью, с несколькими говорящими и о референсной разметки для каждого аудиофайла (для каждого набора данных).
3. Embeddings extraction: создаются словари uri2data с векторными представлениями сегментов аудиофайлов.
4. Clustering: подбираются гипер параметры алгоритмов кластеризации (development set) и кластеризуются векторные представления сегментов (создаются словари uri2ann_hyp с предсказанной разметкой).
5. Perfomance metrics: подсчитываются значения метрик DER и JER.

Доступ к папке `diarization`: [гугл-диск](https://drive.google.com/drive/folders/1XwTrRk3Xiwn1LMaR9-HpL57ryzr19vs8?usp=sharing).
