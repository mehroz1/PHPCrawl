# PHPCrawl
 
## Introduction
Since the development on the original PHPCrawl library by Uwe Hunfeld (phpcrawl@cuab.de) is most certainly dead and it would be a shame to replace such a good piece of code. I have decided to maintain this library. 

For now, I have added support for PHP 8. The test interface works flawless in PHP 8.3.2. I have not tested the entire library with my main project. So, I am not sure if I have completely stabilized it or not.

I have also **disabled** **verify_peer and verify_peer_name** by default while creating stream context on **line 557** of **PHPCrawl/libs/PHPCrawlerHTTPRequest.class.php** 

I will be releasing the **0.84rc1** soon.

Right now, my focus is on fixing any errors or bugs that might occur on PHP 8 and decreasing the average time taken to crawl a single url. 

Link to original repository of PHPCrawl:
https://sourceforge.net/projects/phpcrawl/

If you have any feed back, suggestion or bug to report you are welcome.

## Requirements

Minimum Required 

PHP Version: 7.4.24

Tested Upto

PHP Version: 8.3.2

## Performance Metrics

### Test 1
URL to crawl: https://en.wikipedia.org/wiki/Spanish_Inquisition

Follow mode: 3

Page/File limit: 100

Content-types to receive: #text/html#

PHP: 8.3.2

OS: Windows 10

Processor: Intel(R) Xeon(R) CPU E5-1620 0 @ 3.60GHz

Disk Type: SSD

Process finished!  	

Links followed: 	             100

Kb received: 	               35409

Data throughput kb/s: 	         208

Files received: 	             100

Time in sec: 	              170.19

Max memory-usage in KB: 	30720.00

### Conclusion:

Average time taken to crawl single url is 1.7019s.

### Test 2

URL to crawl: https://en.wikipedia.org/wiki/Spanish_Inquisition

Follow mode: 3

Page/File limit: 100

Content-types to receive: #text/html#

PHP: 7.4.24

OS: Windows 10

Processor: Intel(R) Xeon(R) CPU E5-1620 0 @ 3.60GHz

Disk Type: SSD

Process finished!

Links followed: 	100

Kb received: 	35410

Data throughput kb/s: 	216  

Files received: 	100

Time in sec: 	163.87

Max memory-usage in KB: 	30720.00

### Conclusion:

Average time taken to crawl single url is 1.6387s.

**Note:** 

These metrics can change depending on condition of your internet connection and hardware used.

The average time provided in above tests should be taken with a grain of salt as the network conditions and server response times vary. So any change in fraction should be ignored in my opinion.