# Publications Folder

Place PDF copies of your publications here (if allowed by publisher copyright policies).

## Copyright Considerations:

Before posting PDFs, check the publisher's policy:

1. **Open Access papers**: Usually fine to post
2. **Author's accepted manuscript**: Often allowed after embargo period
3. **Publisher's version**: Usually NOT allowed

Check policies at:
- [SHERPA/RoMEO](https://v2.sherpa.ac.uk/romeo/) - Database of publisher policies
- Your publisher's author agreement

## Alternatives to Posting PDFs:

- Link to the DOI (preferred): `[DOI](https://doi.org/10.XXXX/XXXXX)`
- Link to PubMed: `[PubMed](https://pubmed.ncbi.nlm.nih.gov/XXXXXXXX/)`
- Link to preprint (bioRxiv, arXiv, etc.)
- Use institutional repository

## Naming Convention:

If posting PDFs, use consistent naming:
- `AuthorYear_ShortTitle.pdf`
- `Smith2024_GeneExpression.pdf`
- `Jones2023_MethodsDevelopment.pdf`

## BibTeX Alternative:

For advanced users, you can use a .bib file with Quarto's citation system:

1. Create `references.bib` in root folder
2. Add to `_quarto.yml`:
   ```yaml
   bibliography: references.bib
   ```
3. Cite in text: `[@smith2024]`

See: https://quarto.org/docs/authoring/footnotes-and-citations.html
