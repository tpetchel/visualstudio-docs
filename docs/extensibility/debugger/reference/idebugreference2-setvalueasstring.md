---
description: "Sets the value of a reference from a string."
title: IDebugReference2::SetValueAsString | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugReference2::SetValueAsString
helpviewer_keywords:
- IDebugReference2::SetValueAsString
ms.assetid: 9a508ced-fd54-44f5-bb42-ec15c80384d7
author: maiak
ms.author: maiak
manager: jmartens
ms.technology: vs-ide-debug
ms.workload:
- vssdk
dev_langs:
- CPP
- CSharp
---
# IDebugReference2::SetValueAsString

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Sets the value of a reference from a string. Reserved for future use.

## Syntax

### [C#](#tab/csharp)
```csharp
int SetValueAsString ( 
   string pszValue,
   uint   dwRadix,
   uint   dwTimeout
);
```
### [C++](#tab/cpp)
```cpp
HRESULT SetValueAsString ( 
   LPCOLESTR pszValue,
   DWORD     dwRadix,
   DWORD     dwTimeout
);
```
---

## Parameters
`pszValue`\
[in] The value as a string.

`dwRadix`\
[in] The radix to be used in formatting any numerical information.

`dwTimeout`\
[in] Maximum time, in milliseconds, to wait before returning from this method. Use `INFINITE` to wait indefinitely.

## Return Value
 Always returns `E_NOTIMPL`.

## See also
- [IDebugReference2](../../../extensibility/debugger/reference/idebugreference2.md)
