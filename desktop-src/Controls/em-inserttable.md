---
title: EM\_INSERTTABLE message
description: Inserts one or more identical table rows with empty cells.
ms.assetid: '7F9B2F28-1035-44AA-9DF6-57BC62886A4E'
keywords: ["EM_INSERTTABLE message Windows Controls"]
topic_type:
- apiref
api_name:
- EM_INSERTTABLE
api_location:
- Richedit.h
api_type:
- HeaderDef
---

# EM\_INSERTTABLE message

Inserts one or more identical table rows with empty cells.


```C++
#define EM_INSERTTABLE       (WM_USER + 232)
```



## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

A pointer to a [**TABLEROWPARMS**](tablerowparms.md) structure.

</dd> <dt>

*lParam* 
</dt> <dd>

A pointer to a [**TABLECELLPARMS**](tablecellparms.md) structure.

</dd> </dl>

## Return value

Returns S\_OK if the table is inserted, or an error code if not.

## Remarks

If the **cpStartRow** member of the [**TABLEROWPARMS**](tablerowparms.md) is �1, this message deletes the selected text (if any), and then inserts empty table rows with the row and cell parameters given by *wParam* and *lParam*. It leaves the selection pointing to the start of the first cell in the first row. The client can then populate the table cells by pointing the selection (or an [**ITextRange**](itextrange.md)) to the various cell end marks and inserting and formatting the desired text. Such text can include nested table rows. Alternatively, if the **cpStartRow** member of the **TABLEROWPARMS** is 0 or greater, table rows are inserted at the character position given by **cpStartRow**. This only changes the current selection if the table is inserted inside the selected text.

A Microsoft Rich Edit table consists of a sequence of table rows which, in turn, consist of sequences of paragraphs. A table row starts with the special two-character delimiter paragraph U+FFF9 U+000D and ends with the two-character delimiter paragraph U+FFFB U+000D. Each cell is terminated by the cell mark U+0007, which is treated as a hard end-of-paragraph mark just as U+000D (CR) is. The table row and cell parameters are treated as special paragraph formatting of the table-row delimiters. The formatting contains the information in the [**TABLEROWPARMS**](tablerowparms.md) structure. The cell parameters given by the [**TABLECELLPARMS**](tablecellparms.md) structure are stored in an expanded version of the tabs array. This format allows tables to be nested within other tables, up to fifteen levels deep. For more information, see [RichEdit�s Nested Table Facility](http://go.microsoft.com/fwlink/p/?linkid=239678).

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�8 \[desktop apps only\]<br/>                                            |
| Minimum supported server<br/> | Windows Server�2012 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Richedit.h</dt> </dl> |



## See also

<dl> <dt>

[**EM\_INSERTIMAGE**](em-insertimage.md)
</dt> </dl>

�

�




