## [Корпус гимнов стран мира на русском языке](Project1/anthems.json)

Источник: http://discoveric.ru/anthem/

Формат корпуса: JSON

Число текстов в корпусе: 93

### Разметка в корпусе

| Ключ          | Значение           | 
| ------------- |------------------| 
| `name`    | Название страны    |
| `link`    | Ссылка на текст гимна в источнике |   
| `text`  |  Текст гимна         |    
| `name_en`    | Название страны на английском языке    |
| `state_characteristics`     | Форма государства - государственное устройство, форма правления (список) |   
| `area`  | Площадь страны в квадратных километрах         |    
| `population`    | Население страны    |
| `former_colony`     | Была ли страна зависимой в прошлом (была колонией, входила в состав другого государства и т. п.) |   
| `religion`  | Религиозный состав населения страны (словарь с элементами `религия`:`доля населения, ее исповедающая`)|    
| `continent`     | Континент, на котором находится страна    |
| `secular`     | Является ли страна светской |   
| `text_lemmatized`  | Лемматизированный текст гимна (лемматизатор - Mystem)        |    
| `topic_to_similarity` | Близость текста каждой из следующих тем: общепатриотическая, война, бог, описание |
| `ud_graphs`     | Предложения текста гимна в формате словарей (исходно - nltk dependency graph; синтаксический парсер - UDPipe)   |

### Фрагмент корпуса
```
    "90": {
        "name": "ЮАР",
        "link": "http://discoveric.ru/anthem/yuar",
        "text": "Господи,\nблагослови Африку\nГосподи, благослови Африку,\nНаставь ее на путь истинный,\nУслышь наши мольбы.\nГосподи, благослови -\nГосподи, благослови,\n\nГосподи, благослови Африку,\nНаставь ее на путь истинный,\nУслышь наши мольбы.\nГосподи, благослови нас, детей Твоих,\nСвятой Дух, Святой Дух, снизойди к нам.\nГосподи, благослови нас, детей Твоих.\n\nСын Божий, храни наш народ,\nДа покончи с войнами и страданиями.\nТы храни его — ты храни его,\nНарод наш, народ Африки.\nТы храни его. Сын Божий — Ты храни его,\nТы храни его, народ,- Ты храни его,\nНарод наш, народ Африки.",
        "name_en": "South Africa",
        "state_characteristics": [
            "unitary state",
            "dominant-party system",
            "parliamentary system",
            "republic"
        ],
        "area": 1221037,
        "population": 58775022,
        "former_colony": 1,
        "religion": {
            "christianity": 95,
            "no": 15
        },
        "continent": "AF",
        "secular": 1,
        "text_lemmatized": "господи,\nблагословлять африка\nгосподи, благословлять африка,\nнаставлять она на путь истинный,\nуслышать наш мольба.\nгосподи, благословлять -\nгосподи, благословлять,\n\nгосподи, благословлять африка,\nнаставлять она на путь истинный,\nуслышать наш мольба.\nгосподи, благословлять мы, ребенок твой,\nсвятой дух, святой дух, снисходить к мы.\nгосподи, благословлять мы, ребенок твой.\n\nсын божий, хранить наш народ,\nда покончить с война и страдание.\nты хранить он — ты хранить он,\nнарод наш, народ африка.\nты хранить он. сын божий — ты хранить он,\nты хранить он, народ,- ты хранить он,\nнарод наш, народ африка.\n",
        "topic_to_similarity": {
            "общепатриотическая": 0.029578765834599403,
            "война": 0.0072533308896319615,
            "бог": 0.22951459195252744,
            "описание": 0.0
        },
        "ud_graphs": [
            [
                {
                    "address": 0,
                    "word": null,
                    "lemma": null,
                    "ctag": "TOP",
                    "tag": "TOP",
                    "feats": null,
                    "head": null,
                    "deps": {
                        "ROOT": [
                            1
                        ]
                    },
                    "rel": null
                },
                {
                    "address": 1,
                    "word": "Господи",
                    "lemma": "господи",
                    "ctag": "PROPN",
                    "tag": "NNP",
                    "feats": "Animacy=Anim|Case=Nom|Gender=Masc|Number=Sing",
                    "head": 0,
                    "deps": {
                        "conj": [
                            3
                        ],
                        "obj": [
                            7
                        ],
                        "punct": [
                            19
                        ]
                    },
                    "rel": "ROOT"
                },
                {
                    "address": 2,
                    "word": ",",
                    "lemma": ",",
                    "ctag": "PUNCT",
                    "tag": ",",
                    "feats": "_",
                    "head": 3,
                    "deps": {},
                    "rel": "punct"
                },
                {
                    "address": 3,
                    "word": "благослови",
                    "lemma": "благословлять",
                    "ctag": "NOUN",
                    "tag": "NN",
                    "feats": "Animacy=Inan|Case=Dat|Gender=Fem|Number=Sing",
                    "head": 1,
                    "deps": {
                        "punct": [
                            2,
                            6
                        ],
                        "appos": [
                            4
                        ]
                    },
                    "rel": "conj"
                },
                {
                    "address": 4,
                    "word": "Африку",
                    "lemma": "африка",
                    "ctag": "PROPN",
                    "tag": "NNP",
                    "feats": "Animacy=Anim|Case=Dat|Gender=Masc|Number=Sing",
                    "head": 3,
                    "deps": {
                        "flat": [
                            5
                        ]
                    },
                    "rel": "appos"
                },
                {
                    "address": 5,
                    "word": "Господи",
                    "lemma": "господи",
                    "ctag": "PROPN",
                    "tag": "NNP",
                    "feats": "Animacy=Anim|Case=Nom|Gender=Fem|Number=Sing",
                    "head": 4,
                    "deps": {},
                    "rel": "flat"
                },
                {
                    "address": 6,
                    "word": ",",
                    "lemma": ",",
                    "ctag": "PUNCT",
                    "tag": ",",
                    "feats": "_",
                    "head": 3,
                    "deps": {},
                    "rel": "punct"
                },
                {
                    "address": 7,
                    "word": "благослови",
                    "lemma": "благословлять",
                    "ctag": "NOUN",
                    "tag": "NN",
                    "feats": "Animacy=Inan|Case=Acc|Gender=Fem|Number=Sing",
                    "head": 1,
                    "deps": {
                        "appos": [
                            8
                        ],
                        "acl": [
                            10
                        ]
                    },
                    "rel": "obj"
                },
                {
                    "address": 8,
                    "word": "Африку",
                    "lemma": "африка",
                    "ctag": "PROPN",
                    "tag": "NNP",
                    "feats": "Animacy=Inan|Case=Acc|Gender=Fem|Number=Sing",
                    "head": 7,
                    "deps": {},
                    "rel": "appos"
                },
                {
                    "address": 9,
                    "word": ",",
                    "lemma": ",",
                    "ctag": "PUNCT",
                    "tag": ",",
                    "feats": "_",
                    "head": 10,
                    "deps": {},
                    "rel": "punct"
                },
                {
                    "address": 10,
                    "word": "Наставь",
                    "lemma": "наставлять",
                    "ctag": "VERB",
                    "tag": "VBC",
                    "feats": "Aspect=Perf|Mood=Imp|Number=Sing|Person=2|VerbForm=Fin",
                    "head": 7,
                    "deps": {
                        "punct": [
                            9
                        ],
                        "obj": [
                            11
                        ],
                        "obl": [
                            13,
                            14
                        ]
                    },
                    "rel": "acl"
                },
                {
                    "address": 11,
                    "word": "ее",
                    "lemma": "она",
                    "ctag": "PRON",
                    "tag": "PRP",
                    "feats": "Case=Acc|Gender=Fem|Number=Sing|Person=3",
                    "head": 10,
                    "deps": {},
                    "rel": "obj"
                },
                {
                    "address": 12,
                    "word": "на",
                    "lemma": "на",
                    "ctag": "ADP",
                    "tag": "IN",
                    "feats": "_",
                    "head": 13,
                    "deps": {},
                    "rel": "case"
                },
                {
                    "address": 13,
                    "word": "путь",
                    "lemma": "путь",
                    "ctag": "NOUN",
                    "tag": "NN",
                    "feats": "Animacy=Inan|Case=Acc|Gender=Masc|Number=Sing",
                    "head": 10,
                    "deps": {
                        "case": [
                            12
                        ]
                    },
                    "rel": "obl"
                },
                {
                    "address": 14,
                    "word": "истинный",
                    "lemma": "истинный",
                    "ctag": "ADJ",
                    "tag": "JJL",
                    "feats": "Animacy=Inan|Case=Acc|Gender=Masc|Number=Sing",
                    "head": 10,
                    "deps": {
                        "acl": [
                            16
                        ]
                    },
                    "rel": "obl"
                },
                {
                    "address": 15,
                    "word": ",",
                    "lemma": ",",
                    "ctag": "PUNCT",
                    "tag": ",",
                    "feats": "_",
                    "head": 16,
                    "deps": {},
                    "rel": "punct"
                },
                {
                    "address": 16,
                    "word": "Услышь",
                    "lemma": "услышать",
                    "ctag": "VERB",
                    "tag": "VB",
                    "feats": "Aspect=Imp|VerbForm=Inf",
                    "head": 14,
                    "deps": {
                        "punct": [
                            15
                        ],
                        "obj": [
                            18
                        ]
                    },
                    "rel": "acl"
                },
                {
                    "address": 17,
                    "word": "наши",
                    "lemma": "наш",
                    "ctag": "DET",
                    "tag": "PRP$",
                    "feats": "Animacy=Inan|Case=Acc|Number=Plur|Person=1",
                    "head": 18,
                    "deps": {},
                    "rel": "det"
                },
                {
                    "address": 18,
                    "word": "мольбы",
                    "lemma": "мольба",
                    "ctag": "NOUN",
                    "tag": "NN",
                    "feats": "Animacy=Inan|Case=Acc|Gender=Masc|Number=Plur",
                    "head": 16,
                    "deps": {
                        "det": [
                            17
                        ]
                    },
                    "rel": "obj"
                },
                {
                    "address": 19,
                    "word": ".",
                    "lemma": ".",
                    "ctag": "PUNCT",
                    "tag": ".",
                    "feats": "_",
                    "head": 1,
                    "deps": {},
                    "rel": "punct"
                }
            ],

             ** ОСТАЛЬНЫЕ ПРЕДЛОЖЕНИЯ ТЕКСТА В ФОРМАТЕ dependency graph **

        ]
    }

```
