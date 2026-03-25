# Italian WordNet Definitions

A structured, open-licensed JSON dataset mapping Italian lemmas to their WordNet synsets, enriched with Italian and English definitions.

## Contents

- `italian_synsets.json` — full dataset
- `italian_synsets_compact.json` — compact version with essential fields only

Each entry maps an Italian lemma to one or more synsets:

```json
"cane": [
  {
    "synset_id": "i46360",
    "pos": "n",
    "pwn_id": "omw-en31-02086723-n",
    "wordnet31_id": "02086723-n",
    "definition_en": "a member of the genus Canis (probably descended from the common wolf) that has been domesticated by man since prehistoric times; occurs in many breeds",
    "definition_en_source": "oewn",
    "definition_it": "animale domestico molto comune, diffuso in tutto il mondo, usato per la caccia, la difesa, nella pastorizia, e come animale da compagnia.",
    "definition_it_source": "iwn-omw",
    "slug": "cane"
  }
]
```

The compact version includes only the essential fields:

```json
"cane": [
  {
    "synset_id": "i46360",
    "pos": "n",
    "definition_it": "animale domestico molto comune, diffuso in tutto il mondo, usato per la caccia, la difesa, nella pastorizia, e come animale da compagnia.",
    "slug": "cane"
  }
]
```

## Coverage

~18,000 Italian lemmas · ~22,000 synset entries · nouns, verbs, adjectives, adverbs

Synset identifiers use the **ILI** (Interlingual Index) as the primary key, ensuring language-neutral concept linkage stable across WordNet versions.

## Data Sources & Required Attributions

| Source | Role | License |
|--------|------|---------|
| [IWN-OMW](https://github.com/valeq/IWN-OMW) — CNR-ILC | Italian definitions (primary) | **CC BY-SA 4.0** |
| [MultiWordNet](https://multiwordnet.fbk.eu) — FBK | Italian lemmas | CC BY 3.0 |
| [Wikidata](https://www.wikidata.org) (P8814) | Italian definitions (secondary) | CC0 |
| [Open English WordNet 2025](https://github.com/globalwordnet/english-wordnet) | English definitions (primary) | CC BY 4.0 |
| [Princeton WordNet 3.1](https://wordnet.princeton.edu) (via OMW) | English definitions, synset IDs | WordNet License |
| [CILI](https://github.com/globalwordnet/cili) | English definitions (fallback), ILI concept backbone | CC BY 4.0 |

## License

**CC BY-SA 4.0** — inherited from IWN-OMW. Any derivative work must be shared under the same license.

> WordNet® is a registered trademark of Princeton University.  
> WordNet 3.0 Copyright 2006 by Princeton University. All rights reserved.

## Citations

**IWN-OMW:**
> Quochi, V., Bartolini, R., and Monachini, M. "ItalwordNet goes open". *LiLT Special Issues on Open Multilingual WordNets*. CSLI Publications.

> Roventini, A. et al. (2003). "ItalwordNet: building a large semantic database for the automatic treatment of Italian". *Proceedings of the Second International Conference on Language Resources and Evaluation*.

**MultiWordNet:**
> Pianta, E., Bentivogli, L., and Girardi, C. (2002). "MultiWordNet: Developing an Aligned Multilingual Database". *Proceedings of the First International Conference on Global WordNet*, Mysore, India. pp. 293–302.

**Princeton WordNet:**
> Miller, G.A. (1995). "WordNet: A Lexical Database for English". *Communications of the ACM* 38(11): 39–41.

**Open English WordNet:**
> McCrae, J.P. et al. (2019). "English WordNet 2019 – An Open-Source WordNet for English". *Proceedings of the 10th Global WordNet Conference (GWC 2019)*.

**OMW / CILI:**
> Bond, F. and Foster, R. (2013). "Linking and extending an open multilingual wordnet". *ACL-2013*. pp. 1352–1362.
