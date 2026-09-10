# CV source and review versions

- `original/Guido_Spano_CV_original.tex`: the user-supplied source, preserved byte for byte.
- `original/Guido_Spano_CV_original.pdf`: compiled from that source.
- `revised/Guido_Spano_CV_revised.tex`: revised source for approval.
- `revised/Guido_Spano_CV_revised.pdf`: compiled revised version.

Both versions compile with pdfLaTeX to two pages without warnings or overfull boxes.

## Comparison with the website PDF

Compared with `assets/Guido-Spano-CV.pdf` (Git blob `dae8d0027f225f1ff37818f243e725352cd3dd2d`), the original compiled source has the same text except that the header displays `guido-spano.github.io` instead of `guido-spano.com`. Line wrapping and page breaks match; matching-word bounding boxes differ by less than 0.07 points, reflecting the compiler/font environment.

## Revised version

- Adds the ECB Working Paper Series No. 3274, 2026 citation and hyperlinks the two working-paper titles. Uses the ECB publication's plural title, “Banks’ Funding Structures and Pass-Through in the Euro Area”.
- Adds the Stone Centre PhD Scholarship (2026–2027), with the linked centre name on a smaller second line.
- Links the three AY 2024/25 conferences to their event pages. No public event pages were found for the DGMF seminar or the eighth ChaMP Workstream 1 workshop; these remain unlinked.
- Updates AY 2025/26 with all five requested linked events.
- Updates the header domain and revision month.
- Retains plain black hyperlink text with no underlining or borders.

The revised PDF is also published at `assets/Guido-Spano-CV.pdf`, the file used by the website CV link. It includes the linked “PhD Scholar at the Stone Centre at UCL” entry under Service and Memberships. The original source and PDF are retained for reference.

## Compile from the repository root

```sh
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=cv/original cv/original/Guido_Spano_CV_original.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=cv/original cv/original/Guido_Spano_CV_original.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=cv/revised cv/revised/Guido_Spano_CV_revised.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=cv/revised cv/revised/Guido_Spano_CV_revised.tex
```
