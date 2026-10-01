# DEMITROMI Founder Preview 0.1.1 — Known Limitations

DEMITROMI 0.1.1 is prerelease software. Keep independent backups of important originals and review generated output before relying on it.

## Very large PDFs

A synthetic stress document containing approximately **3,150 pages** exposed a responsiveness limit during testing. Normal and practically large documents are covered by the current regression corpus, but extremely large documents may become slow or unresponsive.

## Fill & Sign PDF resource warning

A bounded synthetic/mixed-orientation fixture can retain an empty PDF text instruction referencing an unused font resource that PDFium removes during output generation. The visible original text and added Fill & Sign label remain present, but one external PDF diagnostic tool reports an unknown-font resource warning.

For important documents, review the resulting PDF before relying on it.

## Preview scope

- Windows **x64** is the supported Founder Preview architecture.
- ARM64 runtime acceptance is not part of this release.
- The package declares a Windows 10 1809 technical minimum, but physical runtime acceptance at that minimum has not been completed.
- Accounts, paid licensing, cloud document storage, and hosted AI services are not part of this preview.
