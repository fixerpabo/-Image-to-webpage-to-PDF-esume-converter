# Resume Webpage with PDF/DOCX Download

A professional resume webpage with direct PDF and DOCX download functionality. The webpage is sized to A4 dimensions and generates downloadable files that preserve all styling and content.

## Features

- **A4 Dimensions**: Webpage container is exactly 210mm × 297mm (A4 size)
- **Professional Design**: Two-column layout with dark green sidebar and white content area
- **PDF Download**: Text-based, searchable PDF with clickable links
- **DOCX Download**: Word-compatible document with preserved styling
- **Responsive**: Optimized for both screen viewing and printing
- **ATS-Friendly**: Applicant Tracking Systems can read the PDF text

## Live Demo

View the live resume: [GitHub Pages URL](https://fixerpabo.github.io/-Image-to-webpage-to-PDF-esume-converter/)

## Technologies Used

- **HTML5**: Semantic structure
- **CSS3**: Grid layout, custom properties, print styles
- **JavaScript**: Download functionality
- **Libraries**:
  - [html2pdf.js](https://github.com/eKoopmans/html2pdf.js) - PDF generation
  - [html-docx-js](https://github.com/evidenceprime/html-docx-js) - DOCX generation
  - [FileSaver.js](https://github.com/eligrey/FileSaver.js) - File downloads

## Usage

### View Locally

1. Clone the repository:
```bash
git clone https://github.com/fixerpabo/-Image-to-webpage-to-PDF-esume-converter.git
cd -Image-to-webpage-to-PDF-esume-converter
```

2. Serve the files using any static server:
```bash
# Using Python
python -m http.server 8080

# Using Node.js
npx http-server . -p 8080
```

3. Open `http://localhost:8080` in your browser

### Download Resume

- **PDF**: Click "Download PDF" button - saves `Chetana_CN_Resume.pdf` to Downloads folder
- **DOCX**: Click "Download DOCX" button - saves `Chetana_CN_Resume.docx` to Downloads folder

## File Structure

```
.
├── index.html          # Main HTML structure
├── styles.css          # All styling including print styles
└── README.md          # This file
```

## Customization

### Update Content

Edit `index.html` to change:
- Personal information
- Work experience
- Skills
- Education
- Links

### Modify Styling

Edit `styles.css` to customize:
- Colors (see CSS variables at top of file)
- Fonts
- Layout proportions
- Spacing

### Change Colors

```css
:root {
    --sidebar-bg: #1a3c34;      /* Dark green sidebar */
    --sidebar-text: #e0e0e0;    /* Light gray text */
    --main-bg: #ffffff;         /* White background */
    --main-text: #2c2c2c;       /* Dark text */
}
```

## Technical Details

### PDF Generation
- Uses html2pdf.js for text-based PDF
- Format: A4 portrait (210mm × 297mm)
- Zero margins (edge-to-edge content)
- Single-page output
- Preserves clickable hyperlinks

### DOCX Generation
- Uses html-docx-js + FileSaver.js
- Table-based layout for Word compatibility
- Preserves two-column design
- All content and styling maintained

### Print Styles
- Comprehensive `@media print` rules
- Preserves background colors
- Hides download buttons
- Optimized font sizes for single-page fit

## Browser Compatibility

- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- Mobile browsers: ✅ Responsive design

## License

MIT License - feel free to use this template for your own resume!

## Author

**Chetana CN**
- LinkedIn: [c-n-chetana](https://www.linkedin.com/in/c-n-chetana-93a716258/)
- GitHub: [@fixerpabo](https://github.com/fixerpabo)
- Medium: [@chinnanagireddy.chetana](https://medium.com/@chinnanagireddy.chetana)

## Acknowledgments

- Design inspired by modern resume builders
- Built with vanilla HTML, CSS, and JavaScript
- No frameworks required!
