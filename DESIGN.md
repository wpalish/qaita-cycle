---
name: QaitaCycle
description: The inherited working cabinet for explicit date windows, preserved bilingual instructions and owner-authored manual results.
colors:
  primary: "#126653"
  primary-hover: "#0b5343"
  navy: "#183e60"
  ink: "#172e45"
  page: "#edf3f8"
  surface: "#ffffff"
  line: "#b9cbd9"
  navigation-surface: "#dce9f3"
  muted: "#46627a"
  input-stroke: "#7894aa"
  link: "#174e7e"
  pending: "#795200"
  error: "#942721"
  error-surface: "#fff0ee"
  focus: "#bd671a"
  selection-surface: "#b7ded2"
  selection-ink: "#132f29"
typography:
  primary-heading:
    fontFamily: 'system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif'
    fontSize: "2rem"
    lineHeight: 1.15
    letterSpacing: "-0.025em"
  section-heading:
    fontSize: "1.3rem"
  brand:
    fontSize: "1.4rem"
    fontWeight: 740
  body:
    fontFamily: 'system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif'
  label:
    fontWeight: 600
  supporting:
    fontSize: "0.9rem"
  preformatted:
    fontSize: "0.85rem"
rounded:
  control: "7px"
  panel: "12px"
spacing:
  evidence-gap: "0.4rem"
  inline-gap: "0.5rem"
  action-gap: "0.6rem"
  control-inset: "0.7rem"
  table-cell: "0.9rem"
  unit: "1rem"
  page-inline: "1.25rem"
  panel-inset: "1.4rem"
  section: "2rem"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.surface}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.navy}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  button-default:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.surface}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  field:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "{spacing.control-inset}"
    width: "100%"
  panel:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.panel}"
    padding: "{spacing.panel-inset}"
  navigation-current:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.navy}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  record-table:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.panel}"
    width: "100%"
  snapshot-disclosure:
    padding: "0.7rem 0"
  error-notice:
    backgroundColor: "{colors.error-surface}"
    textColor: "{colors.error}"
    rounded: "{rounded.control}"
    padding: "{spacing.unit}"
---

# Design System: QaitaCycle

## Overview

**Creative North Star: "The Shared Work Cabinet"**

QaitaCycle extends the project's own DalelCheck Shared Work Cabinet: navy identity and navigation, a pale blue workspace, white labelled native forms, green explicit actions and system typography. The owned incumbent authority is the [DalelCheck design system](../dalel-check/DESIGN.md) and [sidecar](../dalel-check/.impeccable/design.json), pinned to own-source commit `8bb1213ca5fb564b5f766edbbb8892fb04440bff`. The settled inherited direction supplies the qualitative language for this scan; no new visual-world workshop or image comp is introduced.

Its character is flat, direct and readable. A full dated decision table separates an unsaved window from a saved record. An occurrence keeps its original owner, due time and authored RU/KK instructions above a once-only manual-result form. Written labels distinguish waiting, refusal, saved assertions and retained unsaved input. These are synthetic working records; a due date or manual result does not establish real work.

**Key Characteristics:**

- Inherited navy shell, cool workspace and flat white native controls.
- Restrained system type, visible labels and a readable dated table.
- Authored bilingual snapshots remain visible before manual actions.
- Explicit unsaved, refused, saved and retained-input states.
- Native focus, text selection, date fields, selects and disclosures.

## Colors

The frontmatter owns the implemented values extracted from [the stylesheet](public/styles.css#L1). Descriptive names and derived inspection ramps continue the identical owned incumbent palette. Ramps in the [sidecar](.impeccable/design.json) are metadata, not additional interface colors.

### Primary

- **Working Green / Deep Working Green** (`primary`, `primary-hover`): explicit primary and submit actions, including preview, publication, whole-window save and manual-result save. The green fill identifies an available action; its label identifies what will be written.

### Secondary

- **Cabinet Navy** (`navy`): identity header, baseline filled buttons, secondary borders and navigation text.
- **Link Blue** (`link`): ordinary links and native field carets.

### Tertiary

- **Pending Amber** (`pending`): the written due/pending explanation below the waiting heading.
- **Error Red / Pale Error** (`error`, `error-surface`): refused-request notice with focused written explanation.
- **Focus Amber** (`focus`): visible focus outline on controls, headings and disclosures.
- **Soft Selection Green / Selection Ink** (`selection-surface`, `selection-ink`): native selected text.

### Neutral

- **Cabinet Ink** (`ink`): primary reading text and authored instructions.
- **Cool Workspace / White Surface** (`page`, `surface`): page ground and native inputs, panels, notices and tables.
- **Divider Blue / Navigation Mist** (`line`, `navigation-surface`): one-pixel boundaries, navigation ground and table headers.
- **Supporting Slate / Field Slate** (`muted`, `input-stroke`): helpers/footer and field strokes/scrollbars.

**The Inherited Shell Rule.** Extend the existing Shared Work Cabinet palette, type and native control grammar.

## Typography

The system stack serves body, headings and controls; no font asset is loaded. The fixed task heading, smaller section heading, heavier brand and connected label roles are normative in frontmatter. Unspecified body size and heading weights retain browser defaults. Paragraphs have a maximum measure (72ch) and line height (1.6). Tables and native date fields use tabular numerals; data/audit preformatted text uses the smaller `preformatted` role. Source: [heading and paragraph rules](public/styles.css#L63), [fields](public/styles.css#L91), [preformatted text](public/styles.css#L235).

The shell language is Russian. Authored instruction text uses separate RU and KK nodes with `lang` attributes. Snapshot paragraphs preserve line breaks through `white-space: pre-wrap`; long headings, paragraphs and digests wrap instead of clipping. Rationale and unsaved rationale stay authored text. Source: [authored helper](public/app.js#L4), [routine fields](public/app.js#L28), [snapshot renderer](public/app.js#L29), [retained rationale](public/app.js#L46).

**The Authored Text Rule.** Preserve authored RU/KK text, language nodes and visible line breaks; do not silently rewrite a historical instruction or rationale.

## Layout

Header and navigation share inline padding (`max(1.25rem, calc((100% - 1160px) / 2))`). Main is centered at maximum width (1200px), padding (`2rem 1.25rem`) and minimum height (75vh). Navigation wraps at every width. List actions wrap with their existing gap; search and archive visibility sit above a native record table. White panels contain connected fields. The inherited optional work and paired-row grids remain defined in CSS, but this app's main window and occurrence forms are single-column. Source: [shell and grids](public/styles.css#L26), [actions](public/styles.css#L144), [search/table rules](public/styles.css#L290), [final navigation rule](public/styles.css#L417).

Window entry orders publication → inclusive dates → rationale → preview control, then written preview state, counts, every calendar-date decision and the explicit whole-window save. Saved window detail places actor, time and rationale before a native exact-rule disclosure and the recorded decision table. Occurrence detail orders original owner/due/version → original RU/KK snapshot → waiting or saved-result state → eligible manual-result form or saved metadata → any separate retained-input panel → refresh/return. Source: [window renderers](public/app.js#L32), [occurrence renderer](public/app.js#L35).

At the source-defined stacked breakpoint (700px), optional grids become one column, page/panel insets reduce, header identity narrows and button/navigation sizing adapts. At (600px), search stacks, cells gain minimum width (140px), table type reduces and the horizontal-scroll hint appears. Labelled focusable wrappers own table overflow. These are [source-defined responsive rules](public/styles.css#L258); mobile rendering has not been verified.

### Evidence scope and freshness

The [finish review](docs/finish-review.json) initially returned `fix` for F1, the rationale-loss recovery path. Its later `ship` verdict resolves **F1 only** using the edited source, two current recovery captures and supplied synthetic state/audit comparisons. It does not constitute a fresh whole-surface review. The nine original captures below remain historical pre-F1 evidence. The two current F1 captures show the edited recovery branches. All eleven were opened in this documentation pass and are nonblank full-page desktop states without visible clipping or loading artifacts. Actual width (1280 CSS px) and scroll width (1280) remain builder-reported; raster dimensions and hashes were independently checked. Every shipping JPEG is byte-identical to its review original in [capture provenance](docs/capture-provenance.json).

| Shipping capture | Freshness | Raster dimensions | SHA-256 |
| --- | --- | --- | --- |
| [preview-1280](docs/preview-1280.jpg) | Historical pre-F1 | 1280 × 1592 | `cfaac85a337731cdbda4739e86018ac602cc868cd8a0c7794f7aa9f9bd4a832b` |
| [stale-window-1280](docs/stale-window-1280.jpg) | Historical pre-F1 | 1280 × 1661 | `109d4a876e3198538b9bb61103d5960ec9875e0ea6b7896ac4d121357fa9fcb4` |
| [window-saved-1280](docs/window-saved-1280.jpg) | Historical pre-F1 | 1280 × 1157 | `692e9a1df4066c2d13a77cf15db99029ccdd8a8637ad032cd5e2088b41fb142e` |
| [owner-form-1280](docs/owner-form-1280.jpg) | Historical pre-F1 | 1280 × 1053 | `fb4afd6d0bc6cfbbe7c4cd112bf25ab2e88e733751d94cb24713cb200fcfe4df` |
| [stale-outcome-1280](docs/stale-outcome-1280.jpg) | Historical pre-F1 | 1280 × 1122 | `1ddacec9417c935b70197ed125b9c6ae27c649a9316902c60543c8bfdf7369a7` |
| [completed-1280](docs/completed-1280.jpg) | Historical pre-F1 | 1280 × 946 | `e9c9db5e33a3b01068dc3ad112432c641f639f6232ee3f9ca9cc7ce00ef52e2b` |
| [zero-preview-1280](docs/zero-preview-1280.jpg) | Historical pre-F1 | 1280 × 1934 | `c8946db4af9c0213c9c040df868da8d0087686086d34733583a076a09e150cfe` |
| [zero-saved-1280](docs/zero-saved-1280.jpg) | Historical pre-F1 | 1280 × 1794 | `2b1ef7cd1f74e773c98fba6397a0cce84108fa4e6b0b9ce0d55fd948d1c69c3d` |
| [early-refusal-1280](docs/early-refusal-1280.jpg) | Historical pre-F1 | 1280 × 1122 | `490210ec13adb4891a20a1e92cdef2b27bcf241d4ee6b9e01e1b37612dbd1540` |
| [f1-pending-refreshed-1280](docs/f1-pending-refreshed-1280.jpg) | Current F1 recovery | 1280 × 1053 | `25a4fd12cc8a9134f19cd8b10152600c0c68552a679051f52bbb8fe7ef4d1a54` |
| [f1-resolved-retained-1280](docs/f1-resolved-retained-1280.jpg) | Current F1 recovery | 1280 × 1199 | `e50465b428cb7acf10cd7454fdd364dcc7ab3b82fe7677b9bd97515f3120b5a6` |

The original nine came from the synthetic local IAB runtime (`127.0.0.1:8856`); the two F1 captures came from the isolated synthetic fixture (`localhost:8899`). Images are evidence records, not decorative assets, and no pixel edits are implied. The review records unchanged before/after-refresh fixture proofs, followed by a separate explicit pending-owner submit. This documenter did not repeat those browser interactions, the detector, backend tests or state/audit comparisons. Builder-reported Tab/Return submission, authored language nodes, focus and native disclosure checks are bounded observations recorded in [browser proof](docs/browser-proof.json), not an exhaustive accessibility verdict.

Only actual 1280 desktop capture evidence is recorded. Mobile/390px, 1440px, touch, screen-reader, exhaustive keyboard/hover/loading/empty/overlong and every account/archive state remain unverified. No backend, concurrency, isolation, restore authenticity, transport or security certification follows from this visual packet. It makes no claim of calendar integration, notifications or real work outcomes. The review's nonblocking notes on touching occurrence refresh/return buttons and punctuation spacing remain recorded; these docs do not imply they were fixed.

## Elevation & Depth

No shadow, transition, animation or backdrop treatment is defined. Pale page ground, white native surfaces, one-pixel boundaries and section spacing convey hierarchy. Hover brightens buttons; primary hover also deepens the fill without motion. Programmatic task/preview-heading focus and the focused refusal notice provide continuity after content replacement. Source: [button states](public/styles.css#L120), [evidence boundary](public/styles.css#L166), [focus ring](public/styles.css#L246).

## Shapes

Controls and notices use the smaller recorded radius; form panels and table wrappers use the larger one. Buttons and native disclosure summaries have minimum height (44px). Textareas start at minimum height (100px) and resize vertically. Native disclosure markers remain visible. There are no implemented chips, custom date pickers or floating overlay components to document. Source: [forms and buttons](public/styles.css#L84), [disclosures](public/styles.css#L225), [table wrapper](public/styles.css#L290).

## Components

### Buttons, Fields and Navigation

Primary and submit actions use green. Secondary refresh, return and archive controls use white with navy text and border; the navy-filled baseline remains in CSS. Buttons have inset (`0.65rem 1rem`), weight (600), hover brightness (1.13), disabled opacity (0.55) and final disabled `cursor: not-allowed`. Focus-visible is an amber outline (3px) with offset (3px). The initiating asynchronous button is disabled during its request. Source: [button rules](public/styles.css#L120), [final overrides](public/styles.css#L377), [request helper](public/app.js#L6).

Native text, date, select and rationale fields keep connected labels, required semantics, full width, white ground, the smaller radius, field stroke and blue carets. The user picks from a native select, and dates use native date controls. Read-only retained rationale uses the same textarea surface so it remains selectable. Source: [field helpers](public/app.js#L9), [window form](public/app.js#L33), [manual result and recovery](public/app.js#L42).

The header shows linked brand and account/role. Active collection navigation uses a white bordered button and `aria-current="page"`; inactive buttons remain transparent on Navigation Mist. Windows is the initial collection. The skip link appears on focus; replaced task headings receive programmatic focus. Notices use `role="status"`, `aria-live="polite"` and a focus target; empty notices hide. Refusal turns the notice pale red. Source: [shell semantics](public/index.html#L10), [navigation](public/app.js#L12).

### Tables and Exact Snapshot Disclosure

Search and archive visibility precede the native record table. Headers use `scope="col"`; cells align left/top, wrap and use tabular numerals. A labelled focusable wrapper provides horizontal overflow. Empty collections show a written next step. The window decision table has date, written decision, owner and original due time, without action controls in its rows. Source: [record renderer](public/app.js#L26), [decision renderer](public/app.js#L32).

The native **Точное опубликованное правило** disclosure holds code/version, title, both authored instruction texts and original owner/weekdays/time. The same snapshot content precedes the occurrence state directly. Publication preview says **Предпросмотр · ещё не опубликован** before its explicit publish action; changing the selected rule clears that preview. Source: [snapshot/publication](public/app.js#L29), [saved window](public/app.js#L34).

**The Snapshot Rule.** Keep the displayed publication and original occurrence snapshot explicit; a newer version never visually replaces an older date's owner, time or instructions.

### Window Preview, Refusal and Saved Window

**Предпросмотр дат · ещё не записано** leads with counts, the preserved-key explanation and every calendar-date decision. Preview labels are **Создать дату**, **Сохранить прежнюю дату** and **Не назначено этим правилом**. Only the subsequent **Создать всё окно один раз** action writes. Editing the window fields clears its preview. A refused save focuses the notice and changes the heading to **Запись отказала · заново проверьте даты**, keeping the entered form values. Source: [window form and preview](public/app.js#L32).

A saved window shows actor/time/rationale and **Сохранённое целое окно**; newly created rows say **Дата создана**. Zero-new windows remain real saved records: the example shows the newer beta/10:00 publication while all existing alpha/09:00 dates are kept. The table is historical and has no second-save control. Source: [saved window renderer](public/app.js#L34), [historical zero-new capture](docs/zero-saved-1280.jpg).

**The Written State Rule.** Name unsaved, refused and saved states in text; counts, color and a preview alone never assert that a write occurred.

### Manual Result and Refresh Recovery

The occurrence shows original owner and due time before the exact bilingual snapshot, then **Ожидает ручного результата** and an amber explanation of whether the due time has arrived. A pending, unarchived occurrence owned by the current account has a native **Ручной результат** select and required **Основание результата** textarea. Its two options are **Выполнение отмечено вручную** and **Пропуск отмечен вручную**; the server may still refuse an early submit. Other readers get a written owner-only explanation. Source: [occurrence renderer](public/app.js#L35).

A saved outcome replaces the result form with its written manual status, rationale, actor/time and ledger number. It remains an explicit manual assertion, without edit, reversal or reopen controls. Refresh does not itself write. The F1 fix captures the current unsaved status and rationale before fetching state, then rehydrates them only in the eligible pending-owner form. The new renderer captures the fresh revision; another explicit submit is required. Source: [saved/pending branches](public/app.js#L38), [refresh callback](public/app.js#L50), [current eligible recovery capture](docs/f1-pending-refreshed-1280.jpg).

If refreshed state already has a result, or the pending form is no longer available, nonempty retained input appears in a distinct white panel headed **Несохранённый ввод после обновления**. It names the previously selected status and shows **Несохранённое основание** in a `readOnly` textarea. The text explicitly says these values are for copying, do not replace the saved result and are not automatically sent. This panel has no outcome-submit control. Source: [read-only recovery branch](public/app.js#L46), [current resolved recovery capture](docs/f1-resolved-retained-1280.jpg).

**The Unsaved Recovery Rule.** Preserve unsaved input across explicit refresh, but display ineligible retained text separately from the saved record and require a new explicit action for any eligible write.

### Documentation Examples

The [schemaVersion 2 sidecar](.impeccable/design.json) supplies thirteen self-contained static synthetic examples grounded in the current CSS and DOM: primary/secondary actions, navigation, native field, window-entry panel, record table, exact-rule disclosure, unsaved decision table, zero-new saved window, owner form, saved outcome, error notice and read-only retained input. They use scoped `ds-` classes and non-submitting action buttons without application handlers. Native inputs and disclosures retain ordinary browser behavior. Compact tables omit other dates for documentation only; production renders every report row. These snippets are not additional reviewed captures or executable workflows.

[PRODUCT.md](PRODUCT.md) and the [surface brief](.impeccable/surfaces/public-app-js.md) bound this inherited interface to synthetic recurring work in one shared staff area. Design documentation does not add tenant isolation, a real calendar, external integrations, notifications or evidence of actual performance.

## Do's and Don'ts

### Do:

- Do retain the inherited navy shell, pale workspace, green explicit actions and white native controls.
- Do keep connected labels, visible focus, native disclosure markers and column-scoped table headers.
- Do preserve authored RU/KK instructions, language attributes, rationale and visible line breaks.
- Do show original owner, due time and publication version before the manual-result action.
- Do place every date decision before the explicit whole-window save.
- Do distinguish unsaved preview, refused write, saved window and manual outcome in words.
- Do keep zero-new saved windows and the old owner/time of kept dates visible.
- Do retain status and rationale across explicit occurrence refresh.
- Do separate read-only retained unsaved text from a saved outcome when editing is unavailable.
- Do let long text and digests wrap without a fixed-height crop.

### Don't:

- Don't replace the inherited identity with ornamental media, display lettering or animation.
- Don't replace native dates, selects, tables or disclosures with decorative imitations.
- Don't present a preview or retained rationale as a saved record.
- Don't present elapsed time, refresh or a manual result as proof of real work.
- Don't display a newer rule's owner/time as the original obligation of a kept date.
- Don't offer outcome edit, reopen, reversal or an administrator authorship bypass.
- Don't imply a real calendar, notifications, AI, external messaging or customer outcomes.
- Don't describe a digest or this visual packet as authenticity or security certification.
- Don't call the F1-only verdict a fresh whole-surface approval.
- Don't claim mobile/390px, 1440px, touch, screen-reader or exhaustive keyboard verification from these 1280px captures.
