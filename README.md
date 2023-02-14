Kullanılan araçlar'a bu linklerden ulaşabilirsiniz.

https://github.com/d3mondev/puredns

https://github.com/projectdiscovery/httpx

https://github.com/michenriksen/aquatone

-----------------------------------------

1.wget 'https://www.whoisds.com//whois-database/newly-registered-domains/MjAyMy0wMi0xMC56aXA=/nrd' -O subdomains.zip && unzip subdomains.zip

Not:Repoda belirtilen domain-names.txt 'in içeriği ile aynıdır.

2.cat domain-names.txt | grep -f filter.txt >> filtered_output.txt

3.puredns resolve filtered_output.txt -r resolvers.txt  >>resolversdomains.txt

----------------------------OR------------------------

//cat filtered_output.txt|httpx>>httpxphishingdomains.txt//

4.cat resolversdomains.txt|httpx -title    

Sonrasında manuel bir şekilde bakabilir veya ekran görüntüleri alınabilir.

cat resolversdomains.txt | aquatone -ports 80,443


Deprem felaketinden sonra dolandırıcıların/fırsatçıların kurmuş olduğu yeni phishing sitelerin, tespit edilmesine yönelik bir yapı kurulmak istenmiştir.

Farklı whois sunucuları kullanılabilir ve yeni oluşturulan domainler, domain-names.txt dosyası içerisine eklenebilir.

Filtrenemek istenen farklı kelimelerde filtrele.txt dosyasına eklenebilir

