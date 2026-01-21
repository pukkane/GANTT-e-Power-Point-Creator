# mYcOMOANY Timeline

mYcOMOANY Timeline is a **web-based Gantt and presentation generator** designed to create **structured, professional PowerPoint decks** starting from an interactive project timeline.

It is a **single-page HTML/JavaScript application**, runs entirely in the browser, requires **no backend**, and produces **high-quality PPTX files** suitable for executive, technical, and project governance presentations.

---

## Key Features

### Timeline & Gantt
- Interactive **Gantt chart editor**
- Support for:
  - Phases
  - Tasks with start/end dates
  - Progress percentage
  - Milestones
  - Vertical reference markers
- Multiple timelines in the same project, each with an optional **suffix** (e.g. *Pilot*, *Wave 1*, *Release A*)
- Automatic ordering and rendering consistency between UI and PPTX export

---

### PowerPoint (PPTX) Export
- One-click **PPTX generation** using `PptxGenJS`
- Corporate-style layout with:
  - Cover slide
  - Agenda
  - Structured content sections
  - Timeline narrative + visual chart
  - SAL (Status / Issues / Notes)
  - Final “Thank you” slide
- **Automatic slide splitting**:
  - Any text-heavy slide is automatically paginated
  - Titles are never broken
  - Page indicators (e.g. `1/3`) are added consistently
- High-resolution Gantt chart export (SVG → PNG at 300 DPI)

---

### Timeline Slides Structure

For each timeline, the export produces:

1. **“Project phases, timeline and milestones”**  
   Textual, readable narrative including:
   - Phase breakdown
   - Tasks with dates, duration, progress
   - Milestones
   - Vertical markers  
   Automatically split across multiple slides if needed.

2. **“Timeline Chart”**  
   Visual Gantt chart image:
   - Centered and scaled proportionally
   - Same suffix and naming as the textual slide
   - Consistent disclaimer footer

---

### Content Sections Included

The PPTX includes the following sections (all editable in the UI):

- Agenda (auto-generated, SAL-aware)
- Project purpose
- Context and objectives
- Scope
- Stakeholders (mYcOMOANY / Client)
- Governance
- Deliverables
- Prerequisites
- BOM – Licenses
- BOM – Materials
- Communication & Collaboration plan
- Risks and dependencies
- Out of scope
- Next steps & Q&A
- SAL history (Issues & Notes, per reporting date)

All sections automatically paginate if content exceeds a single slide.

---

## Image & Background Customization

The application supports **full visual customization** of PPTX slides through background images.

### Supported Backgrounds
You can configure different background images for:
- Cover slide
- Agenda slide
- Middle/content slides
- Final slide

Backgrounds can be:
- Solid colors
- PNG / JPG images
- Corporate templates

Images are automatically stretched or fitted depending on configuration.

---

## Theme Customization

Centralized theme configuration allows you to align the deck with corporate branding:

- Fonts:
  - Heading font
  - Body font
- Colors:
  - Accent color (used consistently across cover, timeline labels, final slide)
  - Text colors
- Margins and spacing
- Font sizes hierarchy

The final slide (“Thank you”) uses:
- The same font as the cover title
- White main text
- Project name in the same accent color used on the cover

---

## Save & Restore Projects

- Save the entire project state as a **JSON file**
- Restore a project exactly as it was saved
- Backward-compatible loading (older files continue to work)
- No cookies, no local storage pollution

---

## CSV Import

- Import timelines from CSV
- Automatically creates:
  - Phases
  - Tasks
  - Dates
- Fully compatible with PPTX export and slide splitting

---

## Technology Stack

- Vanilla HTML / CSS / JavaScript
- No frameworks
- `PptxGenJS` for PowerPoint generation
- SVG rendering for Gantt chart
- Client-side only (offline-capable)

---

## Usage

1. Clone or download the repository
2. Open `index.html` in a modern browser (Chrome, Edge recommended)
3. Build your timeline and content
4. Export the PPTX

No installation, no build step, no server required.

---

## Browser Compatibility

- Chrome (recommended)
- Microsoft Edge
- Firefox (supported, minor rendering differences possible)

---

## License

This project is released under the **MIT License**.

You are free to:
- Use
- Modify
- Distribute
- Use commercially

Attribution is appreciated but not required.

---

## Disclaimer

This tool generates **indicative project timelines**.  
Final schedules, commitments, and governance decisions must be validated through formal project management processes.

---

## Contributing

Contributions are welcome:
- Bug fixes
- UX improvements
- Additional export formats
- Layout or theme enhancements

Please open an issue or submit a pull request.

---

## Author

Developed as a practical, presentation-oriented timeline tool focused on **clarity, executive readability, and real-world project usage**.


