# bmex

lets you download both quotes (best bid/ask) as well as trades for all symbols and indices (including delisted ones) + sorts them out by creating the following structure:

Example: `python bmex.py --symbols XBTUSD ETHUSD --channels quotes trades --begin 2018-10-30 --end 2019-11-01`

```
Current_Directory # where you run the code
  └──BITMEX/
      ├── ETHUSD
      │   ├── quotes
      │   │   └── 2018
      │   │       ├── 10
      │   │       │   ├── 2018-10-30.csv
      │   │       │   └── 2018-10-31.csv
      │   │       └── 11
      │   │           └── 2018-11-01.csv
      │   └── trades
      │       └── 2018
      │           ├── 10
      │           │   ├── 2018-10-30.csv
      │           │   └── 2018-10-31.csv
      │           └── 11
      │               └── 2018-11-01.csv
      └── XBTUSD
          ├── quotes
          │   └── 2018
          │       ├── 10
          │       │   ├── 2018-10-30.csv
          │       │   └── 2018-10-31.csv
          │       └── 11
          │           └── 2018-11-01.csv
          └── trades
              └── 2018
                  ├── 10
                  │   ├── 2018-10-30.csv
                  │   └── 2018-10-31.csv
                  └── 11
                      └── 2018-11-01.csv
```
