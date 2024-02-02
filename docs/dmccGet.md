## dmccGet
This function allows you to access Paramter from the Dataman

```
var roi = dmccGet("DECODER.ROI");
```

you can access the reponse with the `.response` in this case `roi.response` will hold the value.

```
	var roi = dmccGet("DECODER.ROI");
	console.log(roi);
    //will log "1320 1720 316 664"
```
