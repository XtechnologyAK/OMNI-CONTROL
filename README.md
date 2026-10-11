# Xtechnology OMNI CONTROL


**SCORPION EXPIREMENTAL 1 — Reliability 2** is an experimental Windows 10/11 x64 mouse utility with a native interface.


[Download Reliability 2](https://github.com/XtechnologyAK/OMNI-CONTROL/releases/tag/scorpion-expiremental-1-reliability-2) · [Website](https://omni-control.xtechnologies.workers.dev/) · [Report a test or bug](https://github.com/XtechnologyAK/OMNI-CONTROL/issues/new/choose)


Download the Windows-x64 ZIP, extract all files, close OMNI and run INSTALL.exe. The offline installer includes runtimes, keeps existing local profiles and creates shortcuts. CHECK FOR UPDATES finds new releases; downloading and installing remains manual.


| Mouse / adapter | Available controls | OMNI validation |
| --- | --- | --- |
| Attack Shark X11, 2.4 GHz | DPI, Hz, buttons, onboard custom macros, local profiles | Developer hardware tests |
| Attack Shark R1, 2.4 GHz | Experimental DPI (100–18,000), Hz (125/250/500/1000); no macros or live settings read-back | Receiver acknowledgement checks; physical testing needed |
| Razer Basilisk V3 / Viper V3 Pro | Experimental DPI / Hz | Physical testing needed |
| Logitech G502 HERO / G Pro Wireless / G Pro X Superlight, wired | Experimental DPI / Hz, stages, basic buttons; onboard mode required | Physical testing needed |
| Other matching OpenMouse drivers | Experimental DPI / Hz | Individual models unverified |


Generic OpenMouse macro/RGB controls are not connected yet. Recognition does not prove control compatibility. The upstream list has 663 entries, including requests/pending models, and 142 marked supported upstream; these are not hardware-tested OMNI counts. Unknown limits or ambiguous interfaces block writes. Driver values can be cached and are labelled unverified.


The temporary Node/HID helper runs only for requested operations. It uses additional RAM while active. The earlier ~2 MB Task Manager idle measurement applies to the previous native build on one PC; it is not a preview memory guarantee. Profiles stay local. No analytics, resident input listener or automatic uploads; SEND LOGS exports a filtered local report when no online inbox is configured; it does not upload automatically.


Automated validation: 211 app checks, 12 protocol tests, 14 Python backend tests and 14 installer checks, with actual mouse configuration disabled. Hardware testers are needed for exact model/connection behavior and persistence. The new binaries are unsigned and not yet freshly antivirus-scanned; see release notes for the earlier unresolved scanner discrepancy.


The derived preview is AGPL-3.0-or-later. **Complete corresponding source and licenses are attached as SOURCE.zip to the same release**, alongside the binary and SHA-256 checksums. Third-party notices remain included.


## Help test


Open a hardware-test issue with the exact model, connection, Windows version, build, DPI/Hz result and power-cycle persistence. Please share only public technical results; do not post personal logs, serials or full USB paths. Feedback is reviewed to distinguish recognition from working configuration.



## Reliability 2 fixes

The polling test matches the same Windows input instance across HID and mouse interface GUIDs, while excluding other devices. Experimental adapters use the same DPI slider and manual input. DPI and Hz capabilities are independent, and unsaved drafts survive transient reads and reconnects for the same device. R1 SAVE waits for receiver acknowledgements; physical behavior and persistence still need testing. Helper operations are bounded, corrupt local configuration is recovered without device writes, and failed installations restore previous managed files.
