# rPI-Tests
Tools &amp; data: Performance Tests on Raspberry PI 3 Model B+ &amp; B


## Scripts
* `queenpool_multithread.py <Output.csv> <Queens> <Threads> <Repeat>`: It Solves the N-Queen Problem. Usage:

```
queenpool_multithread.py multithread_output.csv 12 4 100
```
This code example solves the N-queens problem with N=12 using 4 threads and repeat the process 100 times. 
Note: It only works with Raspberry Pi because of the temperature measurement. If you need to use it, you need to remove this.

* `temperature.py`: Need by `queenpool_multithread.py` for temperature measurement on the Raspberry Pi.
* `webserver.py`: It starts a web server that responds to GET and POST and allows to upload files from a Client. You need to modify the upload path.
* `webclient.py`: It connects to the web server started using `webserver.py` and send the contain of the images located in the images folder.

## More Information
* [Raspberry Pi 3 Model B & B+ Performance Tests](https://lemariva.com/blog/2018/04/raspberry-pi-the-n-queens-problem-performance-test)

If you find the results of the Performance Tests useful, please leave a comment and spread the news! Thanks!
