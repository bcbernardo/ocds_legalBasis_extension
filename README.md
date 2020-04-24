# Legal basis

Adds fields to the tender object to describe the legal basis of the procedure.

The `tender.legalBasis` field is a `Classification` object. Example classification schemes are [LEX](https://en.wikipedia.org/wiki/Lex_(URN)), [CELEX](https://eur-lex.europa.eu/content/help/faq/intro.html#help8) and [ELI](https://en.wikipedia.org/wiki/European_Legislation_Identifier).

To indicate whether a procedure is covered by an international treaty like the Agreemement on Government Procurement (GPA), use the [coveredBy extension](https://extensions.open-contracting.org/en/extensions/coveredBy/) instead.

## Legal context

In the European Union, this extension's fields correspond to [eForms BT-01 (Procedure Legal Basis), BT-09 (Cross Border Law)](https://github.com/eForms/eForms) and [Article 39, paragraph 5 of Directive 2014/24/EU](https://eur-lex.europa.eu/legal-content/EN/TXT/?qid=1585836130257&uri=CELEX:32014L0024#d1e4669-65-1).See [OCDS for the European Union](http://standard.open-contracting.org/profiles/eu/master/en/) for the correspondences to Tenders Electronic Daily (TED).

## Example

```json
{
  "tender": {
    "crossBorderLaw": "Italian procurement legislation",
    "legalBasis": {
      "id": "32014L0025",
      "scheme": "CELEX"
    }
  }
}
```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.

## Changelog

### 2020-04-24

* Add `minProperties`, `minItems` and/or `minLength` properties.

This extension was originally discussed as part of the [OCDS for EU profile](https://github.com/open-contracting-extensions/european-union/issues) and in [pull requests](https://github.com/open-contracting-extensions/ocds_contractTerms_extension/pulls?q=is%3Apr+is%3Aclosed).
