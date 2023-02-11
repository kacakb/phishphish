1.wget 'https://www.whoisds.com//whois-database/newly-registered-domains/MjAyMy0wMi0xMC56aXA=/nrd' -O subdomains.zip && unzip subdomains.zip

Not:Repoda belirtilen domain-names.txt 'in içeriği ile aynıdır.

2.cat domain-names.txt | grep -f filter.txt >> filtered_output.txt
Not:Repoda belirtilen Newly Subdomains 'in

3.puredns resolve filtered_output.txt -r resolvers.txt 

4.puredns resolve filtered_output.txt -r resolvers.txt  >>resolversdomains.txt

----------------------------OR------------------------


//cat filtered_output.txt|httpx>>httpxphishingdomains.txt//



5.cat resolversdomains.txt|httpx -title

Sonrasında manuel bir şekilde bakabilir veya ekran görüntüleri alınabilir.

cat resolversdomains.txt | aquatone -ports 80,443


! https://github.com/gkhan496/phishing-brute-earthquake tarafından ilk olarak düşünmülmüştür !


Farklı whois sunucuları kullanılabilir ve domain-names.txt dosyası içerisine eklenebilir.

Filtrenemek istenen farklı kelimelerde filter.txt dosyasına eklenebilir

