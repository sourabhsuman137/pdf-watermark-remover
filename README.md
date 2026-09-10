# 📄 PDF Watermark Remover

A simple, privacy-friendly browser tool that removes light logos and watermarks from PDF files — **100% client-side**, no server, no upload, no data ever leaves your device.

🔗 **Live Demo:** [https://YOUR-USERNAME.github.io/pdf-watermark-remover/](https://sourabhsuman137.github.io/pdf-watermark-remover/)

---

## ✨ Features

- 🔒 **Fully client-side** — your PDF never leaves your browser
- 🖼️ Removes faint/light watermarks and logos automatically
- 📐 Preserves original page orientation (portrait & landscape)
- ⚡ Adjustable quality mode (better quality vs. smaller file size)
- 📊 Live progress bar with page count and time estimates
- 💾 One-click download of the cleaned PDF

## 🚀 How It Works

1. Upload a PDF file
2. Each page is rendered to a canvas using [PDF.js](https://mozilla.github.io/pdf.js/)
3. Very light/faint pixels (likely watermarks) are whitened out
4. Cleaned pages are reassembled into a new PDF using [jsPDF](https://github.com/parallax/jsPDF)
5. Download the result — original filename is preserved with a suffix

## 🛠️ Tech Stack

- Vanilla HTML, CSS, JavaScript (no framework, no build step)
- [PDF.js](https://mozilla.github.io/pdf.js/) — for reading and rendering PDF pages
- [jsPDF](https://github.com/parallax/jsPDF) — for generating the output PDF

## 📦 Usage

### Option 1: Use it online
Just open the [live demo](https://sourabhsuman137.github.io/pdf-watermark-remover/) link — no install needed.

### Option 2: Run locally
```bash
git clone https://github.com/YOUR-USERNAME/pdf-watermark-remover.git
cd pdf-watermark-remover
```
Then simply open `index.html` in your browser.

## ⚠️ Limitations

- Works best on **light/faint** watermarks — solid or dark logos won't be removed
- Output pages are rendered as images (JPEG), so PDF text is no longer selectable in the result
- Large PDFs with many pages may take a while to process, since everything runs in-browser

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

## 📄 License

This project is licensed under the [MIT License](LICENSE).
