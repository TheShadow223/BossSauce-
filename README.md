# BossSauce-
Public Class Form1
    Private Sub btnBirthdates_Click(sender As Object, e As EventArgs) Handles btnBirthdates.Click
        Dim namesArr(3) As String
        Dim datesArr(3) As String

        For i As Integer = 0 To 3
            namesArr(i) = InputBox("Enter the name", "Names")
            datesArr(i) = InputBox("Enter the Birthdate", "Dates")
            Me.lstDisplay.Items.Add(namesArr(i) & " " & datesArr(i))
        Next
    End Sub

    Private Sub AboutToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles AboutToolStripMenuItem.Click
        About.Show()
    End Sub

    Private Sub ExitToolStripMenuItem_Click(sender As Object, e As EventArgs) Handles ExitToolStripMenuItem.Click
        Application.Exit()
    End Sub
End Class
