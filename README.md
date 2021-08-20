# dns-example
An illustrated wireshark capture of a browser making a DNS request to get the IP address of a page

## Why

Understanding DNS is helpful context for those wishing to create web pages. DNS itself has significant complexity, which is out of scope for the present document. You might like to check out [this explanation of DNS](https://www.cloudflare.com/en-gb/learning/dns/what-is-dns/).

## Methodology

Wireshark is a traffic monitoring tool that you can run with administrator priviledges on your machine. It can show you every packet of network traffic that passes through your machine. You can see so much, the main issue is finding a way to filter out what you don't want to see. First we filter for DNS to see the DNS request made by the browser, then for HTTP to see the browser request the page itself (and the contents). 

## Results

Here is the result of running the wireshark scan (there is some other traffic going on at the same time from other applications/pages that I have open, which I have shaded out a bit for clarity. The page is requested, by the browser, using the IP address returned from the DNS request.

![foo]



[foo]: ./img/foo.png "Illustrated DNS request before page GET"
