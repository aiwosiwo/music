## full path of N/A
```
^.*\.(N/A|NA)[a-ZA-Z0-9\-\_]*$
N/A
```

## amount
```
^([\t\s]*)("[a-zA-Z0-9]+Amount")\s*:\s*(".*")(,?)$
$1$2 : {\n$1\t"amount" : $3,\n$1\t"currencyCode" : "HKD"\n$1}$4
```

## balance
```
^([\t\s]*)("[a-zA-Z0-9]+Balance")\s*:\s*(".*")(,?)$
$1$2 : {\n$1\t"amount" : $3,\n$1\t"currencyCode" : "HKD"\n$1}$4
```

## sapi amount
```
^([\t\s]*)(".*")(,?)$
$1$2,\n$1"N/A_currencyCode_1" : ""$3
```