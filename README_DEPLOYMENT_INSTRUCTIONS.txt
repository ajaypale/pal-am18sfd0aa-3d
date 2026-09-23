================================================================================
PAL ENGINEERS - HEAT EXCHANGER AM18SFD0AA 3D WEB DEPLOYMENT PACKAGE
================================================================================

This package contains the complete, production-ready, interactive 3D Web CAD suite
for the AM18SFD0AA Heat Exchanger and Replacement Tube Bundle.

It runs 100% client-side via hardware-accelerated WebGL.
No backend server, no PHP, and no database required.
Works smoothly across all modern web browsers: Google Chrome, Apple Safari,
Mozilla Firefox, Microsoft Edge, and Android/iOS mobile devices.

--------------------------------------------------------------------------------
PACKAGE CONTENTS:
--------------------------------------------------------------------------------
1. index.html                   : Master 3D CAD Inspection Suite (Interactive 3D Viewer)
                                  - Option A: Replacement Tube Bundle (Default View)
                                  - Master Cutaway Inspection Model
                                  - Exploded 3D Assembly (with 0-100% Separation Slider & Auto-Animate)
                                  - Option B: Complete Exchanger Assembly
                                  - Individual Components (Tubes, Baffles, Tubesheets, Shell, Headers)
2. bundle_cad_sheet.html        : Standalone Certified Engineering Drawing Sheet (Option A)
3. complete_unit_cad_sheet.html : Standalone Certified Engineering Drawing Sheet (Option B)
4. models/                      : Directory containing all optimized binary 3D GLB files
5. README_DEPLOYMENT_INSTRUCTIONS.txt : This deployment and hosting guide

--------------------------------------------------------------------------------
HOW TO HOST ON YOUR WEBSITE:
--------------------------------------------------------------------------------

METHOD A: UPLOAD TO YOUR COMPANY WEBSITE (e.g. palengineers.com)
1. Using cPanel File Manager, FTP (FileZilla), or SSH:
   - Navigate to your website's web root (e.g., public_html/ or htdocs/).
   - Create a new directory named '3d' or 'cad' (e.g. public_html/3d/).
   - Upload all files from this package into that directory:
     - index.html
     - bundle_cad_sheet.html
     - complete_unit_cad_sheet.html
     - models/ folder (with all .glb files inside)
2. Once uploaded, your 3D viewer is instantly live at:
   https://www.palengineers.com/3d/
   and the direct bundle sheet is live at:
   https://www.palengineers.com/3d/bundle_cad_sheet.html

METHOD B: EMBED INTO AN EXISTING WEBPAGE (WORDPRESS, HTML, WIX, ETC.)
To embed this interactive 3D viewer directly inside any existing page or blog post:
Paste the following HTML code into your page:

<div style="width: 100%; height: 750px; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 20px rgba(0,0,0,0.15);">
    <iframe src="https://www.palengineers.com/3d/index.html" 
            width="100%" 
            height="100%" 
            frameborder="0" 
            allow="fullscreen; xr-spatial-tracking" 
            loading="lazy">
    </iframe>
</div>

METHOD C: FREE 60-SECOND INSTANT GLOBAL HOSTING (CLOUDFLARE PAGES / VERCEL / NETLIFY)
If you want to host it online immediately without touching your company server:
1. Go to https://pages.cloudflare.com/ (or https://vercel.com/ or https://netlify.com/).
2. Drag and drop this 'PAL_ENGINEERS_3D_Web_Deploy' folder directly into the web uploader.
3. Your 3D viewer is live globally in 30 seconds with a free HTTPS URL!

METHOD D: GITHUB PAGES (100% FREE PERMANENT HOSTING)
1. Create a free GitHub repository (e.g. 'pal-engineers-3d').
2. Push or upload these files to the repository.
3. In Repository Settings -> Pages, select 'Deploy from branch: main / root'.
4. Your site is immediately live at https://<username>.github.io/pal-engineers-3d/

--------------------------------------------------------------------------------
TECHNICAL SPECIFICATIONS & PERFORMANCE:
--------------------------------------------------------------------------------
- Graphics Engine     : Google <model-viewer> v3.4.0 / Three.js WebGL
- Frame Rate          : 60 FPS hardware accelerated
- Controls            : 
  * Desktop Mouse     : Left Click + Drag = 360° Orbit | Scroll Wheel = Zoom | Right Click + Drag = Pan
  * Mobile / Touch    : 1-Finger Drag = Orbit | Pinch = Zoom | 2-Finger Drag = Pan
- CAD View Presets    : ISO (Isometric), TOP, FRONT, END, ⟳ Rotate, ⛶ Fit to Viewport
- Model Accuracy      : 100% dimensional match to OEM Plan P4429 Rev 3 and Datasheet 6114.
================================================================================
