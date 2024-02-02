# Howto's

#### Custom FileName from PLC
i use a trick in order to transfer the filename from the PLC. I abuse the matchstring function from the camera and scripting. If the FileName is not equal to the Code disable the code match it still works. I always do the comparison in the PLC never in the camera so this is a great option to archive the custom file name.

You have to transfer the matchstring from the PLC to the Reader via bus.



`decodeResults[0].validation.matchString` you cannot use this since it will be empty on a no read and we still want to capture no reads to maybe toubleshoot the image.

Here is an Example on the Javascript for the `function onGenerateFTPFilename(decodeResults, readerProperties, output)`
which creates the File Name like `ABC_48_NG_2023-11-29_17582`

```
function onGenerateFTPFilename(decodeResults, readerProperties, output)
{
	//var test = decodeResults[0].validation.matchString;
	const matchString = dmccGet("DVALID.MATCH-STRING");
	const trigger_index = readerProperties.trigger.index;
	
	//creationTime - 2023-11-29_175515
	const date = new Date(readerProperties.trigger.executionDate);
	const creationTime = date.getFullYear() + "-" + (date.getMonth()+1) + "-" + date.getDate()+ "_" + date.getHours() + date.getMinutes() + +date.getSeconds();
	
	var result = "";
	if(decodeResults[0].decoded){
		result="OK"	
	}else{
		result="NG"	
	}
	
	var ftp_filename = matchString.response + "_"; // String transfered from PLC
	ftp_filename += readerProperties.trigger.index + "_"; // Trigger Index
	ftp_filename += result + "_"; // Trigger Index
	ftp_filename += creationTime; // Trigger Index
	
	return ftp_filename;
}
```
