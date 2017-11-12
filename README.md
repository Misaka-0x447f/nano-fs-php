# nanoFileOp
A portable file operator for light work and/or original php

Exported from [projectNanopoolMonitor/htmlMonitor](https://github.com/projectNanopoolMonitor/htmlMonitor)
# Requirement
php 5.6 or above
# Deployment
cp fileOp.php to your project

require("fileOp.php")
# Example
$fileOpt = new fileOp();

$fileOpt->fileSelect("example.file")

$fileOpt->fileCreate();
# Usage
`fileOp::fileSelect($fileName)`

You must select a file before do anything else.

`fileOp::fileRead()`

Read selected file and return it back.

`fileOp::jsonFileRead([$targetName])`

Read selected file in json format and return it back.

You could able to specify which property to read by using $targetName.

`fileOp::fileOverwrite($content)`

Remove selected file, then write a string to file.

`fileOp::jsonFileOverwrite($contentArray)`

Remove selected file, then write an php array to json file.

`fileOp::jsonFileWrite($name, $value)`

Write a property and its content to a json file.

`fileOp::jsonFileHasOwnProperty($key)`

Verify that a json file has owned property.

`fileOp::fileEmpty()`

Test if a file is empty.

`fileOp::fileExist()`

Test if a file is exist.

`fileOp::fileCreate()`

Create file with specified file name in 'SelectFile'

`fileOp::fileUnlink()`

Remove selected file.

`fileOp::fileLockRO()`

Make selected file read only with flock() //advisory file locking

`fileOp::fileLocked()`

Check if specified file locked by php

`fileOp::getFileLines()`

Return lines of file.

`fileOp::getFileContentByLineNumber($lineNumber)`

Get file content by line number.

$lineNumber is 1-based.