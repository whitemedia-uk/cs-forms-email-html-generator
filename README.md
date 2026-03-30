<h1>CS Form Email Builder</h1>

<p>A standalone browser-based tool for generating professional HTML email notification templates for <a href="https://theme.co/">Cornerstone Forms (Themeco)</a>, using Cornerstone's <code>{{dc:form:data key=""}}</code> dynamic content syntax.</p>

<p>Built by <a href="https://www.whitemedia.uk/">Christopher White — White Media</a><br>
Built with assistance from <a href="https://www.anthropic.com/">Claude</a> (Anthropic)</p>

<hr>

<h2>What it does</h2>

<p>Cornerstone Form email notifications require hand-coded HTML tables with inline styles and dynamic content tags — a repetitive and error-prone process. This tool provides a visual interface for building those templates without writing any code.</p>

<p>You define your branding, build sections, assign fields, and click <strong>Generate HTML</strong> to produce a complete, production-ready email template ready to paste directly into the Cornerstone Form email action body.</p>

<hr>

<h2>Features</h2>

<ul>
  <li><strong>Visual section and field builder</strong> — create sections, add fields, drag to reorder and reassign</li>
  <li><strong>All field types supported</strong> — plain text, email link, tel link, URL link, address block, message block (pre-wrap)</li>
  <li><strong>Enquiry Details section</strong> — optional page-source field block, managed as a removable section</li>
  <li><strong>Branding controls</strong> — background colour, header title colour (white/black), logo, footer site name and URL</li>
  <li><strong>Branded footer</strong> — footer automatically matches the header background and title colour</li>
  <li><strong>Live code output</strong> — generated HTML displayed in a dark code panel with syntax-correct formatting</li>
  <li><strong>Preview tab</strong> — rendered preview of the finished email</li>
  <li><strong>Copy to clipboard</strong> — one click to copy the HTML</li>
  <li><strong>Download</strong> — saves the template as a named <code>.html</code> file</li>
  <li><strong>Preset system</strong> — save and reload complete configurations (branding + sections + fields) using browser <code>localStorage</code></li>
  <li><strong>Responsive layout</strong> — adapts from three columns on wide screens down to a single column on mobile</li>
  <li><strong>No dependencies</strong> — pure HTML, CSS, and JavaScript; no frameworks, no build step, no internet connection required</li>
</ul>

<hr>

<h2>Usage</h2>

<h3>Option 1 — Local file (recommended)</h3>
<ol>
  <li>Download <code>cs-email-builder.html</code></li>
  <li>Open it in any modern browser (Chrome, Edge, Firefox)</li>
  <li>No installation, no login, no internet connection required</li>
</ol>

<h3>Option 2 — Host on your own server</h3>
<p>Upload the single <code>.html</code> file to any web server. No server-side processing is needed.</p>

<h3>Option 3 — Embed in a Cornerstone page</h3>
<p>Place the contents inside a <strong>Raw Content</strong> element on a full-width, minimal-template Cornerstone page. Note that some browsers may restrict clipboard access inside iframes — hosting as a standalone file is more reliable.</p>

<hr>

<h2>Workflow</h2>

<ol>
  <li><strong>Branding (left column)</strong> — fill in your email title, background colour, header text colour, logo URL, and footer details</li>
  <li><strong>Sections (middle column)</strong> — the default layout includes an Enquiry Details section, a Contact Details section, and a Message section. Rename, reorder, or remove as needed</li>
  <li><strong>Fields</strong> — click <strong>+ Add field</strong> to add fields, specifying the Cornerstone field key, a display label, and the field type. Drag fields between sections to organise them</li>
  <li><strong>Generate</strong> — click <strong>Generate HTML</strong> in the top bar to produce the template</li>
  <li><strong>Copy or download</strong> — use <strong>Copy HTML</strong> to paste directly into Cornerstone, or <strong>Download .html</strong> to save a copy</li>
</ol>

<hr>

<h2>Field types</h2>

<table>
  <thead>
    <tr>
      <th>Type</th>
      <th>Output</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Plain text</td><td>Bold dark value cell</td></tr>
    <tr><td>Email link</td><td><code>mailto:</code> anchor in blue</td></tr>
    <tr><td>Tel link</td><td><code>tel:</code> anchor in blue</td></tr>
    <tr><td>URL link</td><td>Standard anchor in blue</td></tr>
    <tr><td>Address block</td><td>Single cell, suitable for a full address line</td></tr>
    <tr><td>Message block</td><td>Full-width pre-wrap paragraph for message text</td></tr>
  </tbody>
</table>

<hr>

<h2>Presets</h2>

<p>Presets save your complete configuration — branding, sections, and fields — to the browser's <code>localStorage</code>. They persist between sessions on the same browser and machine. Preset data is stored only in your browser and does not travel with the downloaded HTML file.</p>

<hr>

<h2>Dynamic content tag format</h2>

<p>All field values are output using Cornerstone's standard dynamic content syntax:</p>

<pre><code>{{dc:form:data key="your_field_key"}}</code></pre>

<p>Ensure your field keys exactly match the <strong>Name</strong> values set on your Cornerstone Form input elements.</p>

<hr>

<h2>Compatibility</h2>

<p>Tested in Chrome, Edge, and Firefox. Requires a modern browser with JavaScript enabled. The generated HTML is compatible with all major email clients that support inline-styled HTML tables (Gmail, Outlook, Apple Mail, etc.).</p>

<hr>

<h2>Licence</h2>

<p>MIT Licence — Copyright (c) 2026 Christopher White, White Media</p>

<p>Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:</p>

<p>The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.</p>

<p>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</p>
