Last login: Sun Aug 13 20:00:53 on ttys006
fuzhengwei@MacBook-Pro ~ % ab -c 20 -n 1000000 http://127.0.0.1:8091/api/mysql/insert         
This is ApacheBench, Version 2.3 <$Revision: 1879490 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 100000 requests
Completed 200000 requests
Completed 300000 requests
Completed 400000 requests
Completed 500000 requests
Completed 600000 requests
Completed 700000 requests
Completed 800000 requests
Completed 900000 requests
Completed 1000000 requests
Finished 1000000 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   11888.654 seconds
Complete requests:      1000000
Failed requests:        5635
(Connect: 0, Receive: 0, Length: 5635, Exceptions: 0)
Non-2xx responses:      4
Total transferred:      155994633 bytes
HTML transferred:       22994745 bytes
Requests per second:    84.11 [#/sec] (mean)
Time per request:       237.773 [ms] (mean)
Time per request:       11.889 [ms] (mean, across all concurrent requests)
Transfer rate:          12.81 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    1   4.7      0    2015
Processing:    29  237 170.9    193    7807
Waiting:       29  237 170.8    192    7807
Total:         29  238 171.1    193    7807

Percentage of the requests served within a certain time (ms)
50%    193
66%    263
75%    313
80%    346
90%    435
95%    513
98%    619
99%    732
100%   7807 (longest request)
fuzhengwei@MacBook-Pro ~ % ab -c 20 -n 10000 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1879490 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 1000 requests
Completed 2000 requests
Completed 3000 requests
Completed 4000 requests
Completed 5000 requests
Completed 6000 requests
Completed 7000 requests
Completed 8000 requests
Completed 9000 requests
Completed 10000 requests
Finished 10000 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   24.228 seconds
Complete requests:      10000
Failed requests:        20
(Connect: 0, Receive: 0, Length: 20, Exceptions: 0)
Total transferred:      1559980 bytes
HTML transferred:       229980 bytes
Requests per second:    412.74 [#/sec] (mean)
Time per request:       48.457 [ms] (mean)
Time per request:       2.423 [ms] (mean, across all concurrent requests)
Transfer rate:          62.88 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.5      0       8
Processing:     9   47  53.0     39    1067
Waiting:        9   47  53.0     39    1067
Total:          9   47  53.1     39    1067

Percentage of the requests served within a certain time (ms)
50%     39
66%     49
75%     56
80%     61
90%     75
95%     90
98%    113
99%    134
100%   1067 (longest request)
fuzhengwei@MacBook-Pro ~ % ab -c 20 -n 10000 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1879490 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 1000 requests
Completed 2000 requests
Completed 3000 requests
Completed 4000 requests
Completed 5000 requests
Completed 6000 requests
Completed 7000 requests
Completed 8000 requests
Completed 9000 requests
Completed 10000 requests
Finished 10000 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   33.656 seconds
Complete requests:      10000
Failed requests:        0
Total transferred:      1560000 bytes
HTML transferred:       230000 bytes
Requests per second:    297.12 [#/sec] (mean)
Time per request:       67.312 [ms] (mean)
Time per request:       3.366 [ms] (mean, across all concurrent requests)
Transfer rate:          45.27 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.3      0       5
Processing:     9   65  35.6     59     828
Waiting:        9   65  35.5     59     818
Total:          9   66  35.7     60     828

Percentage of the requests served within a certain time (ms)
50%     60
66%     73
75%     81
80%     86
90%    103
95%    119
98%    138
99%    153
100%    828 (longest request)
fuzhengwei@MacBook-Pro ~ % ab -c 20 -n 10000 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1879490 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 1000 requests
Completed 2000 requests
Completed 3000 requests
Completed 4000 requests
Completed 5000 requests
Completed 6000 requests
Completed 7000 requests
Completed 8000 requests
Completed 9000 requests
Completed 10000 requests
Finished 10000 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   25.971 seconds
Complete requests:      10000
Failed requests:        20
(Connect: 0, Receive: 0, Length: 20, Exceptions: 0)
Total transferred:      1559980 bytes
HTML transferred:       229980 bytes
Requests per second:    385.04 [#/sec] (mean)
Time per request:       51.943 [ms] (mean)
Time per request:       2.597 [ms] (mean, across all concurrent requests)
Transfer rate:          58.66 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.3      0       7
Processing:     7   50  52.2     45    1029
Waiting:        7   50  52.2     45    1029
Total:          7   51  52.2     45    1030

Percentage of the requests served within a certain time (ms)
50%     45
66%     54
75%     60
80%     64
90%     75
95%     85
98%     96
99%    110
100%   1030 (longest request)
fuzhengwei@MacBook-Pro ~ % ab -c 20 -n 10000 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1879490 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 1000 requests
Completed 2000 requests
Completed 3000 requests
Completed 4000 requests
Completed 5000 requests
Completed 6000 requests
Completed 7000 requests
Completed 8000 requests
Completed 9000 requests
Completed 10000 requests
Finished 10000 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   25.002 seconds
Complete requests:      10000
Failed requests:        0
Total transferred:      1560000 bytes
HTML transferred:       230000 bytes
Requests per second:    399.97 [#/sec] (mean)
Time per request:       50.004 [ms] (mean)
Time per request:       2.500 [ms] (mean, across all concurrent requests)
Transfer rate:          60.93 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.3      0       7
Processing:     8   48  29.2     43     606
Waiting:        8   48  29.2     43     601
Total:          9   49  29.3     43     606

Percentage of the requests served within a certain time (ms)
50%     43
66%     53
75%     60
80%     64
90%     76
95%     87
98%    107
99%    122
100%    606 (longest request)
fuzhengwei@MacBook-Pro ~ % ab -c 20 -n 10000 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1879490 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 1000 requests
Completed 2000 requests
Completed 3000 requests
Completed 4000 requests
Completed 5000 requests
Completed 6000 requests
Completed 7000 requests
Completed 8000 requests
Completed 9000 requests
Completed 10000 requests
Finished 10000 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   88.990 seconds
Complete requests:      10000
Failed requests:        20
(Connect: 0, Receive: 0, Length: 20, Exceptions: 0)
Total transferred:      1559980 bytes
HTML transferred:       229980 bytes
Requests per second:    112.37 [#/sec] (mean)
Time per request:       177.981 [ms] (mean)
Time per request:       8.899 [ms] (mean, across all concurrent requests)
Transfer rate:          17.12 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.4      0       8
Processing:    41  176 104.9    154    1198
Waiting:       41  176 104.8    154    1198
Total:         41  177 104.9    155    1198

Percentage of the requests served within a certain time (ms)
50%    155
66%    184
75%    206
80%    223
90%    291
95%    378
98%    475
99%    562
100%   1198 (longest request)