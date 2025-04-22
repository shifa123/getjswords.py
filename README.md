# How to Use:

1. waybackurls example.com | tee example-js.txt
2. cat example-js.txt|sed -E 's/(\.js)(\?.*|#.*)?$/\1/'|sort -u| uniq | tee example-js-uniq.txt
3. example-js-uniq.txt | python3 getjswords.py | tee example-js-uniq-wordlist.txt
4. Enjoy with your customised wordlist file example-js-uniq-wordlist.txt
