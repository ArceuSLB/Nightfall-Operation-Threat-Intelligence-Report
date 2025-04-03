📄 Static Analysis Report (analysis/static_analysis.md)

📁 File Information

Filename: Entropy.exe

Size: 77 MB

Type: PE32 executable (GUI) for MS Windows (Nullsoft Installer)

Entropy (estimated): High — presence of large .ndata section and PE compression expected

Timestamp: March 6, 21:57 (from file system)

🔐 Hashes

MD5: 5e3279d3242e453a5ab2dd342427517c

SHA-1: ac077192f23249601c2a389c7df4c6d7665f3d64

SHA-256: 40d276bfC90c67f621bc25acfdec93b3943842b2f2b5446a8fe370065c1d9402

🧩 PE Sections

Name

Size

Perm

Description

.text

0x6800

r-x

Main code

.rdata

0x1600

r--

Strings and API references

.data

0x7100

rw-

Writable global data

.ndata

0x124000

rw-

⚠️ Suspiciously large — likely payload or encrypted content

.rsrc

0x5c00

r--

Resources, possibly embedded files

🧠 Suspicious Strings

LoadLibraryExW

GetModuleHandleW

FindFirstFileW, FindNextFileW, FindClose

DeleteFileW

WritePrivateProfileStringW, GetPrivateProfileStringW

GlobalAlloc, GlobalFree, FreeLibrary

🛑 Behavior Indicators

Presence of file manipulation APIs

Memory allocation and module loading calls suggest runtime injection

Potential for dynamic unpacking or embedded second-stage payload

🧠 Notes

.ndata section is unusually large and may contain the actual payload

Further dynamic analysis is required to confirm execution behavior and C2 connections
