# Xtechnology OMNI CONTROL

**SCORPION EXPIREMENTAL 1 — OpenMouse preview** is an experimental Windows 10/11 x64 mouse utility with a native interface.

[Download the OpenMouse preview](https://github.com/XtechnologyAK/OMNI-CONTROL/releases/tag/scorpion-expiremental-1-openmouse-preview) · [Website](https://omni-control.xtechnologies.workers.dev/) · [Report a test or bug](https://github.com/XtechnologyAK/OMNI-CONTROL/issues/new/choose)

Download the Windows-x64 ZIP, extract all files, close OMNI and run INSTALL.exe. The offline installer includes runtimes, keeps existing local profiles and creates shortcuts. There is no automatic updater.

| Mouse / adapter | Available controls | OMNI validation |
| --- | --- | --- |
| Attack Shark X11, 2.4 GHz | DPI, Hz, buttons, onboard custom macros, local profiles | Developer hardware tests |
| Razer Basilisk V3 / Viper V3 Pro | Experimental DPI / Hz | Physical testing needed |
| Logitech G502 HERO / G Pro Wireless / G Pro X Superlight, wired | Experimental DPI / Hz, stages, basic buttons; onboard mode required | Physical testing needed |
| Other matching OpenMouse drivers | Experimental DPI / Hz | Individual models unverified |

Generic OpenMouse macro/RGB controls are not connected yet. Recognition does not prove control compatibility. The upstream list has 663 entries, including requests/pending models, and 142 marked supported upstream; these are not hardware-tested OMNI counts. Unknown limits or ambiguous interfaces block writes. Driver values can be cached and are labelled unverified.

The temporary Node/HID helper runs only for requested operations. It uses additional RAM while active. The earlier ~2 MB Task Manager idle measurement applies to the previous native build on one PC; it is not a preview memory guarantee. Profiles stay local. No analytics, resident input listener or automatic uploads; SEND LOGS is not connected to an online inbox.

Automated validation: 169 app checks, 8 protocol tests and 12 installer checks, with actual mouse configuration disabled. Hardware testers are needed for exact model/connection behavior and persistence. The new binaries are unsigned and not yet freshly antivirus-scanned; see release notes for the earlier unresolved scanner discrepancy.

The derived preview is AGPL-3.0-or-later. **Complete corresponding source and licenses are attached as SOURCE.zip to the same release**, alongside the binary and SHA-256 checksums. Third-party notices remain included.

## Help test

Open a hardware-test issue with the exact model, connection, Windows version, build, DPI/Hz result and power-cycle persistence. Please share only public technical results; do not post personal logs, serials or full USB paths. Feedback is reviewed to distinguish recognition from working configuration.
