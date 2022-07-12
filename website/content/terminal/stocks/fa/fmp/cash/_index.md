```
usage: cash [-l LIMIT] [-q] [-h] [--export {csv,json,xlsx}]
```

Prints a complete cash flow statement over time. This can be either quarterly or annually. [Source: Financial Modeling Prep]
```
optional arguments:
  -l LIMIT, --limit LIMIT
                        Limit of latest years/quarters. (default: 1)
  -q, --quarter         Quarter fundamental data flag. (default: False)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xlsx (default: )
```

Example (with ticker AAPL):
```
2022 Feb 16, 05:19 (✨) /stocks/fa/fmp/ $ cash -l 12
                                                                                                                              Ticker Cash Flow
┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┓
┃                                                ┃ 2010       ┃ 2011       ┃ 2012       ┃ 2013       ┃ 2014       ┃ 2015                ┃ 2016                ┃ 2017                ┃ 2018                ┃ 2019                ┃ 2020                ┃ 2021                ┃
┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━┩
│ Reported currency                              │ USD        │ USD        │ USD        │ USD        │ USD        │ USD                 │ USD                 │ USD                 │ USD                 │ USD                 │ USD                 │ USD                 │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Cik                                            │ 1.652 M    │ 1.652 M    │ 1.652 M    │ 1.652 M    │ 1.652 M    │ 1.652 M             │ 1.652 M             │ 1.652 M             │ 1.652 M             │ 1.652 M             │ 1.652 M             │ 1.652 M             │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Filling date                                   │ 2010-12-31 │ 2011-12-31 │ 2012-12-31 │ 2013-12-31 │ 2014-12-31 │ 2016-02-11          │ 2017-02-03          │ 2018-02-06          │ 2019-02-05          │ 2020-02-04          │ 2021-02-03          │ 2022-02-02          │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Accepted date                                  │ 2010-12-31 │ 2011-12-31 │ 2012-12-31 │ 2013-12-31 │ 2014-12-31 │ 2016-02-11 16:38:35 │ 2017-02-02 18:13:47 │ 2018-02-05 20:46:29 │ 2019-02-04 21:06:38 │ 2020-02-03 21:03:59 │ 2021-02-02 20:12:25 │ 2022-02-01 21:08:02 │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Calendar year                                  │ 2.010 K    │ 2.011 K    │ 2.012 K    │ 2.013 K    │ 2.014 K    │ 2.015 K             │ 2.016 K             │ 2.017 K             │ 2.018 K             │ 2.019 K             │ 2.020 K             │ 2.021 K             │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Period                                         │ FY         │ FY         │ FY         │ FY         │ FY         │ FY                  │ FY                  │ FY                  │ FY                  │ FY                  │ FY                  │ FY                  │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Net income                                     │ 8.505 B    │ 9.737 B    │ 10.737 B   │ 12.733 B   │ 14.136 B   │ 16.348 B            │ 19.478 B            │ 12.662 B            │ 30.736 B            │ 34.343 B            │ 40.269 B            │ 76.033 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Depreciation and amortization                  │ 1.396 B    │ 1.851 B    │ 2.962 B    │ 3.939 B    │ 4.979 B    │ 5.063 B             │ 6.144 B             │ 6.915 B             │ 9.035 B             │ 11.781 B            │ 13.697 B            │ 12.441 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Deferred income tax                            │ 9 M        │ 343 M      │ -266 M     │ -437 M     │ -104 M     │ -179 M              │ -38 M               │ 258 M               │ 778 M               │ 173 M               │ 1.390 B             │ 1.808 B             │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Stock based compensation                       │ 1.376 B    │ 1.974 B    │ 2.692 B    │ 3.343 B    │ 4.279 B    │ 5.203 B             │ 6.703 B             │ 7.679 B             │ 9.353 B             │ 10.794 B            │ 12.991 B            │ 15.376 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Change in working capital                      │ 5.146 B    │ 12.279 B   │ 2.272 B    │ 10.861 B   │ 4.899 B    │ 8.927 B             │ 17.848 B            │ 11.473 B            │ 931 M               │ 6.301 B             │ 10.105 B            │ -1.523 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Accounts receivables                           │ -1.129 B   │ -1.156 B   │ -787 M     │ -1.307 B   │ -1.641 B   │ -2.094 B            │ -2.578 B            │ -3.768 B            │ -2.169 B            │ -4.340 B            │ -6.524 B            │ -9.095 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Inventory                                      │ 0          │ 0          │ 301 M      │ -234 M     │ 0          │ 0                   │ 0                   │ 0                   │ 0                   │ 0                   │ 0                   │ 0                   │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Accounts payables                              │ 272 M      │ 101 M      │ -499 M     │ 605 M      │ 436 M      │ 203 M               │ 110 M               │ 731 M               │ 1.067 B             │ 428 M               │ 694 M               │ 283 M               │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Other working capital                          │ 31.566 B   │ 43.845 B   │ 46.117 B   │ 56.978 B   │ 61.877 B   │ 70.804 B            │ 88.652 B            │ 100.125 B           │ 101.056 B           │ 107.357 B           │ 117.462 B           │ 149 M               │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Other non cash items                           │ -5.351 B   │ -11.619 B  │ -1.778 B   │ -11.780 B  │ -5.813 B   │ -9.338 B            │ -14.099 B           │ -1.896 B            │ -2.862 B            │ -8.872 B            │ -13.328 B           │ -12.483 B           │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Net cash provided by operating activities      │ 11.081 B   │ 14.565 B   │ 16.619 B   │ 18.659 B   │ 22.376 B   │ 26.024 B            │ 36.036 B            │ 37.091 B            │ 47.971 B            │ 54.520 B            │ 65.124 B            │ 91.652 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Investments in property plant and equipment    │ -4.018 B   │ -3.438 B   │ -3.273 B   │ -7.358 B   │ -10.959 B  │ -9.915 B            │ -10.212 B           │ -13.184 B           │ -25.139 B           │ -23.548 B           │ -22.281 B           │ -24.640 B           │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Acquisitions net                               │ -1.067 B   │ -1.900 B   │ -10.568 B  │ 1.077 B    │ -4.502 B   │ -236 M              │ -986 M              │ -287 M              │ -1.491 B            │ -2.515 B            │ -738 M              │ -2.618 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Purchases of investments                       │ -45.055 B  │ -62.095 B  │ -34.106 B  │ -46.013 B  │ -58.312 B  │ -76.540 B           │ -85.618 B           │ -93.940 B           │ -52.231 B           │ -102.247 B          │ -143.751 B          │ -138.034 B          │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Sales maturities of investments                │ 37.099 B   │ 48.746 B   │ 35.225 B   │ 38.914 B   │ 51.315 B   │ 63.330 B            │ 67.839 B            │ 74.492 B            │ 50.259 B            │ 98.230 B            │ 133.929 B           │ 129.228 B           │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Other investing activities                      │ 2.361 B    │ -354 M     │ -334 M     │ -299 M     │ 1.403 B    │ -350 M              │ -2.188 B            │ 1.518 B             │ 98 M                │ 589 M               │ 68 M                │ 541 M               │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Net cash used for investing activities          │ -10.680 B  │ -19.041 B  │ -13.056 B  │ -13.679 B  │ -21.055 B  │ -23.711 B           │ -31.165 B           │ -31.401 B           │ -28.504 B           │ -29.491 B           │ -32.773 B           │ -35.523 B           │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Debt repayment                                 │ -1.783 B   │ -10.179 B  │ -14.781 B  │ -11.325 B  │ -11.643 B  │ -13.728 B           │ -10.064 B           │ -4.377 B            │ -6.827 B            │ -585 M              │ -2.100 B            │ -21.435 B           │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Common stock issued                            │ 0          │ 0          │ 0          │ 0          │ 0          │ 0                   │ 0                   │ 800 M               │ 950 M               │ 0                   │ 0                   │ 0                   │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Common stock repurchased                       │ -801 M     │ 0          │ 0          │ 0          │ 0          │ -1.780 B            │ -3.693 B            │ -4.846 B            │ -9.075 B            │ -18.396 B           │ -31.149 B           │ -50.274 B           │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Dividends paid                                 │ 0          │ 0          │ 0          │ 0          │ 0          │ 0                   │ 0                   │ 0                   │ 0                   │ 0                   │ 0                   │ 0                   │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Other financing activities                      │ 5.634 B    │ 10.986 B   │ 16.010 B   │ 10.468 B   │ 10.204 B   │ 11.831 B            │ 5.425 B             │ 125 M               │ 1.773 B             │ -4.228 B            │ 8.841 B             │ 10.347 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Net cash used provided by financing activities │ 3.050 B    │ 807 M      │ 1.229 B    │ -857 M     │ -1.439 B   │ -3.677 B            │ -8.332 B            │ -8.298 B            │ -13.179 B           │ -23.209 B           │ -24.408 B           │ -61.362 B           │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Effect of forex changes on cash                │ -19 M      │ 22 M       │ 3 M        │ -3 M       │ -433 M     │ -434 M              │ -170 M              │ 405 M               │ -302 M              │ -23 M               │ 24 M                │ -287 M              │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Net change in cash                             │ 3.432 B    │ -3.647 B   │ 4.795 B    │ 4.120 B    │ -551 M     │ -1.798 B            │ -3.631 B            │ -2.203 B            │ 5.986 B             │ 1.797 B             │ 7.967 B             │ -5.520 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Cash at end of period                          │ 13.630 B   │ 9.983 B    │ 14.778 B   │ 18.898 B   │ 18.347 B   │ 16.549 B            │ 12.918 B            │ 10.715 B            │ 16.701 B            │ 18.498 B            │ 26.465 B            │ 20.945 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Cash at beginning of period                    │ 10.198 B   │ 13.630 B   │ 9.983 B    │ 14.778 B   │ 18.898 B   │ 18.347 B            │ 16.549 B            │ 12.918 B            │ 10.715 B            │ 16.701 B            │ 18.498 B            │ 26.465 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Operating cash flow                            │ 11.081 B   │ 14.565 B   │ 16.619 B   │ 18.659 B   │ 22.376 B   │ 26.024 B            │ 36.036 B            │ 37.091 B            │ 47.971 B            │ 54.520 B            │ 65.124 B            │ 91.652 B            │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Capital expenditure                            │ -4.018 B   │ -3.438 B   │ -3.273 B   │ -7.358 B   │ -10.959 B  │ -9.915 B            │ -10.212 B           │ -13.184 B           │ -25.139 B           │ -23.548 B           │ -22.281 B           │ -24.640 B           │
├────────────────────────────────────────────────┼────────────┼────────────┼────────────┼────────────┼────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┼─────────────────────┤
│ Free cash flow                                 │ 7.063 B    │ 11.127 B   │ 13.346 B   │ 11.301 B   │ 11.417 B   │ 16.109 B            │ 25.824 B            │ 23.907 B            │ 22.832 B            │ 30.972 B            │ 42.843 B            │ 67.012 B            │
└────────────────────────────────────────────────┴────────────┴────────────┴────────────┴────────────┴────────────┴─────────────────────┴─────────────────────┴─────────────────────┴─────────────────────┴─────────────────────┴─────────────────────┴─────────────────────┘
```
```
                                                                                               Final link
Fiscal Date Ending
2010
2011
2012
2013
2014
2015                  https://www.sec.gov/Archives/edgar/data/1652044/000165204416000012/goog10-k2015.htm
2016                https://www.sec.gov/Archives/edgar/data/1652044/000165204417000008/goog10-kq42016.htm
2017                https://www.sec.gov/Archives/edgar/data/1652044/000165204418000007/goog10-kq42017.htm
2018                https://www.sec.gov/Archives/edgar/data/1652044/000165204419000004/goog10-kq42018.htm
2019                  https://www.sec.gov/Archives/edgar/data/1652044/000165204420000008/goog10-k2019.htm
2020                 https://www.sec.gov/Archives/edgar/data/1652044/000165204421000010/goog-20201231.htm
2021                 https://www.sec.gov/Archives/edgar/data/1652044/000165204422000019/goog-20211231.htm
```
```
                                                                                                                 Link
Fiscal Date Ending
2010
2011
2012
2013
2014
2015                              https://www.sec.gov/Archives/edgar/data/1652044/000165204416000012/goog10-k2015.htm
2016                            https://www.sec.gov/Archives/edgar/data/1652044/000165204417000008/goog10-kq42016.htm
2017                            https://www.sec.gov/Archives/edgar/data/1652044/000165204418000007/goog10-kq42017.htm
2018                            https://www.sec.gov/Archives/edgar/data/1652044/000165204419000004/goog10-kq42018.htm
2019                              https://www.sec.gov/Archives/edgar/data/1652044/000165204420000008/goog10-k2019.htm
2020                https://www.sec.gov/Archives/edgar/data/1652044/000165204421000010/0001652044-21-000010-index.htm
2021                https://www.sec.gov/Archives/edgar/data/1652044/000165204422000019/0001652044-22-000019-index.htm
```