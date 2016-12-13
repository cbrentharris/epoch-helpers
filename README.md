Epoch Helpers
======

A command line utility for helping with comparing the number of days or months since epoch and other dates.

Days Helpers
------


When you have a **date** and would like to convert it to the **number of days since epoch**:
```sh
epoch_helpers --days-since-epoch -y 2016 -m 1 -d 1
16801
epoch_helpers --days-since-epoch 2016-01-01
16801
epoch_helpers --days-since-epoch 2016/1/1 --date-format %Y/%m/%d
16801
```

When you have the **number of days since epoch** and would like to convert it to a **date**:
```sh
epoch_helpers --days-to-date 16801
2016-01-01 00:00:00
```

When you would like to know the **date** a certain **number of days ago**:
```sh
epoch_helpers --days-ago 7
2016-12-05 22:34:49.993501
```

When you would like to know the **number of days** since a specific **date**:
```sh
epoch_helpers --days-since 2016-01-01
346
epoch_helpers --days-since -y 2016 -m 1 -d 1
346
epoch_helpers --days-since 2016/1/1 --date-format %Y/%m/%d
346
```
