## OnResults

onResult Event

```
function onResult (decodeResults, readerProperties, output){}
```

### decodeResults
```
[
    {
        "decoded": false,
        "content": "",
        "decodeTime": 11,
        "triggerTime": 36,
        "timeout": 2000,
        "readSetup": 0,
        "image": {
            "id": 20,
            "index": 0,
            "FoV": {
                "left": 0,
                "top": 0,
                "right": 2048,
                "bottom": 1536
            },
            "RoI": {
                "left": 1320,
                "top": 316,
                "right": 1720,
                "bottom": 664
            },
            "exposureTime": 81,
            "gain": "1.00",
            "autoExposure": true,
            "illEnabled": true,
            "illIntensity": 15,
            "extIllEnabled": false,
            "extIllIntensity": 15,
            "focusLength": 308,
            "focusPower": "2.27",
            "setupIndex": 0,
            "inputStates": [
                false,
                false,
                false,
                false
            ],
            "filterTime": 0,
            "creationTime": 1042811588,
            "creationTicks": 0,
            "creationDate": "2023-11-29T22:05:44.471Z",
            "ptpTimeStamp": {
                "s": 0,
                "ns": 0
            },
            "mirrorAngleA": "0.000",
            "mirrorAngleB": "0.000",
            "mirrorPathIndex": -1,
            "intIllWavelength": 65535,
            "intIllWavelengthMask": 0,
            "multicolorWavelength": [],
            "multicolorRatio": [],
            "multicolorName": []
        },
        "validation": {
            "state": 0,
            "method": 0,
            "gs1": {},
            "dodUid": {}
        },
        "metrics": {
            "symbolContrast": {
                "raw": -1,
                "grade": "NA"
            },
            "cellContrast": {
                "raw": -1,
                "grade": "NA"
            },
            "axialNonUniformity": {
                "raw": -1,
                "grade": "NA"
            },
            "printGrowth": {
                "raw": -1,
                "grade": "NA"
            },
            "UEC": {
                "raw": -1,
                "grade": "NA"
            },
            "modulation": {
                "raw": -1,
                "grade": "NA"
            },
            "fixedPatternDamage": {
                "raw": -1,
                "grade": "NA"
            },
            "gridNonUniformity": {
                "raw": -1,
                "grade": "NA"
            },
            "extremeReflectance": {
                "raw": -1,
                "grade": "NA"
            },
            "reflectMin": {
                "raw": -1,
                "grade": "NA"
            },
            "edgeContrastMin": {
                "raw": -1,
                "grade": "NA"
            },
            "singleScanInt": {
                "raw": -1,
                "grade": "NA"
            },
            "multiScanInt": {
                "raw": -1,
                "grade": "NA"
            },
            "signalToNoiseRatio": {
                "raw": -1,
                "grade": "NA"
            },
            "horizontalMarkGrowth": {
                "raw": -1,
                "grade": "NA"
            },
            "verticalMarkGrowth": {
                "raw": -1,
                "grade": "NA"
            },
            "dataMatrixCellWidth": {
                "raw": -1,
                "grade": "NA"
            },
            "dataMatrixCellHeight": {
                "raw": -1,
                "grade": "NA"
            },
            "horizontalMarkMisplacement": {
                "raw": -1,
                "grade": "NA"
            },
            "verticalMarkMisplacement": {
                "raw": -1,
                "grade": "NA"
            },
            "cellDefects": {
                "raw": -1,
                "grade": "NA"
            },
            "finderPatternDefects": {
                "raw": -1,
                "grade": "NA"
            },
            "overallGrade": {
                "raw": -1,
                "grade": "NA"
            },
            "edgeDetermination": {
                "raw": -1,
                "grade": "NA"
            },
            "defects": {
                "raw": -1,
                "grade": "NA"
            },
            "referenceDecode": {
                "raw": -1,
                "grade": "NA"
            },
            "decodability": {
                "raw": -1,
                "grade": "NA"
            },
            "contrastUniformity": {
                "raw": -1,
                "grade": "NA"
            },
            "reflectanceMargin": {
                "raw": -1,
                "grade": "NA"
            },
            "minPassGrade": {
                "raw": -1,
                "grade": "NA"
            }
        },
        "source": "FL2-OP30-DM374-9E6B82",
        "annotation": "",
        "label": "",
        "custom_svg": "",
        "trucheck": {},
        "barcodeAssignment": {
            "result": -1,
            "stats": {
                "parcel": -1
            }
        }
    }
]
```

### readerProperties
```
{
    "name": "FL2-OP30-DM374-9E6B82",
    "trigger": {
        "type": 0,
        "index": 24,
        "groupIndex": 24,
        "burstLength": 1,
        "interval": 200000,
        "delayType": 0,
        "startDelay": 0,
        "endDelay": 0,
        "creationTime": 1043134997,
        "creationTicks": 0,
        "endTime": 1043135019,
        "endTicks": 0,
        "creationDate": "2023-11-29T22:11:07.878Z",
        "executionDate": "2023-11-29T22:11:07.878Z",
        "validDimensions": false,
        "encoderDimsMatch": false
    },
    "stats": {
        "reads": 3,
        "noReads": 21,
        "triggers": 24,
        "bufferOverflows": 0,
        "triggerOverruns": 0,
        "itemCount": 0,
        "passedValidations": 0,
        "failedValidations": 0
    },
    "inputstr": "",
    "status3D": {
        "fieldCalibrated": false,
        "factoryCalibrated": false
    }
}
```

### output

```
{
    "content": "",
    "events": {
        "system": 2,
        "user1": false,
        "user2": false
    },
    "Serial": "",
    "Telnet": "",
    "Keyboard": "",
    "FTP": "",
    "NetworkClient": "",
    "IndustrialProtocols": "",
    "OLED": "",
    "SetupTool": ""
}
```