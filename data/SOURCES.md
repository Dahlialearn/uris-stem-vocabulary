# Website data provenance

Version: 0.5
Updated: 2026-09-23

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
   - Current-study item ID, POS, iWeb frequency, morphological category, and lexical analysis.
7. `analysis_pipeline/correlation_preliminary_2026_09_16/outputs/word_level_inputs.csv`
   - Verified mean usefulness and difficulty ratings for the 34 current study words.
8. `Methods/background Info/URIS_3_9 /Second Pilot/Gorilla Spreadsheet/22-4/Learn_Short_Morph_schedule.xlsx`
   - Implemented morphology breakdowns used to distinguish recorded prefixes and suffixes in the 34-word study set.
9. `PolyU-CALLS 2025 .pdf`
   - Approved conference presentation. The unchanged PDF is displayed through the browser's built-in viewer from `assets/outputs/polyu-calls-2025.pdf`; SHA-256: `1b0ffd8ff5317a9d39b462c576233178d641ef236af258519aa746667177d5d6`.
10. `Photo/IMG_0199.JPG`
   - Researcher-supplied project event photograph. A resized website derivative is stored at `assets/news/november-2025-curi-visit.jpg`; the original photograph is unchanged.
11. `Methods/background Info/URIS_3_9 /_Pilot_Data Analysis/Pilot - Second Round Analysis /Descriptive_Table.xlsx`
   - Word-level expert-rating coverage for the candidate pool. Ratings are available for 137 of the 138 candidate words.

## Official public terminology sources

Exact English headwords were matched against four Hong Kong Education Bureau glossaries: Biology (2020), Science (2017), Chemistry (2007), and Physics (2020). The source page is `https://www.edb.gov.hk/en/curriculum-development/kla/science-edu/ref-and-resources/glossary.html`.

## Transformations

- COCA POS codes were expanded into readable labels. Multiple recorded values are retained.
- The 433- and 468-word lists contain 86 shared words; neither was treated as a subset of the other.
- Only complete English-headword matches from the official glossaries were accepted. Biology was prioritized, followed by general Science, Chemistry, and Physics.
- Traditional Chinese terminology was reviewed and synchronised across the four vocabulary sets. POS values were added for 133 high-confidence entries; 28 context-sensitive entries remain explicitly marked `Pending verification` pending specialist confirmation.
- Candidate-pool affixes reproduce the source workbook without silent normalization.
- For the 34-word study set, morphological category is drawn from the current word-level workbook. Simple words display `NA` for prefix and suffix. Derived and compound words display a prefix or suffix only where the project materials support that label.
- The Affix Explorer uses this 34-word coding as its core and shows no more than four separately labelled 138-pool examples for a matching recorded affix.
- No participant data, responses, identifiers, outcomes, or preliminary inferential findings are included.

## Current coverage and limitations

- HKUST Life Science: POS verified for 272/433; Traditional Chinese verified for 162/433.
- HKUST × COCA Medicine: POS verified for 468/468; Traditional Chinese verified for 236/468.
- Candidate pool: POS verified for 138/138; Chinese coverage follows the same official/project terminology rules.
- POS describes the source lexical entry, not a new researcher-coded STEM-sense annotation.
- `待核實` is a status marker, not a translation.
- Morphological categories and split prefix/suffix fields for the broader 138-word pool are deferred until a researcher-reviewed classification workbook is supplied.
- Remaining Traditional Chinese verification is deferred until the researcher supplies the completed terminology list.
