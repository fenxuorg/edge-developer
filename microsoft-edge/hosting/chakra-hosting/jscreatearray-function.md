---
description: "Creates a Javascript array object."
title: "JsCreateArray Function | Microsoft Docs"
ms.custom: ""
ms.date: "01/18/2017"
ms.prod: microsoft-edge
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "reference"
f1_keywords: 
  - "jsrt/JsCreateArray"
helpviewer_keywords: 
  - "JsCreateArray function"
ms.assetid: a119949a-e427-4349-9d00-5ec20fb9319c
caps.latest.revision: 12
author: "erikadoyle"
ms.author: "edoyle"
manager: "jken"
---
# JsCreateArray Function
Creates a Javascript array object.  
  
## Syntax  
  
```cpp  
STDAPI_(JsErrorCode) JsCreateArray(  
   _In_ unsigned int length,  
   _Out_ JsValueRef *result  
);  
```  
  
#### Parameters  
 `length`  
 The initial length of the array.  
  
 `result`  
 The new array object.  
  
## Return Value  
 The code `JsNoError` if the operation succeeded, a failure code otherwise.  
  
## Remarks  
 Requires an active script context.  
  
## Requirements  
 **Header:** jsrt.h  
  
## See Also  
 [Reference (JavaScript Runtime)](../chakra-hosting/reference-javascript-runtime.md)