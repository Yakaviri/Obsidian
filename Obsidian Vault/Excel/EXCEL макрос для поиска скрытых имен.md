
Sub UnhideAllSheets()
    For Each ws In ThisWorkbook.Names
        If ws.Visible <> xlSheetVisible Then
            ws.Visible = xlSheetVisible
        End If
    Next ws
    MsgBox "ГОТОВО"
End Sub
