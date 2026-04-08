# Loon自用配置
# =====================================
# General
# =====================================
[General]
ipv6-vif = auto
resource-parser = https://github.com/sub-store-org/Sub-Store/releases/latest/download/sub-store-parser.loon.min.js
ip-mode = dual
disable-stun = false
dns-reject-mode = LoopbackIP
domain-reject-mode = DNS
udp-fallback-mode = REJECT
sni-sniffing = true
disconnect-on-policy-change = false
switch-node-after-failure-times = 3
# > 跳过某个域名或者IP段
skip-proxy = 192.168.0.0/16,10.0.0.0/8,172.16.0.0/12,localhost,*.local,e.crashlynatics.com
bypass-tun = 10.0.0.0/8,100.64.0.0/10,127.0.0.0/8,169.254.0.0/16,172.16.0.0/12,192.0.0.0/24,192.0.2.0/24,192.88.99.0/24,192.168.0.0/16,198.51.100.0/24,203.0.113.0/24,224.0.0.0/4,255.255.255.255/32
# > DNS 服务器
dns-server = system,223.5.5.5,119.29.29.29,8.8.8.8
interface-mode = auto
# Wi-Fi 访问
# > 允许 Wi-Fi 网络下其它设备访问
#allow-udp-proxy = false
allow-wifi-access = false
wifi-access-http-port = 7222
wifi-access-socks5-port = 7221
# > 代理测速 URL
proxy-test-url = http://www.google.com/generate_204
internet-test-url = http://connectivitycheck.platform.hicloud.com/generate_204
# > 测速超时 (s)
test-timeout = 5
# > 解决一些ip请求无法匹配域名类规则的问题。real-ip指定的域名将不返回fake ip响应，直接将dns请求发往目标dns服务器
#real-ip = msftconnecttest.com,msftncsi.com,*.msftconnecttest.com,*.msftncsi.com,*.srv.nintendo.net,*.stun.playstation.net,xbox.*.microsoft.com,*.xboxlive.com,*.battlenet.com.cn,*.battlenet.com,*.blzstatic.cn,*.battle.net
# 解析器
# resource-parser = https://gitlab.com/sub-store/Sub-Store/-/releases/permalink/latest/downloads/sub-store-parser.loon.min.js
# geoip
geoip-url = https://github.com/Masaiki/GeoIP2-CN/raw/release/Country.mmdb
# ssid-trigger参数，用于指定SSID下流量模式切换，（default表示默认，cellular表示蜂窝，目前支持三种值：rule，direct，proxy） 
# ssid-trigger="default":rule,"cellular":rule,"ASUS":direct,"TPLINK":proxy 
ipasn-url = https://raw.githubusercontent.com/P3TERX/GeoLite.mmdb/download/GeoLite2-ASN.mmdb


# =====================================
# Host
# =====================================
[Host]
# 改善App Store下载速度
iosapps.itunes.apple.com = iosapps.itunes.apple.com.download.ks-cdn.com


# =====================================
# Proxy 本地的代理节点
# =====================================
[Proxy]


# =====================================
# Remote Proxy 订阅链接
# =====================================
[Remote Proxy]


# =====================================
# Proxy Group
# =====================================
[Proxy Group]
X = select,美国节点,日本节点,狮城节点,韩国节点,其他节点,img-url = https://raw.githubusercontent.com/lige47/QuanX-icon-rule/main/icon/twitter(2).png
AI = select,日本节点,狮城节点,美国节点,韩国节点,img-url = https://raw.githubusercontent.com/lige47/QuanX-icon-rule/main/icon/02ProxySoftLogo/Loon(8).png
Apple = select,DIRECT,香港节点,狮城节点,美国节点,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Apple_2.png
Google = select,香港节点,狮城节点,美国节点,日本节点,韩国节点,img-url = https://raw.githubusercontent.com/Orz-3/mini/master/Color/Google.png
Telegram = select,香港节点,狮城节点,美国节点,日本节点,其他节点,img-url = https://raw.githubusercontent.com/fmz200/wool_scripts/main/icons/apps/Telegram_01.png
GitHub = select,美国节点,日本节点,韩国节点,狮城节点,其他节点,香港节点,台湾节点,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/GitHub.png
TikTok = select,香港节点,台湾节点,狮城节点,韩国节点,美国节点,日本节点,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/TikTok_1.png
Spotify = select,美国节点,日本节点,韩国节点,狮城节点,其他节点,img-url = https://raw.githubusercontent.com/lige47/QuanX-icon-rule/main/icon/spotify(green).png
Reddit = select,台湾节点,美国节点,日本节点,韩国节点,狮城节点,img-url = https://raw.githubusercontent.com/lige47/QuanX-icon-rule/main/icon/04ProxySoft/reddit(1).png
Meta = select,狮城节点,香港节点,台湾节点,日本节点,韩国节点,img-url = https://raw.githubusercontent.com/lige47/QuanX-icon-rule/main/icon/meta.png
Discord = select,美国节点,日本节点,韩国节点,狮城节点,img-url = https://raw.githubusercontent.com/lige47/QuanX-icon-rule/main/icon/04ProxySoft/discord(2).png
YouTube = select,香港节点,美国节点,日本节点,韩国节点,狮城节点,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/YouTube.png
Reveal all = select,香港节点,台湾节点,狮城节点,美国节点,日本节点,韩国节点,其他节点,img-url = https://raw.githubusercontent.com/lige47/QuanX-icon-rule/main/icon/05icon/quanqiu(1).png
# 节点筛选
香港节点 = url-test,HK_Filter,interval = 600,tolerance = 50,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Hong_Kong.png
台湾节点 = url-test,TW_Filter,interval = 600,tolerance = 50,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Taiwan.png
美国节点 = url-test,US_Filter,interval = 600,tolerance = 50,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/United_States.png
日本节点 = url-test,JP_Filter,interval = 600,tolerance = 50,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Japan.png
韩国节点 = url-test,KR_Filter,interval = 600,tolerance = 50,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Korea.png
狮城节点 = url-test,SG_Filter,interval = 600,tolerance = 50,img-url = https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Singapore.png
其他节点 = url-test,OT_Filter,interval = 600,tolerance = 50,img-url = https://gitlab.com/lodepuly/iconlibrary/-/raw/main/Flag_icon/120px/WW.png


# =====================================
# Remote Filter
# (?i)：表示后面整个括号内的表达式不区分大小写
# =====================================
[Remote Filter]
OT_Filter = NameRegex, FilterKey = "^(?!.*(?:US|TW|JP|SG|美|韩|日本|新|港|澳|台|英|🇬🇧|🇺🇸|🇲🇴|🇸🇬|🇯🇵|🇭🇰|🇰🇷)).*$"
HK_Filter = NameRegex, FilterKey = "(?i)(🇭🇰|港|HK)"
MO_Filter = NameRegex, FilterKey = "(?i)(🇲🇴|澳门|MO)"
TW_Filter = NameRegex, FilterKey = "(?i)(台|TW|Tai)"
US_Filter = NameRegex, FilterKey = "(?i)(🇺🇸|美|US)"
JP_Filter = NameRegex, FilterKey = "(?i)(🇯🇵|日本|JP|Japan)"
KR_Filter = NameRegex, FilterKey = "(?i)(🇰🇷|KR|Korea|KOR|首尔|韩|韓)"
SG_Filter = NameRegex, FilterKey = "(?i)(🇸🇬|新加坡|狮城|SG|Singapore)"
UK_Filter = NameRegex, FilterKey = "(?i)(🇬🇧|英国)"


# =====================================
# Rule
# Options:no-resolve(only for cidr)
# =====================================
[Rule]
# 信息收集
URL-REGEX,"\.log\.",REJECT
# 海角社区
# 兜底策略
FINAL,Reveal all


# =====================================
# Remote Rule
# =====================================
[Remote Rule]
https://github.com/fmz200/wool_scripts/raw/main/Loon/rule/Twitter.list, policy=X, tag=X, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/rule/AI.list, policy=AI, tag=AI, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/rule/AppleAll.list, policy=Apple, tag=Apple, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Reddit/Reddit.list, policy=Reddit, tag=Reddit, enabled=true
https://github.com/blackmatrix7/ios_rule_script/raw/master/rule/Loon/TikTok/TikTok.list, policy=TikTok, tag=TikTok, enabled=true
https://rule.kelee.one/Loon/Google.lsr, policy=Google, tag=Google, enabled=true
https://rule.kelee.one/Loon/Discord.lsr, policy=Discord, tag=Discord, enabled=true
https://github.com/blackmatrix7/ios_rule_script/raw/master/rule/Loon/Telegram/Telegram.list, policy=Telegram, tag=Telegram, enabled=true
https://github.com/blackmatrix7/ios_rule_script/raw/master/rule/Loon/GitHub/GitHub.list, policy=GitHub, tag=Github, enabled=true
https://github.com/blackmatrix7/ios_rule_script/raw/master/rule/Loon/Spotify/Spotify.list, policy=Spotify, tag=Spotify, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/rule/Facebook.list, policy=Meta, tag=Meta, enabled=true
https://github.com/blackmatrix7/ios_rule_script/raw/master/rule/Loon/YouTube/YouTube.list, policy=YouTube, tag=YouTube, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/ChinaIPs/ChinaIPs.list, policy=DIRECT, tag=大陆IP, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/China/China.list, policy=DIRECT, tag=大陆IP, enabled=true
https://github.com/blackmatrix7/ios_rule_script/raw/master/rule/Loon/Weibo/Weibo.list, policy=DIRECT, tag=Weibo, enabled=true
https://github.com/blackmatrix7/ios_rule_script/raw/master/rule/Loon/WeChat/WeChat.list, policy=DIRECT, tag=WeChat, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/rule/Douyin.list, policy=DIRECT, tag=抖音, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/rule/LAN.list, policy=DIRECT, tag=LAN, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/rule/GeoIP_CN.list, policy=DIRECT, tag=GeoIP_CN, enabled=true
https://raw.githubusercontent.com/NobyDa/Script/master/Surge/AdRule.list, policy=REJECT, tag=NobyDa, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/AdvertisingLite/AdvertisingLite.list, policy=REJECT, tag=ios_rule_script, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Reject/Advertising.list, policy=REJECT, tag=广告拦截, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Reject/Tracking.list, policy=REJECT, tag=隐私保护, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/rule/rejectAd.list, policy=REJECT, tag=广告拦截合集, enabled=true



# =====================================
# Rewrite
# =====================================
[Rewrite]
# TF解锁区域限制
# ^https?://testflight\.apple\.com/v\d/accounts/.+?/install$ request-body-json-jq '.storefrontId = "143441-19,29"'


# =====================================
# Script
# =====================================
[Script]
cron "3 6 * * *" script-path=https://raw.githubusercontent.com/wf021325/qx/master/task/hzh.js, timeout=60, enabled=false, tag=华住会, img-url=https://raw.githubusercontent.com/evilbutcher/Quantumult_X/master/picture/hzh.png
cron "1 6 * * *" script-path=https://raw.githubusercontent.com/evilbutcher/Quantumult_X/master/check_in/glados/checkin_env.js, timeout=60, tag=云翼网络, img-url=https://raw.githubusercontent.com/lige47/QuanX-icon-rule/main/icon/06jichang/ikuuu.png


# =====================================
# Remote Script
# =====================================
[Remote Script]
https://github.com/fmz200/wool_scripts/raw/main/Loon/script/tasks.scripts, tag=定时任务合集, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/script/tools.scripts, tag=脚本工具合集, enabled=true


# =====================================
# 插件
# =====================================
[Plugin]
https://kelee.one/Tool/Loon/Lpx/Block_HTTPDNS.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/BlockAdvertisers.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/AppleWeatherEnhancer.lpx, enabled=true
https://rucu6.pages.dev/Plugins/youtube.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/Soul_remove_ads.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/NeteaseCloudMusic_remove_ads.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/Taobao_remove_ads.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/BaiduNetDisk_remove_ads.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/RedPaper_remove_ads.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/QQMusic_remove_ads.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/Google.lpx, enabled=true
https://kelee.one/Tool/Loon/Lpx/Reddit_remove_ads.lpx, tag=Reddit, enabled=true
https://kelee.one/Tool/Loon/Lpx/FleaMarket_remove_ads.lpx, tag=咸鱼, enabled=true
https://kelee.one/Tool/Loon/Lpx/Weixin_Official_Accounts_remove_ads.lpx, tag=微信公众号, enabled=true
https://kelee.one/Tool/Loon/Lpx/PinDuoDuo_remove_ads.lpx, tag=PDD, enabled=true
https://kelee.one/Tool/Loon/Lpx/QuarkBrowser_remove_ads.lpx, tag=Quark, enabled=true
https://kelee.one/Tool/Loon/Lpx/Amap_remove_ads.lpx, tag=高德地图, enabled=true
https://kelee.one/Tool/Loon/Lpx/Weibo_intl_remove_ads.lpx, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/plugin/WeChatMiniAds.plugin, tag=微信小程序, enabled=true
https://raw.githubusercontent.com/001ProMax/Surge/main/Loon/Spotify.plugin, tag=Spotify, img-url=https://raw.githubusercontent.com/lige47/QuanX-icon-rule/main/icon/spotify(green).png, enabled=true
https://github.com/fmz200/wool_scripts/raw/main/Loon/plugin/blockAds.plugin, policy=REJECT, enabled=true
https://rucu6.pages.dev/Plugins/myblockads.lpx, enabled=true
https://raw.githubusercontent.com/Crazy-Z7/AdGuard/main/Ad.conf, tag=Crazy-Z7, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Advertising.png, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Module/Block/Advertising.sgmodule, tag=神机去广告, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Advertising.png, enabled=true
https://raw.githubusercontent.com/Tartarus2014/Loon-Script/refs/heads/master/Plugin/skip-proxy.lpx, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Alpha/Imm.png, enabled=true
https://raw.githubusercontent.com/VirgilClyne/GetSomeFries/main/plugin/HTTPDNS.Block.plugin, tag=Block HTTPDNS, enabled=true
https://raw.githubusercontent.com/chavyleung/scripts/master/box/rewrite/boxjs.rewrite.loon.plugin, policy=狮城节点, enabled=true
https://raw.githubusercontent.com/sub-store-org/Sub-Store/master/config/Loon.plugin, policy=代理节点, enabled=true
https://raw.githubusercontent.com/Script-Hub-Org/Script-Hub/main/modules/script-hub.loon.plugin, policy=代理节点, enabled=true


# =====================================
# Mitm
# =====================================
[Mitm]
ca-p12 = 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
ca-passphrase = 25143909
hostname =
ca-p12 = 
ca-passphrase = 
skip-server-cert-verify = false
