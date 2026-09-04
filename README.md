# NPOIHelper

A .NET Framework class library of NPOI extension methods that simplify creating and writing Excel spreadsheets. Working with NPOI directly takes several steps per cell; NPOIHelper wraps that into overloaded SetCellValue calls.

**Source last updated:** 2021-04-05
**Initiated:** 2021-04-09 · **Framework:** .NET Framework 4.8

---

## Overview

Working with NPOI directly requires several steps to write a single cell value. `NPOIHelper` wraps this into a single overloaded `SetCellValue` call.

---

## API

All methods are extension methods on `NPOI.SS.UserModel.ISheet`.

```csharp
sheet.SetCellValue(0, 0, "Name");        // string
sheet.SetCellValue(1, 0, 42);            // int
sheet.SetCellValue(2, 0, 98.5);          // double
sheet.SetCellValue(3, 0, true);          // bool
sheet.SetCellValue(4, 0, DateTime.Now);  // DateTime

IRow row = sheet.AddRow(rowIndex);       // get or create row
```

---

## Dependencies

| Package | Version |
|---------|---------|
| NPOI | 2.5.2 |

---

> This library depends on [NPOI](https://github.com/nissl-lab/npoi) (Apache 2.0). See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

## Requirements

- Visual Studio 2017 or later, .NET Framework 4.8

