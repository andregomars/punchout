# punchout
[![Build Status](https://travis-ci.org/andregomars/punchout.svg?branch=master)](https://travis-ci.org/andregomars/punchout)
> take care of clock in / out time of your daily work exactly

### Get PM punch out clock
```
$ punchout '09:00, 12:00, 13:00,'
['09:00','12:00','13:00','18:00']

$ punchout '09:53,12:12,12:38,'
['09:53','12:12','12:38','18:19']

$ punchout '09:00,12:00,13:00', 6
['09:00','12:00','13:00','16:00']

$ punchout '09:00,13:00,14:00,', 4
['09:00','13:00','','']
```

### Get AM punch in clock
```
$ punchout ',12:00,13:00,18:00'
['09:00','12:00','13:00','18:00']

$ punchout ',12:00,13:00,16:00', 6
['09:00','12:00','13:00','16:00']
```