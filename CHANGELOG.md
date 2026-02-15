# YFull Finder (Ajwla) — Release Notes
This file tracks all changes, improvements, and fixes for the YFull Finder browser extension.
## [2.0.8] — 2026-02-15
**Auth Stability & Session Isolation**
### 🚀 Features
- **Fork-on-Sync Auth**: Implemented a new authentication architecture where the extension and web portal maintain independent sessions. This prevents "Token Reuse" errors that were causing frequent logouts.
- **Auto-Login Preservation**: Seamlessly logs you into the extension when you log into the portal (and vice versa) without linking the sessions permanently.
### 🛠 Improvements
- **Cross-Tab Stability**: Added safeguards to prevent multiple portal tabs from conflicting during session refreshes.
## [2.0.7] — 2026-02-14
**Mobile Polish & Localization Guard**
### 🚀 Features
- **Modernized Tooltips**: Enhanced support for mobile devices. Tooltips now work via **tap-to-toggle** on touch screens.
- **Improved Tooltip Styling**: Replaced arrows with high-performance CSS styling for better visual appearance.
### 🛠 Improvements
- **Authorship Localization**: Fixed date formatting in the Edit Modal to correctly follow the user's selected language (Spanish, English, Abkhazian, or Russian).
- **Flag Accuracy**: Fixed a bug where language codes like `cse` incorrectly displayed the Swedish flag.
## [2.0.6] — 2026-02-13
**Transliteration Polish & Stability**
### 🚀 Features
- **Synchronization Resilience**: Improved error handling for the portal synchronization.
### 🛠 Improvements
- **Transliteration Guard**: Improved transliteration engine to better handle mixed character inputs.
- **Improved Warnings**: Restored descriptive warning text for non-Latin input: "For the convenience of all users, it is better to write in Latin letters."
### 🐞 Bug Fixes
- **Latin Check Fix**: Corrected logic for Latin character detection in input fields.
---
## [2.0.5] — 2026-02-12
**Screenshot PDF Fix & Notification Polish**
### 🐞 Bug Fixes
- **PDF Export Fix**: Resolved a bug where "Full Tree" PDF screenshots in Chart mode failed.
- **Unified Notification**: Added a full-screen "Capturing..." overlay for all screenshot modes (Area, Full Tree, PDF/PNG/SVG) to provide consistent user feedback.
- **Error Handling**: Improved error alerts when screenshot capture fails.
---
## [2.0.4] — 2026-02-10
**Minor Update: Visibility Rules & Transliteration Fixes**
### 🚀 Features
- **Smart Visibility**: Restored screenshot button support for user profile/orders pages.
- **Clean UI**: Optimized mobile "plus" button visibility to reduce clutter on sample pages.
### 🛠 Improvements
- **Transliteration Overhaul**: Fixed issues with certain uppercase Cyrillic characters in the transliteration engine.
---
## [2.0.3] — 2026-02-09
**Bug Fix: Firefox Screenshot Recovery**
### 🐞 Bug Fixes
- **Firefox Fix**: Resolved a critical issue in Firefox where the screenshot tool would fail due to security restrictions.
- **Improved Performance**: Resolved infinite retry loop during screenshot capture on restricted environments.
### 🚀 Features
- **Scientific Tree Screenshot**: Full capture support for Scientific View, ensuring all branches and the timeline are visible.
- **Chart View Screenshot**: Added support for Diagram View with full expansion of nested structures.
- **Smart Watermark**: Adaptive watermark positioning to prevent data obstruction.
---
## [2.0.2] — 2026-02-06
**Maintenance Update**
### 🛠 Improvements
- **Version Standardization**: Synchronized version numbers across extension components.
- **Translation Maintenance**: Audited and improved internal translation mapping for better consistency.
---
## [2.0.1] — 2026-02-06
## [2.0.0] — 2026-02-06
**Major Feature Release: Screenshot Tool & Expansion**
### 🚀 Features
- **Advanced Screenshot Tool**: Capture YFull tree pages with full export options:
  - **Selection Mode**: Draw a rectangle to capture specific areas.
  - **Multi-format Export**: Save as PNG, SVG, or PDF.
  - **Canvas Watermark**: Branded overlay with customizable logo.
  - **Full-page Capture**: Nested tree containers captured correctly.
- **Spanish Language Support**: Full localization for Spanish language.
- **Krsna Slava Field**: Added Serbian patron saint field (`krsna_slava`) to samples schema.
- **New Ethnic Flags**: Added XAL (Kalmyk), CHV (Chuvash), KUR (Kurdish), HYE (Armenian) flags.
- **Mobile Add Button Toggle**: Settings option to control visibility of quick-add buttons on touch devices.
### 🛠 Improvements
- **Dynamic Plus Button**: Rebuilt button creation for better performance (reduces load time).
- **Button Sizing**: Optimized sizing for edit and add buttons.
- **Screenshot Modal Redesign**: Modern UI with separate tabs for format and mode selection.
- **Library Upgrade**: Upgraded screenshot engine for better SVG/PDF support.
### 🐞 Bug Fixes
- **Selection Overlay Visibility**: Fixed issues preventing selection rectangle from displaying.
- **Modal Lockup**: Resolved issues with session validation.
- **Sample ID Normalization**: Fixed uppercase normalization errors.
- **Sync Improvements**: Corrected auto-sync and portal-to-extension synchronization.
- **Input Validation**: Link field now validates URL format before submission.
---
## [1.0.0] — 2026-01-18
**Initial Release (Manifest V3)**
### 🚀 Key Features
- **Modern UI Architecture**: Full support for Manifest V3 with improved security and performance.
- **Enrichment Engine**: Injects genealogical data (Surnames, Tribes, Regions) directly into YFull.com sample pages.
- **Project Support**: Seamless integration with supported databases.
- **Premium Design System**: Choice between "Lite" (high-density) and "Premium" (glassmorphism) UI themes.
- **Localized Experience**: Full support for Abkhazian, English, and Russian languages.
- **Secure Authentication**: Integration for user profiles and attribution.
- **Admin Tools**: Direct synchronization and change request management for authorized users.
### 🛠 Improvements & Fixes
- **Optimized Performance**: Multi-sample batch loading reduces API requests.
- **Interactive Tooltips**: Detailed field info using custom styled popups.
- **Cross-Browser Styling**: Refined SVG flags and icon alignment for Chrome and Firefox.
- **Privacy First**: Minimal permissions and restricted host access.
---
## [1.2.0] — 2026-01-30
**Ethnic Flag Standardization & Expansion**
### 🚀 Key Features
- **Major Flag Expansion**: Added 30+ new ethnic flags for Caucasian, Turkic, Uralic, and Baltic groups.
- **Flag Aspect Ratio Standardization**: All SVG flag assets have been standardized to a consistent aspect ratio to ensure uniform display across all browser environments.
### 🛠 Improvements
- **Simplified Styling**: Refined the flag rendering logic for consistent scaling.
- **Resource Access**: Improved asset loading reliability.
- **Improved Portability**: Standardized visual assets to prevent rendering artifacts.
### 🐞 Bug Fixes
- **Transparency Issue**: Resolved bug where newly added flags appeared transparent.
- **Restored Assets**: Manually restored and standardized the Tatar flag based on user request.
---
## [1.1.6] — 2026-01-24
**Attribution & Anonymous Toggle Fix**
### 🐞 Bug Fixes
- **Anonymous Toggle Now Visible**: Fixed issue where the "Submit Anonymously" toggle was not appearing for logged-in users.
- **Correct Attribution**: Change requests now correctly include username information.
- **Anonymous Logic**: Fixed logic which was incorrectly defaulting to anonymous in some cases.
### 🛠 Technical Improvements
- Improved user data loading reliability.
- Optimized UI rendering sequence.
---
## [1.1.5] — 2026-01-23
### 🛠 Improvements
- **Mobile Layout Fix**: Chips now display horizontally with scroll instead of stacking vertically on mobile devices.
- **Input Validation**: Added input length limits and new validation error messages.
## [1.1.4] — 2026-01-23
### 🛠 Improvements
- **Mobile Experience**: Improved visibility for Edit and Add buttons on touch devices/mobile browsers.
- **Bug Fix**: Restored "Quick Add" (+) button functionality.
## [1.1.3] — 2026-01-23
### 🚀 Features
- **Universal Transliteration**: One-click transliteration (Cyrillic to Latin) now supported for all text fields, enabling easier data entry in English.
- **Localized Chip Tooltips**: Hovering over data chips now displays the field name in the user's selected language.
### 🛠 Improvements
- **Lite Theme Polish**:
    - **Refined Typography**: Updated fonts for a premium aesthetic.
    - **Space Optimization**: Improved spacing and density for the Lite theme.
    - **Visual Clarity**: Improved contrast for data chips and action buttons.
## [1.1.1] — 2026-01-22
### Changed
- Production hardening.
- Internal version bump.
## [1.1.0] — 2026-01-21
**Major Synchronization & Performance Update**
### 🚀 Features
- **Synchronization Tools**: Enhanced tools for data management.
- **Transliteration Support**: Dynamic transliteration for surnames and names in the Edit Modal.
- **Enhanced Visitor Tracking**: Advanced identification system.
### 🛠 Improvements
- **Performance Optimization**: Reduced server overhead by 80%.
- **Design Refinement**:  Restored vertical density for a "bone-tight" Lite theme.
- **Secure Auth Sync**: Seamless session sharing between the web portal and extension.
- **Extended Localization**: Added Abkhazian locale.
### 🐞 Bug Fixes
- **UI Consistency**: Fixed popup dimensions and restored desktop-first layouts.
- **Security Audit**: Manifest V3 compliance check.
