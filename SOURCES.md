# Website data provenance

Version: 0.3  
Prepared: 2026-09-22

## Canonical website dataset

`vocabulary.js` is a compact, derived, non-participant dataset with four website views: the 138-word candidate pool, 34-word current study set, 433-word HKUST Life Science list, and 468-word HKUST × COCA Medicine overlap. JavaScript is used so the site works when opened directly from the filesystem.

## Project sources

1. `Methods/background Info/URIS_3_9 /Wordlists/ UST STEM Wordlist.xlsx`
   - HKUST discipline lists, including all 433 Life Science words.
2. `Methods/background Info/URIS_3_9 /backup_URIS/UST STEM Wordlist + COCA (repeat).xlsx`
   - Recorded HKUST × COCA overlap and all 468 words labelled Medicine.
3. `Methods/background Info/URIS_3_9 /Wordlists/COCA Academic Vocabulary List.xlsx`
   - Source-recorded POS codes. Coverage: 138/138 candidate words, 468/468 Medicine-overlap words, and 272/433 Life Science words.
4. `Methods/background Info/URIS_3_9 /Wordlists/Survey Wordlists - 3.20.xlsx`
   - Formal 138-word candidate pool and recorded prefix/suffix coding.
5. `Methods/background Info/URIS_3_9 /Second Pilot/Gorilla Spreadsheet/22-4/Learn_Short_Morph_schedule.xlsx`
   - Implemented Chinese meanings for the 34 current study words. Simplified characters were converted to standard Traditional Chinese without changing meaning.
6. `Mixed Effects Model/19_9/Word_Level_Variable.xlsx`
   - Current-study item ID, POS, iWeb frequency, and lexical analysis.
7. `analysis_pipeline/correlation_preliminary_2026_09_16/outputs/word_level_inputs.csv`
   - Verified mean usefulness and difficulty ratings for the 34 current study words.

## Official public terminology sources

Exact English headwords were matched against four Hong Kong Education Bureau glossaries: Biology (2020), Science (2017), Chemistry (2007), and Physics (2020). The source page is `https://www.edb.gov.hk/en/curriculum-development/kla/science-edu/ref-and-resources/glossary.html`.

## Transformations

- COCA POS codes were expanded into readable labels. Multiple recorded values are retained.
- The 433- and 468-word lists contain 86 shared words; neither was treated as a subset of the other.
- Only complete English-headword matches from the official glossaries were accepted. Biology was prioritized, followed by general Science, Chemistry, and Physics.
- Missing POS is shown as `Pending verification`; missing Chinese terminology is shown as `待核實`. Neither is inferred from spelling or machine translation.
- Candidate-pool affixes reproduce the source workbook without silent normalization.
- The Affix Explorer uses the 34-word set as its core and shows no more than four separately labelled 138-pool examples for a matching recorded affix.
- No participant data, responses, identifiers, outcomes, or preliminary inferential findings are included.

## Current coverage and limitations

- HKUST Life Science: POS verified for 272/433; Traditional Chinese verified for 162/433.
- HKUST × COCA Medicine: POS verified for 468/468; Traditional Chinese verified for 236/468.
- Candidate pool: POS verified for 138/138; Chinese coverage follows the same official/project terminology rules.
- POS describes the source lexical entry, not a new researcher-coded STEM-sense annotation.
- `待核實` is a status marker, not a translation.
