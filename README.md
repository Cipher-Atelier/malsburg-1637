# Malsburg’s cipher letter (1637)

A separate ten-line alphabetic cipher block at the foot of a January 1637 letter attributed to Malsburg. This investigation covers that block, not the whole surrounding numerical correspondence.

[Cipher Atelier](https://github.com/Cipher-Atelier) · [Research index](https://github.com/Cipher-Atelier/research-index) · [Reading guide](READING_GUIDE.md) · [Verification](verification/README.md)

## Current status — 11 October 2026

This is a reproducible reading proposal for the 510-letter alphabetic block, awaiting external historical and palaeographic verification. The proposed German text discusses command, Swedish generals and possible departure; the opening remains conditional. It does not decipher the surrounding numerical correspondence. The modern label `EFDGC` represents shifts `4,5,3,6,2` over the specified 24-letter alphabet; it is not an established historical keyword. Daniel Bourdeau’s foundational work and Larry Beck’s later contribution with ChatGPT remain credited.

| Evidence layer | Open this |
| --- | --- |
| Original | [HCP497 catalogue](https://crypto.hcportal.eu/dashboard/cryptograms/497) · [source image](https://api.hcportal.eu/media/1395/79511677516420.jpg) |
| Recorded letters / key rule | [Normalized ciphertext](verification/readings/evidence/Malsburg_1637_evidence_and_code/Malsburg_1637/cryptanalysis/normalized_ciphertext.txt) · [alphabet and shifts](malsburg-1637/article.md#one-alphabet-one-key-one-continuous-stream) |
| Literal / diplomatic German | [Letter-only literal](verification/readings/evidence/Malsburg_1637_evidence_and_code/Malsburg_1637/cryptanalysis/literal_plaintext.txt) · [diplomatic text](verification/readings/evidence/Malsburg_1637_evidence_and_code/Malsburg_1637/cryptanalysis/diplomatic_decipherment.txt) |
| English interpretation | [What the block says](malsburg-1637/article.md#what-the-block-says) |

With zero-based `abcdefghiklmnopqrstuwxyz`, `h(7) − 4 = d(3)`, `k(9) − 5 = e(4)` and normalized `ü → u(19) − 3 = r(16)` give `der`. After `[43]`, `z` uses the fourth shift 6 and gives `s`; the marker consumes no key position. [Check the alignment](READING_GUIDE.md#check-one-example-by-hand).

**Unresolved / scope limits:** `[43]`, `[45]`, `[LL]` and the cancelled patch have unknown meanings; preserve `seist`, `tqouppen` and `itzigdn`. The English interpretation keeps the opening conditional and allows a proposed letter; it does not establish that the described events occurred. The [9 October numerical-code update](research-updates/2026-10-09-numerical-codes.md) concerns a different corpus and a bounded rejected direct-transfer hypothesis. The 510-letter checker reproduces neither that investigation nor the original statistical search.

### Research update — 9 October 2026

Read the [new check and its limits](research-updates/2026-10-09-numerical-codes.md). This update is documentation; new experiment scripts are not included.

## Start here

1. [Read the plain-language guide](READING_GUIDE.md): the document, result, file meanings and one worked check. No programming is required.
2. Open [German reading with manuscript markers](verification/readings/evidence/Malsburg_1637_evidence_and_code/Malsburg_1637/cryptanalysis/diplomatic_decipherment.txt) to inspect the saved text or test result itself.
3. Read the [research account](malsburg-1637/article.md) for historical context, methods, earlier work and unresolved questions.

## Reproduce the checks

Follow the worked example in [the reading guide](READING_GUIDE.md#check-one-example-by-hand). It connects a source record, a key or model assumption, and the saved output. For an independent source check, use the [original-source entry](https://crypto.hcportal.eu/dashboard/cryptograms/497); images are linked, not redistributed here.

If you use Python, follow the [complete verification instructions](verification/README.md), including download/setup, expected results and troubleshooting. The command from this repository’s top-level folder is:

```sh
python3 verification/check_all.py
```

A successful run means the published files and declared calculation reproduce. It does not establish that every source sign or historical interpretation is correct.

The standard-library baseline runs offline without extra packages. The [Evidence checks workflow](.github/workflows/verify.yml) runs it on Python 3.10 and 3.13 and checks the committed diff for whitespace errors.

## Research scope and limitations

510-letter alphabetic-block reading proposal. Unresolved markers, literal defects and missing historical alphabet.json remain explicit. Daniel Bourdeau’s foundational work and Larry Beck’s later contribution with ChatGPT are credited in the research account.

## Contribute

Read the current result and source limitations, then coordinate a bounded task in an existing issue or use [Work on existing research](https://github.com/Cipher-Atelier/malsburg-cipher-letter-1637/issues/new?template=research.yml). Fork the repository and submit a focused pull request with your evidence and checks. Independent replication and constructive alternative readings are welcome. See [Start here](https://github.com/Cipher-Atelier/research-index/blob/main/START_HERE.md) for the shared workflow.

This is part of [Cipher Atelier](https://github.com/Cipher-Atelier), founded by [Maxim Egorov](https://github.com/cayde-6). Explore the [research index](https://github.com/Cipher-Atelier/research-index), [contribution guide](https://github.com/Cipher-Atelier/.github/blob/main/CONTRIBUTING.md), and [step-by-step research workflow](https://github.com/Cipher-Atelier/research-index/blob/main/START_HERE.md).

## Sources and rights

Source credit and item-specific restrictions remain in the research records. Scans, crops, restricted materials and private correspondence are excluded. No new blanket licence is asserted. AI-assisted work requires evidence checking and does not constitute external human expert review.

[Publication provenance](SOURCE_PROVENANCE.json) records the source commit, retained file hashes and deliberate code/navigation adaptations. The original repository history remains intact.
