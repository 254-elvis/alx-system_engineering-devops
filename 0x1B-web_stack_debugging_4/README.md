root@0a62aa706eb3:/#
root@0a62aa706eb3:/# puppet apply 0-the_sky_is_the_limit_not.pp
Notice: Compiled catalog for 0a62aa706eb3.local in environment production in 0.01 seconds
Notice: /Stage[main]/Main/Exec[fix--for-nginx]/returns: executed successfully
Notice: Finished catalog run in 1.12 seconds
root@0a62aa706eb3:/#
root@0a62aa706eb3:/#
root@0a62aa706eb3:/# ab -c 100 -n 2000 localhost/
This is ApacheBench, Version 2.3 <$Revision: 1528965 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking localhost (be patient)
Completed 200 requests
Completed 400 requests
Completed 600 requests
Completed 800 requests
Completed 1000 requests
Completed 1200 requests
Completed 1400 requests
Completed 1600 requests
Completed 1800 requests
Completed 2000 requests
Finished 2000 requests


Server Software:        nginx/1.4.6
Server Hostname:        localhost
Server Port:            80

Document Path:          /
Document Length:        612 bytes

Concurrency Level:      100
Time taken for tests:   0.301 seconds
Complete requests:      2000
Failed requests:        0
Total transferred:      1706000 bytes
HTML transferred:       1224000 bytes
Requests per second:    6650.99 [#/sec] (mean)
Time per request:       15.035 [ms] (mean)
Time per request:       0.150 [ms] (mean, across all concurrent requests)
Transfer rate:          5540.33 [Kbytes/sec] received
