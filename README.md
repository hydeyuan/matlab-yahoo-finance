matlab-yahoo-finance
====================

Utility functions in Matlab to retrieve and managed Yahoo! Finance data

Yahoo!Finance let to download historical stock prices (included dividends & splits) at finance.yahoo.com.

Instead of parse data from HTML pages, it's possible to do a download directly from ichart.finance.yahoo.com/table.csv?
It returns all data in CSV-format quickly parsable inside Matlab without write the physical CSV file on disk.

The code uses java.io.BufferedReader class to reads text from a character-input stream.

OUTPUT: Ticker, Date, Open(O), High(H), Low(L), Close(C), Volume, Frequency.
OHLC are already adjusted for dividends/splits. Frequency is timeframe: d/w/m (daily,weekly,monthly)

The functions supports MULTI-SYMBOLS request {'AAPL','MSFT',...}


