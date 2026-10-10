# File Forge
A static, browser-only file converter by Lucas. No backend, keys, paid APIs, or file uploads to a server.

## Conversions
- Text / Markdown / HTML / CSV / JSON → real DOCX, TXT, escaped HTML, JSON.
- CSV ↔ JSON (JSON must be an array for CSV).
- DOCX → extracted text, HTML, or a text-only DOCX.
- Browser-readable images → PNG, JPEG, WebP, image DOCX.
- Browser-readable video → DOCX storyboard, JPEG / PNG still, metadata TXT.
- Browser-readable audio → 16-bit PCM WAV.
- Any file → ZIP, GZIP, metadata JSON, first-64-KB hex preview.
- GZIP → decompressed bytes.

MP4 → Word means a storyboard with frames and metadata, not speech transcription. Unsupported conversions are not presented as available. Image output uses a white background, including PNG/WebP. DOCX conversion extracts text without original formatting. PDF/OCR, arbitrary video transcoding, legacy DOC/XLS/PPT and speech recognition are not implemented.

## Hosting
Serve this directory as a static website. For GitHub Pages, select Settings → Pages → Deploy from a branch → main / root. No build step needed. Browser conversion functions require current browser media/Compression Streams support. Input limit 100 MB. Large decoded media may exceed memory limits.

## Privacy
Files are processed locally. A Google Fonts CSS request loads typography; it never receives the uploaded files.
