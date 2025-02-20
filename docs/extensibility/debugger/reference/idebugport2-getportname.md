---
description: "Gets the port name."
title: IDebugPort2::GetPortName | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugPort2::GetPortName
helpviewer_keywords:
- IDebugPort2::GetPortName
ms.assetid: 4478b3d5-aa30-4105-8d05-e3bae2f8917a
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
# IDebugPort2::GetPortName

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Gets the port name.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetPortName( 
   out string pbstrName
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetPortName( 
   BSTR* pbstrName
);
```
---

## Parameters
`pbstrName`\
[out] Returns the name of the port.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## See also
- [IDebugPort2](../../../extensibility/debugger/reference/idebugport2.md)
