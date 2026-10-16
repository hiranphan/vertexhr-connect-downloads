# VertexHR Connect — Windows diagnostics pilot downloads

Official public download area for the **VertexHR Connect Windows 11 diagnostics-only pilot**. This repository holds public release links and checksums only. The VertexHR application source repository remains private.

**What it does:** On an authorized Windows 11 computer at a customer site, verifies the private-LAN adapter and the identity of a supported NEOCAL ND-AI06F terminal using bounded, read-only network checks.

**What it does not do:** It does not read face templates, fingerprints, punch or scan logs; send Attendance/Payroll data; open an inbound server; or change the terminal, router, or Production settings. A successful identity check is **not** proof of attendance ingestion.

**วิธีติดตั้ง:** ดาวน์โหลด ZIP จากหน้า Releases → แตกไฟล์หนึ่งครั้ง → ดับเบิลคลิก `Install-VertexHRConnect.cmd` (ไม่ใช่ `.ps1`) → ทำตามคำแนะนำ → ตรวจผลด้วย `Check-VertexHRConnect.cmd`. ต้องใช้ Windows PC ที่อยู่ในเครือข่าย LAN ภายในของไซต์เดียวกับ NEOCAL โดยไม่ต้องซื้อฮาร์ดแวร์เพิ่ม

**Caution:** This is an unsigned diagnostics **pilot**, not a generally certified Production attendance bridge. Native customer-site Windows 11 / NEOCAL acceptance testing remains pending. Coordinate installation with authorized site IT. Do not disable Windows Defender or SmartScreen to force installation; raise blocked-installation issues for review.

## Integrity and provenance

Windows build: private `hiranphan/vertex-hr` Draft PR #631, exact source revision `2d2a393e2bc92d993dcb355f125d9c8a7cb34976`, Windows GitHub Actions run `38535090398` (native Windows synthetic build/package PASS). SHA-256 checksum for the release ZIP is supplied as `SHA256SUMS.txt`.

No employee, customer, device serial, passwords, tokens, or physical-site data are published here.
