# Читайте внимательно!

Это личный конфиг, который используется в постоянке, если zapret не помогает. 

Предисловие, если вы хотите пользоваться v2rayn, то придется найти вам подписку, которая вам предоставит доступ к серверам. Могу закинуть только `https://t.me/athena_vpn_bot`

Инструкция:
1. Заходите в приложение
2. Settings -> Routing Setting
3. Add 
- Remark: Любое название - просто имя для конфига
4. Add Rule (ВАЖНО, СМОТРИ КОНФИГ 3 СРАЗУ. Я ПРЕДУПРЕДИЛ!)
- Конфиг 1:
    - Remarks: Название любое (используется файлы customdomains-*)
    - outboundTag: Proxy
    - port: (пустой, т.к., если вставишь порт, то ломается либо zapret, либо весь поток будет идти через прокси, что не желательно в proxy mode)
    - domain: (вставляешь домены из файла customdomains-domains)
    - process: (вставляешь домены из customdomains-apps) - местами не уверен, работает ли или нет.
    
- Конфиг 2:
    - Remarks: назвал его jetbrains (смотри в секцию jetbrains, чтобы понять, как настроить его)
    - outboundTag: proxy
    - inboundTag: socks
    domain: jetbrains.com

- Конфиг 3 (ВАЖНО!!! БЕЗ НЕГО ТЫ ЛИБО БУДЕШЬ ПРОКСИРОВАТЬ ВЕСЬ ТРАФИК ЧЕРЕЗ ПОДПИСКУ, ЛИБО НЕ БУДЕТ ДОСТУПА В ИНТЕРНЕТ)
    - Remarks: Direct
    - outboundTag: Direct
    - port: 0-65535

# Don't wanna for now translate to eng, so I'll use service for translating... Sorry, for any inconvinience 

# Read carefully!

This is a personal config that is constantly used if zapret does not help. 

Preface, if you want to use v2rayn, you will have to find a subscription that will give you access to the servers. I can only send it `https://t.me/athena_vpn_bot `

Instruction manual:
1. Log in to the app
2. Settings -> Routing Setting
3. Add 
- Remark: Any name is just a name for a config
4. Add Rule (IMPORTANT, SEE CONFIG 3 IMMEDIATELY. I WARNED YOU!)
- Config 1:
- Remarks: Any name (using customdomains files-*)
- outboundTag: Proxy
    - port: (empty, because if you insert the port, either zapret breaks, or the entire stream will go through a proxy, which is not desirable in proxy mode)
    - domain: (you insert domains from the customdomains-domains file)
    - process: (inserting domains from customdomains-apps) - sometimes I'm not sure if it works or not.
    
- Config 2:
- Remarks: named it jetbrains (see the jetbrains section to understand how to set it up)
    - outboundTag: proxy
    - inboundTag: socks
    domain: jetbrains.com

- Config 3 (IMPORTANT!!! WITHOUT IT, YOU'LL EITHER HAVE TO PROXY ALL TRAFFIC THROUGH YOUR SUBSCRIPTION, OR YOU WON'T HAVE INTERNET ACCESS)
    - Remarks: Direct
    - outboundTag: Direct
    - port: 0-65535


- CREATED BY EMIREN