# HEIC Bulk Converter

A browser-based tool for bulk converting HEIC and HEIF image files to JPEG or PNG. Built for internal use at The Flagstaff Group.

Everything runs entirely in the browser. No files are uploaded to any server and no data leaves the device.

---

## Features

- Drag and drop or browse to select multiple HEIC or HEIF files at once
- Convert to JPEG or PNG output
- Adjustable JPEG quality (10 to 100 percent)
- Progress bar tracking conversion across the batch
- Download files individually or as a single ZIP archive
- Fully client-side, no backend required

---

## How to Use

1. Open the tool in your browser
2. Drag and drop your HEIC files onto the drop zone, or click Choose files to browse
3. Select your output format (JPEG or PNG) and adjust quality if needed
4. Click Convert all
5. Download individual files or click Download all to get a ZIP of the full batch

---

## Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome | Recommended |
| Edge | Recommended |
| Firefox | Supported |
| Safari | Partial — Safari has native HEIC support which may occasionally interfere |
| Internet Explorer | Not supported |

---

## Technical Notes

- HEIC decoding is handled by [heic2any](https://github.com/alexcorvi/heic2any) (v0.0.4), loaded from jsDelivr CDN
- ZIP bundling is handled by [JSZip](https://stuk.github.io/jszip/) (v3.10.1), loaded dynamically on demand
- The tool is a single static HTML file with no build process or dependencies to install

---

## Deployment

The tool is deployed as a static site on Vercel, connected to this GitHub repository. Any push to the `main` branch triggers an automatic redeploy.

To update the tool:

```bash
git add .
git commit -m "Describe your change"
git push
```

Vercel will pick up the change and redeploy within approximately 30 seconds.

---

## Repository Structure

```
heic-converter/
├── index.html      # The entire tool — single self-contained file
└── README.md       # This file
```

---

## Maintained By

The Flagstaff Group
[github.com/flagstaff-group](https://github.com/flagstaff-group)

Our mission is to provide life skills and employment for people with disability.
