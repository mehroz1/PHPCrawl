# PHPCrawl
 
## Introduction
Since the development on the original PHPCrawl library by Uwe Hunfeld (phpcrawl@cuab.de) is most certainly dead and it would be a shame to replace such a good piece of code. I have decided to maintain this library. 

For now, I have added support for PHP 8. The test interface works flawless in PHP 8.3.2. I have not tested the entire library with my main project. So, I am not sure if I have completely stabilized it or not.

I have also **disabled** **verify_peer and verify_peer_name** by default while creating stream context on **line 557** of **PHPCrawl/libs/PHPCrawlerHTTPRequest.class.php** 

I will be releasing the 0.84rc1 soon.

For now my focus on fixing any errors or bugs that might occur on PHP 8 and decreasing the average time taken to crawl a single url. 

Link to original repository of PHPCrawl:
https://sourceforge.net/projects/phpcrawl/

