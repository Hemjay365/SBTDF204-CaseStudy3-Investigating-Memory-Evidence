# SBT-DF204 Case Study 3: Investigating Suspected Illegal File Transfer From Memory Evidence

**Student:** Mary-Joy Adewole | **Reg. no.:** 2025/FWSD/11468 | **Institution:** International Cybersecurity and Digital Forensics Academy (ICDFA)
**Report dated:** 19 October 2026 | **Tools:** Kali Linux 2026.2 (VMware), Volatility Foundation Volatility Framework 2.6.1 (`python2 vol.py`)

## Contents

| Path | What it is |
|---|---|
| `SBTDF204_CaseStudy3_2025-FWSD-11468.pdf` / `.docx` | The full report (case reference, conclusion and confidence, acquisition, method and profile, findings for Questions 1-8, UTC timeline, attribution and limitations, appendices) |
| `screenshots/` | The 27 labelled figures used in the report, cropped to the terminal window (`Figure_NN_name.png`, numbered as in the report) |
| `evidence_records/` | Every saved output, one file per plugin and profile, as real text (and one HTML) files, plus `evidence_manifest_sha256.txt` |

## Evidence image (not included)

- File: `memdumpWin7.mem`, 1,073,676,288 bytes
- SHA-256: `500bc1ba8b5ffa8053b6213d7e7aae0c84c18cce541dc53a55887e6e5099495e`
- MD5: `ac7eaa46a7006d5eb13cda13ee0b9bc9`
- Copied 2026-10-18 17:36:42 UTC; original and working copy read-only; hashes matched.
- The memory image is **not** in this package (the brief does not authorise uploading it).

## Profile and image time

Selected profile `Win7SP1x86_23418` (Windows 7 SP1, 32-bit PAE; the scenario text says Windows 10, the image does not). Image time 2019-01-06 15:09:06 UTC (local -0800). All times in the report are UTC as printed by Volatility.

## Evidence IDs

E01 acquisition | E02 imageinfo | E03 kdbgscan | E04 pslist | E05 psscan | E06 netscan | E07 cmdline | E08 cmdscan | E09 consoles | E10 hivelist | E11 getsids | E12 MountedDevices | E13 MountPoints2 | E14 USBSTOR | E15 DeviceClasses | E16 Select | E17 shellbags | E18 filescan | E19 strings (supplementary) | E20 hash manifest. The full log is Appendix D of the report.

## Verify the records

```
cd evidence_records
sha256sum -c evidence_manifest_sha256.txt
```

## Safety statement

Offline examination. No IP address, host, account, service or person named in the output was contacted. No recovered file was executed. No password or hash-cracking step was used. Work done individually.
