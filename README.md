Epoch Helpers
======

A command line utility for helping with comparing the number of days or months since epoch and other dates.

Installation
------

```shell
pip install Epoch-Helpers
```

Or alternatively

```shell
git clone git@github.com:cbrentharris/epoch-helpers.git && cd epoch-helpers && python setup.py install
```

Days Helpers
------


When you have a **date** and would like to convert it to the **number of days since epoch**:
```shell
epoch_helpers --days-since-epoch -y 2016 -m 1 -d 1
16801
epoch_helpers --days-since-epoch 2016-01-01
16801
epoch_helpers --days-since-epoch 2016/1/1 --date-format %Y/%m/%d
16801
```

When you have the **number of days since epoch** and would like to convert it to a **date**:
```shell
epoch_helpers --days-to-date 16801
2016-01-01 00:00:00
```

When you would like to know the **date** a certain **number of days ago**:
```shell
epoch_helpers --days-ago 7
2016-12-05 22:34:49.993501
```

When you would like to know the **number of days** since a specific **date**:
```shell
epoch_helpers --days-since 2016-01-01
346
epoch_helpers --days-since -y 2016 -m 1 -d 1
346
epoch_helpers --days-since 2016/1/1 --date-format %Y/%m/%d
346
```

Months Helpers
------

When you have a **date** and would like to conver it to the **number of months since epoch**:
```shell
epoch_helpers --months-since-epoch -y 2016 -m 1 -d 1
552
epoch_helpers --months-since-epoch 2016-01-01
552
epoch_helpers --months-since-epoch 2016/1/1 --date-format %Y/%m/%d
552
```

When you have the **number of months since epoch** and would like to convert it to a **date**:
```shell
epoch_helpers --months-to-date 552
2016-01-01 00:00:00
```

When you would like to know the **date** a certain **number of months ago**:
```shell
epoch_helpers --months-ago 7
2016-05-13 07:55:29.005747
```

When you would liek to know the **number of months** since a specific **date**:
```shell
epoch_helpers --months-since 2014-05-22
31
epoch_helpers --months-since -y 2014 -m 5 -d 22
31
epoch_helpers --months-since 5/22/2014 --date-format %m/%d/%Y
31
```
