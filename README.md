# Guido Spanò — academic website

This is a responsive static academic website designed for GitHub Pages. Its visual structure is inspired by the restrained, text-led format of Morgane Richard's academic website, while using an original implementation and content tailored to Guido Spanò.

## Files to upload

Keep this structure in the root of the GitHub Pages repository:

```text
index.html
styles.css
favicon.svg
assets/
  profile.jpg
  Guido-Spano-CV.pdf
  profile-placeholder.svg
  papers/
    banks-funding-pass-through.pdf
    ample-reserves-deposit-pass-through.pdf
    no-country-young-managers.pdf
```

Filenames and capitalisation are case-sensitive on GitHub Pages.

## Add your photograph

1. Choose a portrait-oriented JPG photograph. A 4:5 crop works best; approximately 1200 × 1500 pixels is ample.
2. Rename it exactly `profile.jpg`.
3. Upload it inside the repository's `assets` folder.

The website already looks for `assets/profile.jpg`. Until that file is present, it shows `profile-placeholder.svg`.

## Add or replace your CV

1. Export the public version of your CV as a PDF.
2. Rename it exactly `Guido-Spano-CV.pdf`.
3. Upload it inside the repository's `assets` folder.

Both CV links in `index.html` already point to `assets/Guido-Spano-CV.pdf`. When the PDF is replaced with a newer file using the same name, the website links do not need to change.

## Add the research papers

Upload public PDFs inside `assets/papers` using the filenames listed above. If you use different filenames, update the corresponding `href` values in `index.html`.

Do not upload a confidential draft. If a paper is not public, delete or comment out its PDF link in `index.html` until it is ready.

## Publish through GitHub's website

1. Download and unzip the website package on your computer.
2. Open the GitHub repository that is configured for GitHub Pages.
3. Select **Add file → Upload files**.
4. Drag the extracted files and folders into the upload area. `index.html` must be at the repository root, not inside another folder.
5. Select **Commit changes**.
6. Open **Settings → Pages** and confirm the publishing source is the branch and root folder containing `index.html`.

If GitHub's upload screen does not preserve the folders, first upload the three root files. Then open or create `assets`, upload the photograph and CV, open or create `assets/papers`, and upload the paper PDFs.

Changes normally appear after GitHub Pages finishes its deployment. Hard-refresh the page if the old version is cached.

## Edit the text

On GitHub, open `index.html`, select the pencil icon, edit the relevant paragraph or paper entry, and commit the change. The colours, spacing and responsive behaviour are controlled by `styles.css`.

The current email address and the UCL and ECB profile links were taken from public institutional profile pages. Review the biography and paper descriptions before publishing, and remove any research item that you do not yet want to make public.
