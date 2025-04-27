

test
$filePath = "path/to/your/file.txt"
$newLine = "This is the new first line"

$existingContent = Get-Content $filePath
$newContent = $newLine + "`n" + ($existingContent -join "`n")

Set-Content $filePath $newContent
