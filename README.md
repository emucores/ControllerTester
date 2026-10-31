<p align="center">
  <a href="https://controllertester.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://controllertester.com/wp-content/uploads/2026/10/controllertester-logo-dark-1000.webp">
      <source media="(prefers-color-scheme: light)" srcset="https://controllertester.com/wp-content/uploads/2026/10/controllertester-logo-light-1000.webp">
      <img src="https://controllertester.com/wp-content/uploads/2026/10/controllertester-logo-light-1000.webp" alt="ControllerTester" width="440">
    </picture>
  </a>
</p>

<h1 align="center">ControllerTester</h1>

<p align="center">
  <strong>Every Input, Understood.</strong><br>
  Test your controller, understand its readings, and get back to playing.
</p>

<p align="center">
  <a href="https://controllertester.com"><strong>Open ControllerTester</strong></a>
  ·
  <a href="https://controllertester.com/controllers/">Controller Directory</a>
  ·
  <a href="https://controllertester.com/controller-guides/">Guides</a>
  ·
  <a href="https://github.com/emucores">EmuCores</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/WordPress-Plugin-21759B?logo=wordpress&logoColor=white" alt="WordPress Plugin">
  <img src="https://img.shields.io/badge/JavaScript-Gamepad_API-F7DF1E?logo=javascript&logoColor=black" alt="JavaScript Gamepad API">
  <img src="https://img.shields.io/badge/License-GPL--2.0--or--later-blue" alt="GPL-2.0-or-later">
</p>

---

## About

**ControllerTester** is a browser-based controller and gamepad testing tool developed by [EmuCores](https://github.com/emucores).

Connect a controller, press a button, and see the inputs your browser receives. Check buttons, triggers, stick movement, resting offsets, range, and vibration from one interface.

The project combines an interactive tester with controller setup guides, model comparisons, troubleshooting resources, and a WordPress plugin that powers the website.

**No download or account is required to use the online tester.**

## Features

| Feature | What You Can Do |
| --- | --- |
| Live Input Testing | Watch button presses, trigger values, and stick movement as they reach the browser. |
| Controller Visuals | View transparent controller artwork or switch to an interactive input diagram. |
| Stick Drift Checks | Run a timed resting-stick test with mean, peak, and percentile offset readings. |
| Range And Circularity | Trace stick movement and run a guided sweep to inspect directional coverage and output shape. |
| Return-To-Centre Checks | Observe where sticks settle after releasing them from different directions. |
| Trigger Testing | Inspect analog travel, observed endpoints, and recent value traces. |
| Deadzone Preview | Visualize a deadzone around the stick centre without changing controller settings. |
| Vibration Testing | Request rumble with adjustable strength and duration where supported. |
| Guided Checkups | Follow a structured sequence covering buttons, triggers, sticks, and results. |
| Multiple Controllers | Switch between gamepads exposed by the browser. |
| Saved Snapshots | Keep named test snapshots locally with connection details, profiles, and notes. |
| Reports And Comparisons | Export JSON or CSV, import reports, print results, and compare saved observations. |
| Controller Directory | Explore model references, connection guidance, configuration notes, and testing tips. |
| Model Comparisons | Compare documented controller features and setup requirements side by side. |

The interface includes light and dark themes, responsive layouts, keyboard navigation, and selectable button naming.

## Get Started

1. Open [controllertester.com](https://controllertester.com).
2. Connect your controller using a supported USB, Bluetooth, or receiver connection.
3. Focus the page and press a controller button.
4. Select your device if more than one controller appears.
5. Move the sticks, squeeze the triggers, and press each button.
6. Run a guided checkup or save a report for future comparison.

If your controller does not appear, start with the [Controller Not Detected Guide](https://controllertester.com/controller-not-detected/).

## Controller Coverage

The directory includes references for:

- **PlayStation:** DualSense, DualSense Edge, DualShock 4, and DualShock 3.
- **Xbox:** Xbox Wireless Controller and Xbox Elite Wireless Controller Series 2.
- **Nintendo:** Switch Pro Controller.
- **Additional Brands:** 8BitDo, Flydigi, GameSir, GuliKit, HORI, Logitech, NACON, PowerA, Razer, SCUF, SteelSeries, Steam Controller, Thrustmaster, Turtle Beach, and Victrix / PDP.

Testing is not restricted to listed models. Other controllers can work when the browser exposes them through the Gamepad API.

Available inputs and vibration support depend on the controller, connection, operating system, browser, firmware, and remapping software. A directory listing provides setup guidance; it does not certify every feature or configuration.

## Understanding Your Results

ControllerTester shows **browser-observed input**.

- A resting offset can help investigate unwanted stick movement.
- Circularity describes the reported stick output shape.
- Extra paddles may repeat existing buttons instead of appearing independently.
- Remapping software can expose a virtual Xbox controller or change the readings.
- An unobserved button is untested, not automatically faulty.

The tester does not measure physical polling rate or end-to-end input latency, change hardware calibration, or test adaptive-trigger resistance.

Read the [Testing Methodology](https://controllertester.com/testing-methodology/) for measurement definitions.

## Privacy And Local Storage

Live controller input is processed in your browser.

- Saved snapshots use local browser storage.
- Reports are not uploaded automatically.
- JSON imports are validated locally.
- Exporting or sharing a report is your choice.
- The plugin itself does not install analytics or advertising trackers.

Website requests and contact-form submissions are separate from controller testing. See [Tester Data And Privacy](https://controllertester.com/tester-data-privacy/) for details.

## WordPress Plugin

**ControllerTester Suite** provides the tester, controller directory, comparisons, shared navigation, and editable starter pages.

### Requirements

- WordPress **6.4 or later**
- PHP **7.4 or later**
- HTTPS for the public website
- A browser that exposes controller input through the Gamepad API

### Installation

1. Obtain an installable ControllerTester Suite plugin ZIP.
2. In WordPress, open **Plugins → Add New Plugin → Upload Plugin**.
3. Upload the ZIP and activate **ControllerTester Suite**.
4. Open **ControllerTester** in the WordPress dashboard.
5. Select your preferred settings and choose **Create Missing Starter Pages**.
6. Review the generated pages, privacy information, contact settings, and SEO metadata.
7. Clear page caches and test with a connected controller.

Activation alone does not create pages, replace the theme, or change the homepage.

### Shortcodes

Embed tools using a WordPress Shortcode block or an Elementor Shortcode widget.

| Shortcode | Tool |
| --- | --- |
| `[ct_tester]` | Live Controller Tester |
| `[ct_tester mode="guided"]` | Guided Checkup |
| `[ct_tester mode="buttons"]` | Buttons And Triggers |
| `[ct_tester mode="drift"]` | Resting Stick Drift Test |
| `[ct_tester mode="range"]` | Range And Circularity Sweep |
| `[ct_tester mode="centering"]` | Return-To-Centre Checks |
| `[ct_tester mode="triggers"]` | Trigger Travel |
| `[ct_tester mode="deadzone"]` | Deadzone Preview |
| `[ct_tester mode="vibration"]` | Vibration Test |
| `[ct_compare]` | Saved Snapshot Comparison |
| `[ct_model_finder]` | Controller Directory |
| `[ct_model_compare]` | Controller Model Comparison |

You can also provide a starting controller reference:

```text
[ct_tester family="dualsense" model="dualsense-edge"]
```

Model selection controls the reference presentation; it does not change the browser's input mapping.

## Technical Overview

- **JavaScript** handles live Gamepad API readings, visualizations, diagnostics, and local reports.
- **PHP And WordPress** provide editable pages, shortcodes, settings, and content management.
- **HTML And CSS** provide the responsive interface and light/dark themes.
- **WebP Artwork** supplies transparent controller illustrations and responsive thumbnails.
- **Rank Math Integration** supplies starter SEO fields, with editable server-rendered page content.

Controller illustrations are visual references. They are not manufacturer photographs or proof of physical testing.

## Contributing

Contributions are welcome, including:

- Reproducible bug reports.
- Browser and controller compatibility observations.
- Corrections to model specifications and setup instructions.
- Accessibility and responsive-layout improvements.
- Improvements to documentation and troubleshooting guides.

When reporting a problem, include:

1. Controller model.
2. Operating system and browser version.
3. Connection type.
4. Relevant firmware, drivers, remappers, or controller profiles.
5. Steps to reproduce the issue.
6. Expected and observed behaviour.

Review exported reports before sharing them because they can include device information and personal notes.

## More From Our Partners

- [DS4Windows](https://ds4-windows.com/)
- [DualSenseX](https://dualsensex.com/)

## License

The plugin code is licensed under **GPL-2.0-or-later**.

Controller names, product names, and trademarks belong to their respective owners. Their inclusion does not imply endorsement or affiliation.

---

<p align="center">
  Developed by <a href="https://github.com/emucores"><strong>EmuCores</strong></a><br>
  <a href="https://controllertester.com">controllertester.com</a>
</p>
