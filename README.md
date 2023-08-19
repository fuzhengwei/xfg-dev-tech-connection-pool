## 0. no-pool

(base) fuzhengwei1@ZBMac-GV47H1GXD ~ % ab -c 20 -n 600 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1901567 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 100 requests
Completed 200 requests
Completed 300 requests
Completed 400 requests
Completed 500 requests
Completed 600 requests
Finished 600 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   9.267 seconds
Complete requests:      600
Failed requests:        0
Total transferred:      93600 bytes
HTML transferred:       13800 bytes
Requests per second:    64.74 [#/sec] (mean)
Time per request:       308.911 [ms] (mean)
Time per request:       15.446 [ms] (mean, across all concurrent requests)
Transfer rate:          9.86 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.3      0       2
Processing:    65  276 182.2    217    1022
Waiting:       65  269 177.1    212    1000
Total:         65  276 182.3    218    1023

Percentage of the requests served within a certain time (ms)
50%    218
66%    283
75%    353
80%    389
90%    534
95%    745
98%    808
99%    821
100%   1023 (longest request)

## 1. C3P0

ab -c 20 -n 600 http://127.0.0.1:8091/api/mysql/insert

This is ApacheBench, Version 2.3 <$Revision: 1901567 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 100 requests
Completed 200 requests
Completed 300 requests
Completed 400 requests
Completed 500 requests
Completed 600 requests
Finished 600 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   3.729 seconds
Complete requests:      600
Failed requests:        0
Total transferred:      93600 bytes
HTML transferred:       13800 bytes
Requests per second:    160.88 [#/sec] (mean)
Time per request:       124.314 [ms] (mean)
Time per request:       6.216 [ms] (mean, across all concurrent requests)
Transfer rate:          24.51 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.3      0       2
Processing:    15   99  82.8     74     787
Waiting:       13   93  80.3     70     763
Total:         15  100  82.9     74     787

Percentage of the requests served within a certain time (ms)
50%     74
66%    112
75%    135
80%    147
90%    219
95%    256
98%    361
99%    378
100%    787 (longest request)

## 2. DBCP

(base) fuzhengwei1@ZBMac-GV47H1GXD ~ % ab -c 20 -n 600 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1901567 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 100 requests
Completed 200 requests
Completed 300 requests
Completed 400 requests
Completed 500 requests
Completed 600 requests
Finished 600 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   4.174 seconds
Complete requests:      600
Failed requests:        0
Total transferred:      93600 bytes
HTML transferred:       13800 bytes
Requests per second:    143.74 [#/sec] (mean)
Time per request:       139.140 [ms] (mean)
Time per request:       6.957 [ms] (mean, across all concurrent requests)
Transfer rate:          21.90 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.3      0       3
Processing:    15  107  92.8     83     997
Waiting:       15  101  89.3     77     987
Total:         15  107  93.0     83     997

Percentage of the requests served within a certain time (ms)
50%     83
66%    103
75%    121
80%    131
90%    204
95%    253
98%    474
99%    482
100%    997 (longest request)

## druid

fuzhengwei1@ZBMac-GV47H1GXD ~ % ab -c 20 -n 600 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1901567 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 100 requests
Completed 200 requests
Completed 300 requests
Completed 400 requests
Completed 500 requests
Completed 600 requests
Finished 600 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   4.885 seconds
Complete requests:      600
Failed requests:        0
Total transferred:      93600 bytes
HTML transferred:       13800 bytes
Requests per second:    122.83 [#/sec] (mean)
Time per request:       162.827 [ms] (mean)
Time per request:       8.141 [ms] (mean, across all concurrent requests)
Transfer rate:          18.71 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.3      0       2
Processing:    39  144  85.3    121     568
Waiting:       38  138  80.0    115     550
Total:         40  145  85.2    122     568

Percentage of the requests served within a certain time (ms)
50%    122
66%    168
75%    193
80%    205
90%    247
95%    353
98%    395
99%    427
100%    568 (longest request)

## hikari

(base) fuzhengwei1@ZBMac-GV47H1GXD ~ % ab -c 20 -n 600 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1901567 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 100 requests
Completed 200 requests
Completed 300 requests
Completed 400 requests
Completed 500 requests
Completed 600 requests
Finished 600 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   3.793 seconds
Complete requests:      600
Failed requests:        0
Total transferred:      93600 bytes
HTML transferred:       13800 bytes
Requests per second:    158.20 [#/sec] (mean)
Time per request:       126.420 [ms] (mean)
Time per request:       6.321 [ms] (mean, across all concurrent requests)
Transfer rate:          24.10 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.6      0       8
Processing:    13   98  64.2     86     915
Waiting:       12   93  62.6     80     883
Total:         14   98  64.1     86     916

Percentage of the requests served within a certain time (ms)
50%     86
66%    111
75%    136
80%    147
90%    180
95%    199
98%    217
99%    271
100%    916 (longest request)

## 测试；插入、无索引更新、有索引更新

### 1. 插入

(base) fuzhengwei1@ZBMac-GV47H1GXD ~ % ab -c 20 -n 600 http://127.0.0.1:8091/api/mysql/insert
This is ApacheBench, Version 2.3 <$Revision: 1901567 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 127.0.0.1 (be patient)
Completed 100 requests
Completed 200 requests
Completed 300 requests
Completed 400 requests
Completed 500 requests
Completed 600 requests
Finished 600 requests


Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/insert
Document Length:        23 bytes

Concurrency Level:      20
Time taken for tests:   4.009 seconds
Complete requests:      600
Failed requests:        0
Total transferred:      93600 bytes
HTML transferred:       13800 bytes
Requests per second:    149.67 [#/sec] (mean)
Time per request:       133.628 [ms] (mean)
Time per request:       6.681 [ms] (mean, across all concurrent requests)
Transfer rate:          22.80 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.4      0       4
Processing:    19  104  74.0     82     912
Waiting:       12   99  69.2     80     895
Total:         20  105  74.0     82     912

Percentage of the requests served within a certain time (ms)
50%     82
66%    116
75%    136
80%    159
90%    202
95%    243
98%    290
99%    291
100%    912 (longest request)
(base) fuzhengwei1@ZBMac-GV47H1GXD ~ % 

### 2. 无索引更新

### 3. 有索引更新


Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.9      0       8
Processing:    23  164  96.0    139     664
Waiting:       23  161  94.4    137     664
Total:         23  164  96.5    139     669

Percentage of the requests served within a certain time (ms)
50%    139
66%    175
75%    196
80%    211
90%    308
95%    374
98%    448
99%    459
100%    669 (longest request)

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.7      0       6
Processing:     5  163 119.8    125     934
Waiting:        5  154 111.9    119     807
Total:          5  163 119.8    126     937

Percentage of the requests served within a certain time (ms)
50%    126
66%    162
75%    225
80%    248
90%    367
95%    428
98%    471
99%    502
100%    937 (longest request)


服务器软件：
服务器主机名：127.0.0.1
服务器端口：8091

文档路径：/api/mysql/selectByOrderId
文档长度：23字节

并发级别：100
测试所用时间：3.395秒
完成请求：2000
失败请求：0
总传输量：312000字节
HTML传输量：46000字节
每秒请求数：589.09 [#/sec]（平均值）
每个请求的时间：169.752 [ms]（平均值）
每个请求的时间：1.698 [ms]（平均值，所有并发请求）
传输速率：89.74 [Kbytes/sec]（接收）

连接时间（毫秒）
最小值 平均值[+/-标准差] 中位数 最大值
连接：0 0 0.9 0 8
处理：23 164 96.0 139 664
等待：23 161 94.4 137 664
总计：23 164 96.5 139 669

在特定时间内完成请求的百分比（毫秒）
50% 139
66% 175
75% 196
80% 211
90% 308
95% 374
98% 448
99% 459
100% 669（最长请求）

解释：
- 服务器软件：指的是在服务器上运行的软件，用于提供服务和处理请求。
- 服务器主机名：指的是服务器的主机名或IP地址。
- 服务器端口：指的是服务器监听的端口号。
- 文档路径：指的是请求的文档路径。
- 文档长度：指的是请求的文档的长度，以字节为单位。
- 并发级别：指的是同时处理的请求数量。
- 完成请求：指的是成功完成的请求数量。
- 失败请求：指的是失败的请求数量。
- 总传输量：指的是总共传输的数据量，以字节为单位。
- HTML传输量：指的是传输的HTML数据量，以字节为单位。
- 每秒请求数：指的是每秒处理的请求数量，也称为QPS（Queries Per Second）。
- 每个请求的时间：指的是每个请求的平均处理时间，以毫秒为单位。
- 传输速率：指的是接收数据的速率，以千字节/秒为单位。
- 连接时间：指的是建立连接所花费的时间。
- 处理时间：指的是处理请求所花费的时间。
- 等待时间：指的是在处理请求期间等待的时间。
- 百分比的请求时间：指的是在特定时间内完成请求的百分比。例如，50%的请求在139毫秒内完成，99%的请求在459毫秒内完成。

===连接数 25 个

Server Software:        
Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/selectByOrderId
Document Length:        23 bytes

Concurrency Level:      100
Time taken for tests:   2.889 seconds
Complete requests:      2000
Failed requests:        0
Total transferred:      312000 bytes
HTML transferred:       46000 bytes
Requests per second:    692.24 [#/sec] (mean)
Time per request:       144.458 [ms] (mean)
Time per request:       1.445 [ms] (mean, across all concurrent requests)
Transfer rate:          105.46 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.7      0       4
Processing:     4  138  89.9    111     495
Waiting:        3  130  88.1     99     495
Total:          4  139  90.1    111     498

Percentage of the requests served within a certain time (ms)
50%    111
66%    159
75%    206
80%    225
90%    274
95%    309
98%    342
99%    378
100%    498 (longest request)


===== 连接数 5

Server Hostname:        127.0.0.1
Server Port:            8091

Document Path:          /api/mysql/selectByOrderId
Document Length:        23 bytes

Concurrency Level:      100
Time taken for tests:   3.086 seconds
Complete requests:      2000
Failed requests:        0
Total transferred:      312000 bytes
HTML transferred:       46000 bytes
Requests per second:    648.10 [#/sec] (mean)
Time per request:       154.296 [ms] (mean)
Time per request:       1.543 [ms] (mean, across all concurrent requests)
Transfer rate:          98.73 [Kbytes/sec] received

Connection Times (ms)
min  mean[+/-sd] median   max
Connect:        0    0   0.9      0      10
Processing:     5  149 101.4    121     555
Waiting:        4  139  89.9    116     469
Total:          5  149 101.5    122     555

Percentage of the requests served within a certain time (ms)
50%    122
66%    168
75%    201
80%    220
90%    267
95%    398
98%    436
99%    454
100%    555 (longest request)