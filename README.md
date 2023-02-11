1.wget 'https://www.whoisds.com//whois-database/newly-registered-domains/MjAyMy0wMi0xMC56aXA=/nrd' -O subdomains.zip && unzip subdomains.zip

2.cat domain-names.txt | grep -f filter.txt >> filtered_output.txt


3.puredns resolve filtered_output.txt -r resolvers.txt 

4.puredns resolve filtered_output.txt -r resolvers.txt  >>resolversdomains.txt

----------------------------OR------------------------
//cat filtered_output.txt|httpx>>httpxphishingdomains.txt//

5.cat resolversdomains.txt|httpx -title

Sonrasında manuel bir şekilde bakabilir veya ekran görüntüleri alınabilir.

cat resolversdomains.txt | aquatone -ports 80,443


