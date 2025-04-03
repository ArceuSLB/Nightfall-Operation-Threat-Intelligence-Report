## 📄 Static Analysis Report (`analysis/static_analysis.md`)
### 📁 File Information
| Field        | Value                                               |
|--------------|-----------------------------------------------------|
| Filename     | Entropy.exe                                         |
| Size         | 77 MB                                               |
| Type         | PE32 executable (GUI) for MS Windows (Nullsoft)    |
| Entropy      | High — large `.ndata` section, likely compression  |
| Timestamp    | March 6, 21:57 (from file system)                   |

### 🔐 Hashes
| Algorithm | Value                                                   |
|-----------|---------------------------------------------------------|
| MD5       | 5e3279d3242e453a5ab2dd342427517c                        |
| SHA-1     | ac077192f23249601c2a389c7df4c6d7665f3d64               |
| SHA-256   | 40d276bfC90c67f621bc25acfdec93b3943842b2f2b5446a8fe370065c1d9402 |

### 🧰 PE Sections
| Name     | Size     | Perm | Description                                        |
|----------|----------|------|----------------------------------------------------|
| `.text`  | 0x6800   | r-x  | Main code                                          |
| `.rdata` | 0x1600   | r--  | Strings and API references                         |
| `.data`  | 0x7100   | rw-  | Writable global data                               |
| `.ndata` | 0x124000 | rw-  | ⚠️ Suspiciously large, likely encrypted payload |
| `.rsrc`  | 0x5c00   | r--  | Resources (potential embedded files)               |

### 🧐 Suspicious Strings
- `LoadLibraryExW`
- `GetModuleHandleW`
- `FindFirstFileW`, `FindNextFileW`, `FindClose`
- `DeleteFileW`
- `WritePrivateProfileStringW`, `GetPrivateProfileStringW`
- `GlobalAlloc`, `GlobalFree`, `FreeLibrary`

### ⛔️ Behavior Indicators
- API calls for file manipulation
- Memory allocation and module injection functions
- Indicators of runtime unpacking or multi-stage payload

### 🧠 Notes
- The `.ndata` section’s size and presence of loading APIs suggest hidden or encrypted behavior
- Further dynamic inspection is required to validate behavior and identify C2 infrastructure

---

## 🔗 License
This repository is intended for educational and research purposes only.


