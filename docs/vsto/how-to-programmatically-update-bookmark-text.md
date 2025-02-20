---
title: "How to: Programmatically update bookmark text"
description: Learn how you can use Visual Studio to programmatically insert text into a placeholder bookmark in a Microsoft Word document.
ms.date: "02/02/2017"
ms.topic: "how-to"
dev_langs:
  - "VB"
  - "CSharp"
helpviewer_keywords:
  - "bookmarks, updating text"
  - "text [Office development in Visual Studio], updating in bookmarks"
  - "Bookmark control, updating contents"
author: John-Hart
ms.author: johnhart
manager: jmartens
ms.technology: office-development
ms.workload:
  - "office"
---
# How to: Programmatically update bookmark text

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
  You can insert text into a placeholder bookmark in a Microsoft Office Word document so that you can retrieve the text at a later time, or to replace text in a bookmark. If you are developing a document-level customization, you can also update text in a <xref:Microsoft.Office.Tools.Word.Bookmark> control that is bound to data. For more information, see [Bind data to controls in Office solutions](../vsto/binding-data-to-controls-in-office-solutions.md).

 [!INCLUDE[appliesto_wdalldocapp](../vsto/includes/appliesto-wdalldocapp-md.md)]

 The bookmark object can be one of two types:

- A <xref:Microsoft.Office.Tools.Word.Bookmark> host control.

   <xref:Microsoft.Office.Tools.Word.Bookmark> controls extend native <xref:Microsoft.Office.Interop.Word.Bookmark> objects by enabling data binding and exposing events. For more information about host controls, see [Host items and host controls overview](../vsto/host-items-and-host-controls-overview.md).

- A native <xref:Microsoft.Office.Interop.Word.Bookmark> object.

   <xref:Microsoft.Office.Interop.Word.Bookmark> objects do not have events or data binding capabilities.

  When you assign text to a bookmark, the behavior differs between a <xref:Microsoft.Office.Interop.Word.Bookmark> and a <xref:Microsoft.Office.Tools.Word.Bookmark>. For more information, see [Bookmark control](../vsto/bookmark-control.md).

## Use host controls

### To update bookmark contents using a Bookmark control

1. Create a procedure that takes a `bookmark` argument for the name of the bookmark, and a `newText` argument for the string to assign to the <xref:Microsoft.Office.Tools.Word.Bookmark.Text%2A> property.

    > [!NOTE]
    > Assigning text to the <xref:Microsoft.Office.Tools.Word.Bookmark.Text%2A> or <xref:Microsoft.Office.Tools.Word.Bookmark.FormattedText%2A> property of a <xref:Microsoft.Office.Tools.Word.Bookmark> control does not cause the bookmark to be deleted.

     ### [C#](#tab/csharp)
     :::code language="csharp" source="../vsto/codesnippet/CSharp/Trin_VstcoreWordAutomationCS/ThisDocument.cs" id="Snippet63":::

     ### [VB](#tab/vb)
     :::code language="vb" source="../vsto/codesnippet/VisualBasic/Trin_VstcoreWordAutomationVB/ThisDocument.vb" id="Snippet63":::
     ---

2. Assign the *newText* string to the <xref:Microsoft.Office.Tools.Word.Bookmark.Text%2A> property of the <xref:Microsoft.Office.Tools.Word.Bookmark>.

     ### [C#](#tab/csharp)
     :::code language="csharp" source="../vsto/codesnippet/CSharp/Trin_VstcoreWordAutomationCS/ThisDocument.cs" id="Snippet64":::

     ### [VB](#tab/vb)
     :::code language="vb" source="../vsto/codesnippet/VisualBasic/Trin_VstcoreWordAutomationVB/ThisDocument.vb" id="Snippet64":::
     ---

## Use Word objects

### To update bookmark contents using a Word Bookmark object

1. Create a procedure that has a `bookmark` argument for the name of the <xref:Microsoft.Office.Interop.Word.Bookmark>, and a `newText` argument for the string to assign to the <xref:Microsoft.Office.Interop.Word.Range.Text%2A> property of the bookmark.

    > [!NOTE]
    > Assigning text to a native Word <xref:Microsoft.Office.Interop.Word.Bookmark> object causes the bookmark to be deleted.

     ### [C#](#tab/csharp)
     :::code language="csharp" source="../vsto/codesnippet/CSharp/Trin_VstcoreWordAutomationCS/ThisDocument.cs" id="Snippet65":::

     ### [VB](#tab/vb)
     :::code language="vb" source="../vsto/codesnippet/VisualBasic/Trin_VstcoreWordAutomationVB/ThisDocument.vb" id="Snippet65":::
     ---

2. Assign the *newText* string to the <xref:Microsoft.Office.Interop.Word.Range.Text%2A> property of the bookmark, which automatically deletes the bookmark. Then re-add the bookmark to the <xref:Microsoft.Office.Interop.Word.Bookmarks> collection.

     The following code example can be used in a document-level customization.

     ### [C#](#tab/csharp)
     :::code language="csharp" source="../vsto/codesnippet/CSharp/Trin_VstcoreWordAutomationCS/ThisDocument.cs" id="Snippet66":::

     ### [VB](#tab/vb)
     :::code language="vb" source="../vsto/codesnippet/VisualBasic/Trin_VstcoreWordAutomationVB/ThisDocument.vb" id="Snippet66":::
     ---

     The following code example can be used in a VSTO Add-in. This example uses the active document.

     ### [C#](#tab/csharp)
     :::code language="csharp" source="../vsto/codesnippet/CSharp/Trin_VstcoreWordAutomationAddIn/ThisAddIn.cs" id="Snippet66":::

     ### [VB](#tab/vb)
     :::code language="vb" source="../vsto/codesnippet/VisualBasic/Trin_VstcoreWordAutomationAddIn/ThisAddIn.vb" id="Snippet66":::
     ---

## See also
- [How to: Programmatically insert text into Word documents](../vsto/how-to-programmatically-insert-text-into-word-documents.md)
- [Word object model overview](../vsto/word-object-model-overview.md)
- [Bookmark control](../vsto/bookmark-control.md)
