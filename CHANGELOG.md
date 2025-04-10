# ChangeLog

Look at the GH releases from now on.

## stable-10008

Based on stable release 10008.

* 1f7544c fix(build) fix local build
* 2a329fa feat(web): include custom nginx conf files
* 862986a feat(web): Drops userRegion comes from backend now.
* 2b5c291 misc: working on unstable

## stable-9955

Based on stable release 9955.

* 3ba77e1 feat(prosody) - Added TURN_USERNAME and TURN_PASSWORD (#1989)
* 82e98d2 web: Added P2P_STUN_SERVERS environment variable (#1990)
* 02499f8 feat(grafana): prosody monitoring dashboard created (#1879)
* 3af0725 web: add option param for Automatic Gain Control
* 9bc57e2 misc: working on unstable

## stable-9909

Based on stable release 9909.

* 9098202 feat(lint): add tpl lint step for each project (#1983)
* 70b75f5 feat(build): Checks config.js syntax. (#1981)
* f18b182 fix(web): config.js syntax errors (#1980)
* eea18b1 feat: Add an option to enable VLA. (#1979)
* 9527545 feat(web) Add defaults and env variables for codec preference. (#1978)
* 6ae3414 feat(prosody): Sets recorder prefixes.
* 07ea79a feat(prosody): Enables connection resumption for jicofo and jvb.
* 5341065 Update docker-compose.yml (#1968)
* 5e8b702 fix(prosody-visitors): proper variable for transcriber jid in rate limit (#1967)
* d3db3a5 fix(jibri,jicofo,jigasi,prosody,web): respect previous XMPP_RECORDER_DOMAIN value if set (#1966)
* 2d9c3cc feat(web): allow comment at the top of config.js to be overridden (#1964)
* 9fe5b8b fix(web) Remove no longer used config setting. Av1 has already been enabled by default.
* a53775c misc: working on unstable

## stable-9823

Based on stable release 9823.

* 51a1214 feat(jibri) bump Chrome to version 130
* 345f8c2 fix(prosody,jicofo,jigasi,jibri) rename recorder domain to hidden domain
* 47d974d feat(jibri,jicofo,jvb): custom hocon support via include for components that support it (#1960)
* 6443c6f feat(transcriber): fix exposing transcript path in web
* 74d913f feat(transcriber): flag to enable translations (#1953)
* 8909050 feat(transcriber): remote config auth parameters (#1951)
* bb17a29 feat(prosody): enable muc_max_participants in lobby component (#1950)
* 26b6f27 fix(prosody): remove admin_adhoc module from defaults (#1948)
* 4ae7438 feat(prosody): move external_services module and config to global prosody.cfg.lua (#1949)
* 74a536e misc: working on unstable

## stable-9779

Based on stable release 9779.

* a5b719c :sparkles: allow configuration of a custom translation service (such as libretranslate) (#1946)
* d6251b7 feat(jaas): updated jaas URLs (#1944)
* 2a87a50 fix(jigasi): ensure tpl doesn't fail even if no JIGASI_SIP_PASSWORD is set (#1943)
* 5164db7 feat(jigasi): config for jigasi in visitor mode (#1942)
* a88c6e4 feat(prosody): allow s2s whitelist additions (#1940)
* b89c328 fix(prosody): install the new version of jitsi-contrib/prosody-plugins
* 0b75cd1 fix(transcriber): fix bosh and xmpp connections from jigasi to prosody (#1934)
* 4369907 feat(jibri,jicofo,jigasi,jvb,prosody,web): trim empty list entries when splitting with splitList to allow trailing comma (#1932)
* c58a9e5 feat(prosody): allow components access even after max participants is reached (#1930)
* 5e1fcd8 fix(prosody): default value for PROSODY_MODE (#1929)
* 7b7f101 feat(prosody): new flags to disable incoming client and server conection limits (#1928)
* 02aa4f1 fix: Only set app_secret when defined. (#1925)
* df0bb25 fix(prosody): install the new version of jitsi-contrib/prosody-plugins (#1926)
* ff0cdc7 fix(prosody): tpl errors on container startup due to missing variables (#1924)
* 905943d feat(prosody) update prosody contrib plugins from 20240117 to 20240817
* 1f2b14d feat(prosody): enable recorder domain for s2s to visitor nodes to allow transcription support (#1905)
* c9b6679 feat(web): mount load-test volume to expose load-test client from host (#1910)
* b726312 feat(jicofo) add config parameter for ENABLE_MODERATOR_CHECKS
* 2d39624 misc: working on unstable

## stable-9753

Based on stable release 9753.

* 9e17f95 feat(jigasi): allow unique account UID for each entry even if the same auth is used (#1917)
* ad2a577 fix(jigasi): transcriber VOSK URL variable into compose file (#1916)
* 6c08391 feat(jigasi): transcriber configuration supports vosk URL (#1915)
* 1db83ed feat(ldap): Start and configure only if enabled.
* ceb4a51 feat(prosody): Skip some modules for prosody-jvb.
* e7786d5 feat(jigasi): transcriber configuration for OCI and whisper and to skip saving (#1909)
* c5afcde feat(jigasi): support graceful shutdown via sidecar (#1908)
* 5d40297 feat(jigasi): allow optional label for xmpp servers (#1907)
* e7cb0f4 feat(jvb): autoscaler sidecar shutdown hook on finish (#1906)
* b0675c0 prosody: recording metadata module (#1734)
* 36b2e16 feat(web) - Added NGINX_KEEPALIVE_TIMEOUT environment variable
* 24bf3e4 fix(web) add HTTPS port to URL in env.example
* 2280f6b feat(web) add ability to run the web container targetting JaaS
* ff49cd9 Revert "feat(jigasi): install openjdk nonheadless, currently required for dep…" (#1899)
* 66c6ad8 feat(jigasi): install openjdk nonheadless, currently required for dependencies (#1895)
* 3f67408 feat(jigasi,transcriber): transcriber component and jigasi configuration updates (#1881)
* 3e93212 fix(jicofo): pass compose variable for jicofo transcription support (#1893)
* 084266c feat(transcriber): transcriber password in env.example and gen-passwords.sh (#1894)
* e1b14f2 feat(prosody): enable brewery muc modules in internal muc component (#1892)
* 1889c5d fix(web): enable hidden domain when transcriptions or recordings are enabled (#1891)
* 46377d4 feat(prosody): transcriber account support and flag configuration fix (#1890)
* 9f2489d feat(log-analyser): updated grafana dashboards (#1885)
* 1e589f3 feat(log-analyser): transfered docker logs from docker containers and updated readme (#1884)
* 1f056b4 web: remove unnecessary option
* f893e49 base: update tpl
* 7617503 fix(log-analyser): added Jitsi network to loki service
* 27150a2 feat(prometheus): Docker Daemon scraping for monitoring (#1865)
* d6b64a2 misc: working on unstable

## stable-9646

Based on stable release 9646.

* 0dad31d fix(jicofo) enable jigasi brewery with ENABLE_TRANSCRIPTIONS
* fae66ad fix(jibri): IGNORE_CERTIFICATE_ERRORS as boolean
* 54baee2 feat(prosody): custom metrics of stanza counts for prosody service implemented (#1862)
* a88dd8b feat(jvb) default to using dcSCTP
* d2c26aa fix(jigasi) add missing variables to jigasi.yml
* 41559d6 feat(log-analyser): added grafana dashboard provisioning (#1855)
* 2e9e6ca misc: working on unstable

## stable-9584-1

Based on stable release 9584-1.

* 29a4523 feat(jvb) add JVB_CC_TRUST_BWE environment variable
* 0f7be54 feat(prometheus): Prometheus container and basic scraping configuration  (#1838)
* 9c87bba feat(jitsi-meet): added grafana loki and otel integration for log analysis (#1844)
* fcb90ba fix(web): whiteboard config.js syntax error (#1851)
* 811518b misc: working on unstable

## stable-9584

Based on stable release 9584.

* b4604f3 feat(whiteboard) add builtin whiteboard integration
* 49bd165 feat(jibri) update Chrome to 126
* 980703b fix(jibri): display modes in xorg config
* c65d2bd feat(jigasi,jicofo,jvb,jibri,prosody): add healthcheck.sh scripts and prosody http_health mod
* d2ac43d feat(jigasi): Add new environment variables for jigasi configuration (#1841)
* fbc250e feat(prosody): openmetrics module support (#1832)
* 2adac72 feat(prosody): Drop non existing config.
* e22b4f3 feat(jibri): Adds more fonts.
* 982e577 feat(jicofo,jvb,web) default to using SCTP based datachannels
* 55c975f fix(jicofo): use integer for port value to fix addition (#1826)
* 7c8763f base: update tpl to version 1.3.0
* 1d3c0f1 jibri: fail to start if the SYS_ADMIN cap is missing (#1816)
* cacee4e jvb: adds autoscaler sidecar hook to signal final shutdown (#1809)
* 726b0f0 jibri: adds autoscaler sidecar hook to signal final shutdown (#1810)
* f2b2cc4 etherpad: update image version and settings
* 731d6d1 base: update tpl to make toBool more resilient
* 59c4eb2 jvb: add fallback WS server ID
* 9a54843 jvb: add ability to configure the TLS option for colibri WS
* 79a4635 jvb: add ability to disable XMPP
* 77ce86a jvb: add ability to enable SCTP datachannels
* 76ffaa7 jicofo, jvb: fix OCTO + SCTP behaviour
* 0298a30 misc: working on unstable

## stable-9457-2

Based on stable release 9457-2.

* fed87fb web: update acme.sh version to 3.0.7
* 11285cd prosody: Fixed the wrong position of the JWT_SIGN_TYPE setting in the file (#1796)
* f9ff2a4 misc: working on unstable

## stable-9457-1

Based on stable release 9457-1.

* 09bbfaf misc: working on unstable

## stable-9457

Based on stable release 9457.

* 6f98bbe prosody: add ability to customize TURN TTL value
* 8fe3139 jvb: fix autoscaler sidecar config (#1785)
* 48d803c jigasi: fix autoscaler sidecar config for shutdown url (#1784)
* c951116 jibri: fix autoscaler sidecar config (#1783)
* cae1e40 feat(jigasi): Adds trusted domains option.
* e939230 prosody: add ability to customize JWT signature type
* b0f9eb2 prosody: integrate prosody-plugins-contrib
* 604ba22 prosody: Switches lua gc back to incremental. (#1777)
* 68d4b1a jibri: fix xorg modeline for 1280x720 (#1778)
* 8094a17 web: add ability to change CORS header value
* 03b6ca2 web: remove no longer needed mime type definition
* 70ba4cb base: update to Debian Bookworm
* dc5cbae misc: working on unstable

## stable-9364-1

Based on stable release 9364-1.

* a5ebb99 jibri: flag to support prometheus-style metrics (#1768)
* 80fc10e feat(prosody): Cleans up gc settings.
* 69bba17 feat(prosody): Adjusts lua to use generational GC for brewery.cfg.lua.
* 2798426 feat(prosody): Adjusts lua to use generational GC.
* 28d2b32 feat(prosody): Make sure muc tumbstones is disabled.
* d5df19d jigasi: autoscaler sidecar support (#1738)
* 0953ca0 jigasi: skip SIP configuration when configured as a transcriber
* ca1d670 fix: :bug: wrong quote in default config (#1761)
* 360361e jibri: move xmpp config for easier override (#1748)
* 452f5ba misc: working on unstable

## stable-9364

Based on stable release 9364.

* ca61ea2 jibri: add ability to ignore certificate errors
* 615396e java: use Java 17
* 140db22 jibri: check for chrome bin before pre-warm (#1757)
* 648612f feat(prosody): Always report visitors support when enabled.
* 28f3cf8 jvb: lipcap from apt to allow for pcap dumps (#1747)
* 33350c3 prosody: fix env var default value
* d6dc1e3 base-java: install nodejs 20 from nodesource
* 8f84f2f jibri: use storage.googleapis.com location for chromedriver
* 1bbb4ab fix(prosody): Updates a rate whitelist config that changed in jitsi-meet. (#1741)
* eccf68e misc: working on unstable

## stable-9258

Based on stable release 9258.

* a198d56 compose: add jvb dependency to web container (#1739)
* 5c5742b prosody: var for speakerstats modules
* a1d1f2c web: Add env vars for setting 1080p and 4k bitrates.
* bb69407 Remove "ping" in ViarualHosts (#1728)
* 14efd9c prosody: disable "offline" and "register" modules. (#1727)
* 8e28256 misc: working on unstable

## stable-9220-1

Based on stable release 9220-1.

* 1e97277 jibri: update Chrome to version 121
* 310b80d jvb: add env var to control require-valid-address
* b0092bc jicofo,jigasi,jvb: fix accidentally enabling Sentry
* 102281e base: update tpl
* bf237da etherpad: update etherpad image to etherpad/etherpad:1.9.6 (#1725)
* 7381471 misc: working on unstable

## stable-9220

Based on stable release 9220.

* 4eb5575 prosody: c2s encryption flag from environment
* cc34823 prosody: tune internal muc settings
* f512116 prosody: jibri and jigasi skip muc passwords (#1718)
* 6c1f384 Add flag for require-muc-config-flag. (#1717)
* 6e6dd96 web: nginx config for load-test client if present (#1715)
* 11d7d75 fix: Do not load domain_mapper under breakout component (#1714)
* 4ca5763 prosody: the new version of contrib-prosody-plugins (#1713)
* d31e164 build: simplify detection of the target platform
* 21f04ea base: update tpl
* 9b686c6 prosody: Drops unused module.
* 1365d7f base-java: include jdk package
* 4584779 jicofo: fix enable sctp octo defaults (#1708)
* 2a3f8fd web: fix config.js syntax
* df88c7c Fix/web settings prop syntax (#1706)
* d64ae1c web: remove 'startBitrate' that is no longer supported.
* 1cba0b5 web: Fix the maxbitrates config setting. Also, remove the 'enforcePreferredCodec' setting which is no longer supported.
* 1dbe5cd web: cleanup config
* 3a888fd jicofo: add support for max-ssrcs-per-user config
* 5093efb feat: Add testing flag for Av1
* 7f86006 prosody: remove muc_meeting_id from lobby
* c21a598 prosody: visitors config whitespace fix (#1694)
* 8845606 Move trusted_proxies from visitors to main prosody config file. (#1699)
* e41e4f4 Require tls by default. (#1698)
* 80e4ee6 Remove unnecessary modules and properties (#1697)
* 2915176 prosody: skip recorder account unless in client mode
* 46b98b5 prosody: brewery mode for jvb/jicofo discovery muc
* 52eef2e feat: Add an option to set jibri-sip brewery jid. (#1689)
* ab30f56 prosody: enable muc_meeting_id in lobby component
* 5cc0ef0 jicofo: fix duplicate line
* 2a67885 jicofo: trusted domain list
* 78fb030 fix: Fix typo in var name. (#1690)
* 1ad045e feat: Add an option to enable sctp for relays. (#1688)
* aa898e4 jicofo: fix visitors auth domain (#1687)
* ec8615a fix: Fix default JIBRI_PENDING_TIMEOUT. (#1686)
* 483bbde web: trim deprecated options and defaults
* 11cbfcc web: provide bosh URL as relative only if flagged (#1682)
* 60100d6 jvb: expose public IP in autoscaler sidecar config (#1679)
* b8a9080 task: fix shutdown script
* 2e3c272 jvb: fix terminate script for autoscaler sidecar
* 3519113 jvb: finish script for graceful shutdown (#1676)
* 4fba8b5 task: support logging to file in JVB container (#1675)
* 431cdcc web: allow desktop framerate to be automatically determined by the browser
* 4c009ad jvb: fix version for autoscaler config
* 4531615 prosody: add smacks to guest vhost
* b4428bf prosody: use mod_smacks.lua from prosody since 0.12.4
* ee2f3c9 docker-compose.yml: expose jicofo and jvb env vars for defining max memory.
* 940cd97 env.example: add jicofo and jvb env vars for defining max memory.
* 71b3892 jicofo,jvb,jigasi: fix SENTRY_DSN cannot be defined
* e6a0c04 jibri: add check for /dev/shm size
* dbffba1 Revert "jicofo, jigasi, jvb: fix SENTRY_DSN not being read"
* 073f85d Revert "logging: fix reference to old variable"
* 8415c84 logging: fix reference to old variable
* fa2b4db jicofo, jigasi, jvb: fix SENTRY_DSN not being read
* 42a2153 misc: working on unstable

## stable-9111

Based on stable release 9111.

* 825730d web: nginx ws-colibri proxy regex updates (#1645)
* 54d3aca jicofo: add AV1 options
* 0827186 prosody: stun in external services (#1644)
* d67938c misc: working on unstable

## stable-9078

Based on stable release 9078.

* 3b9afe4 release: build images before comitting the changelog
* 54d422b jvb: autoscaler sidecar support
* 9f0658d sample: escape/encapsulate string
* 5d05ba2 jicofo: support jicofo log file for tailing (#1632)
* 8555fe1 web: param to control config.hosts.authDomain (#1627)
* cd1c9fb prosody: remove muc limit messages from visitors (#1626)
* af50dde prosody: s2s whitelist duplicate param fix (#1625)
* eb91893 prosody: add ping module to auth domain (#1624)
* 261caa3 prosody: guest ping module, var for auth type (#1623)
* 7fb1026 prosody: params for limits (#1622)
* cf894ce prosody: variables for lobby and breakout modules
* a827437 prosody: param to link room metadata to main vhost (#1616)
* 5120595 prosody: var for config in main vhost (#1615)
* bebd748 web: flag to control sctp bridge channel choice (#1613)
* 6bfa830 prosody: visitor mode support (#1611)
* 7bfc5c1 prosody: update version of prosody-plugings package
* 3a77aac jicofo: support visitors in jicofo configuration (#1610)
* f860c5d jvb: don’t send Jetty server version
* 63380fa misc: working on unstable

## stable-8960-1

Based on stable release 8960-1.

* 9bd3258 jibri: fix variable names
* 807b7bf misc: working on unstable

## stable-8960

Based on stable release 8960.

* 5c5575c jibri: make some ffmpeg arguments configurable via env variables
* 09b0df4 misc: working on unstable

## stable-8922-1

Based on stable release 8922-1.

* b3abfc0 ci: split unstable build and test workflows (#1601)
* 603d461 jibri: adapt to new ChromeDriver zip file structure
* a76b1f4 jibri: simplify ChromeDriver download
* fd1c308 jibri: fix new ChromeDriver API endpoints
* 2c0a793 jibri: update Chrome to 116
* 916bccb jibri: autoscaler sidecar tuning parameters
* 6e59319 misc: working on unstable

## stable-8922

Based on stable release 8922.

* 1cbb8f8 prosody: add hybrid_matrix_token as a new authentication method
* b5b8ea2 jigasi: add toggle to enable REST shutdown
* 6bb2455 jibri: add extra fonts
* 497015b jicofo: add JICOFO_AUTH_LIFETIME as environment variable
* f18acb4 jicofo, prosody: allow to set different AUTH_TYPE
* dc1994a jicofo: remove shibboleth authentication options
* 58d4736 misc: working on unstable

## stable-8719

Based on stable release 8719.

* 6f72293 jibri: bump Chrome version
* 94c7060 jibri: params to override statsd host and port
* 0569bce jibri: add autoscaler-sidecar service support (#1562)
* 57a7c22 jicofo: add ability to disable auth
* a41578c prosody: update the comma logic while listing TURNs
* 9776714 prosody: allow multiple TURN (#1559)
* ce59d1e jibri: upgrade chrome to 113 (#1555)
* c2f01f3 web: update livestreaming settings according to new config.js
* e4c8c2a jibri: pre-warm chrome first before starting jibri (#1549)
* 809f63c compose: add ability to configure the Jicofo REST port in the host
* b81bd5c misc: working on unstable

## stable-8615

Based on stable release 8615.

* 57e3bb3 jibri: bump Chrome version
* a0a3410 fix: Allows jicofo entering rooms without requiring a password.
* 1c27da8 prosody: fix ranges redux (#1538)
* 9fc8ffa prosody: fix ranges definition (#1537)
* 39de818 prosody: enable rate limits (#1536)
* 3568542 prosody: add timestamps to the log
* edb5e76 workflow: tag jibri and jigasi images with version (#1522)
* 5d1d80d jvb: fix missing dot in env (#1521)
* 0b1b45d base: use FQIN in base/Dockerfile FROM statement
* 29f0cb2 actions: tag images with detected versions (#1518)
* 7c50cb7 web: support loading pwa-worker.js from subdir (#1517)
* 3af59c6 web: fix bosh for subdomains
* 2fdc643 jicofo: use bool instead of string for codec flags (#1507)
* bdcae29 jicofo: fix syntax error on opus end brace (#1506)
* e5d4213 jicofo: additional conference options (#1504)
* 6034e09 jicofo: support opus red audio codec (#1503)
* ef7ef9c jicofo: disable cert verification for jvb xmpp (#1501)
* a8fe1aa jicofo: fix template error in jvb xmpp server (#1500)
* 7d1bf8e jicofo: flag to use presence for bridge health checks (#1499)
* 1a4f9bd jicofo: fix broken rest template (#1498)
* 76f886f jicofo: add bridge region support and local region (#1497)
* 9c2f742 jicofo: fix rest bind in container (#1496)
* ed095bc misc: support alternate xmpp server for jvb (#1495)
* e1c1f1b jicofo: enable rest interface (#1494)
* ca0b92e web: allow custom colibri websocket port (#1491)
* fe5dea3 misc: working on unstable

## stable-8319

Based on stable release 8319.

* 57e852f build: fix native build on M1 macs
* 1cdf970 prosody: fix "<no value>" issue in prosody config
* 4a0b48c etherpad: suppress errors in pad
* 15335c0 misc: working on unstable

## stable-8252

Based on stable release 8252.

* 076dbf7 jibri: fix downloading new (>= 109) ChromeDriver
* 8f40804 jibri: update Chrome to M109
* 1cf8638 compose: fix whiteboard collab server variable name
* 9e0305b prosody: set JWT_ENABLE_DOMAIN_VERIFICATION to false by default
* ac551c3 base: update tpl
* ec972ee base: update tpl
* 8684b0b misc: working on unstable

## stable-8218

Based on stable release 8218.

* 8d7728b jibri: update Chrome to M108
* 9cfbaf2 misc: drop JICOFO_AUTH_USER
* 68751c2 prosody: add metadata component
* 07f7054 jaas: pass the jitsi installation type at provisioning (#1456)
* e219bcf web: add ability to configure whiteboard
* ac12313 misc: working on unstable

## stable-8138-1

Based on stable release 8138-1.

* 8923b72 web: fix missing quotes on config.js string
* 6b11a89 misc: working on unstable

## stable-8138

Based on stable release 8138.

* 1e49d65 web: simplify build
* dd399fe web,jvb: remove ENABLE_MULTISTREAM
* 723d661 jibri: add single-use-mode config option
* ca14c52 web: add more transcription config env vars
* ccc5746 prosody: add ability to configure TURN server transports
* 17d047a misc: working on unstable

## stable-8044-1

Based on stable release 8044-1.

* fd70f04 env: add note about JaaS account creation
* 046bb79 jaas: register JaaS account automatically
* c44c59e misc: working on unstable

## stable-8044

Based on stable release 8044.

* b212dca web: fix parsing IPv6 reolver addresses
* 53b2654 web: auto-detect nginx resolver
* 9fbb5bd jicofo: fix XMPP config (all moved to jicofo.conf)
* a2333b3 jicofo: remove JICOFO_SHORT_ID (removed upstream)
* d764db9 doc: update README
* c694a9e web: set charset as utf-8
* 8660089 misc: working on unstable

## stable-7882

Based on stable release 7882.

* 4fcba2c jibri: update Chrome to M106
* 957a225 misc: working on unstable

## stable-7830

Based on stable release 7830.

* dd95b3d prosody: fix arm64 build
* acb2f4e misc: update stale.yml
* 02e32e5 jibri: update Chrome to M105
* c53de72 jvb: add JVB_ADVERTISE_IPS, deprecating DOCKER_HOST_ADDRESS
* 723acc2 web: add ability to configure the room password digit size
* a1e82ea jvb: migrate config to secure octo
* 91043c5 prosody: upgrade UVS module to be compatible with Prosody 0.12 and luajwtjitsi 3.0
* dc5b6a1 fix: multi tenant setup (#1401)
* 47804d0 prosody: add JWT_ENABLE_DOMAIN_VERIFICATION to compose file
* 832b178 prosody: make GC options configurable
* bf6a68b web: fix setting prefix for subdomains
* 5fabec9 prosody: add end conference
* 7f7a9b4 misc: working on unstable

## stable-7648-4

Based on stable release 7648-4.

* 6449c60 prosody: fix installation of lua inspect module
* 6664c89 prosody: add missing lua-inspect dependency
* 755bd3f prosody: add jigasi and jibri users as admins
* 8c5fba1 jigasi: add ability to disable SIP
* 4fa0a2f jvb: allow configuration of videobridge.ice.advertise-private-candidates
* 74e5942 misc: working on unstable

## stable-7648-3

Based on stable release 7648-3.

* 7890183 jibri: fix ENABLE_RECORDING issue
* a2b86a0 fix: Fixes undefined variable $ENABLE_JAAS_COMPONENTS. Fixes #1377.
* 9f3c81f misc: working on unstable

## stable-7648-2

Based on stable release 7648-2.

* 24b6adb feat: Adds room info http endpoint for jaas components.
* 475be2a misc: working on unstable

## stable-7648-1

Based on stable release 7648-1.

* d9921a0 prosody: fix syntax error
* bc6ce20 jibri: update Chrome to M104
* 7c7a43a prosody: add ability to configure max occupants
* 85a38d9 jibri: add ability to enable Dropbox recording without enabling "service recording"
* f8b7037 jvb: enable multi-stream by default
* eb0dd6b web: fix receiveMultipleVideoStreams flag
* 674f134 misc: working on unstable

## stable-7648

Based on stable release 7648.

* 12941f5 web: turn on multi-stream by default
* 1d4b265 web: add new flag for multi-stream
* 4264f25 prosody: make enable_domain_verification configurable
* 2a7db7c jigasi: fix Sentry test
* 2d106d8 jigasi: adjust log formatter
* 6c9e305 jigasi: temporarily disable G722
* 9edecf2 misc: working on unstable

## stable-7577-2

Based on stable release 7577-2.

* 55e0eed prosody: remove explicit dependency
* e0bc4e4 prosody: add missing net-url dependency
* e811d7b misc: working on unstable

## stable-7577-1

Based on stable release 7577-1.

* 20eb991 prosody: clean build
* 6fb422c prosody: fix not finding the basexx and cjsson modules
* 1768164 misc: working on unstable

## stable-7577

Based on stable release 7577.

* b670959 prosody: simplify container build
* e05a9c2 fixup: template syntax for newly added variables (#1355)
* 164d28b web: migrate deprecated recordings options, add some more
* f126f7a web: set config.videoQuality.maxBitratesVideo to null if no bitrates are specified
* 0364d94 jibri: remove deprecated PulseAudio module
* 1c93e1b web: add support for brandingDataUrl (#1346)
* 4372717 web: add support for wav files to nginx default
* d804ba4 misc: make ignore rule more generic
* b224131 prosody: use ENABLE_IPV6 environment variable
* be8c41f etherpad,jigasi: fix compose file version
* d7cee00 misc: working on unstable

## stable-7439-2

Based on stable release 7439-2.

* b2f704a misc: working on unstable
* 62655d8 release: stable-7439-1
* 22dc822 prosody: fix XMPP_MUC_CONFIGURATION
* 11de38f fix: properly use default SIP config
* 82a5382 fix: add missing $ to JIGASI_XMPP_USER
* 76ff646 misc: working on unstable

## stable-7439-1

Based on stable release 7439-1.

* 76ff646 misc: working on unstable

## stable-7439

Based on stable release 7439.

* ea37859 prosody: add ability to configure MUC modules through ENV variables
* 5ff69fd jvb: fix jvb.conf parsing error
* 8f38fe6 web,jvb: add option to enable multi-stream
* 701dadf jvb: add ability to disable STUN
* 264a3d8 web: add prejoin config options
* fec78e4 jigasi: build on arm
* c04f658 web,jvb: allow underscore in JVB_WS_SERVER_ID
* 55a4591 prosody: configure unbound resolver
* 576e5a9 web: start with clean config.js
* a7f260e web,etherpad: fix default public URL
* 0cbfbfd web: don't proxy HTTP traffic to WS endpoints
* 7ed5063 jibri,compose: avoid mounting /dev/shm/
* fbb8a2d jibri: switch to PulseAudio
* e7533f8 jibri: simplify Dockerfile
* 7e74308 jigasi: switch to Java 11
* a9d1ed6 misc: working on unstable
* b227b73 build: fix multiarch build

## stable-7287-2

Based on stable release 7287-2.

* ab08247 build: make sure JITSI_RELEASE is passed when invoking make
* 5109874 prosody: update to latest stable
* 343ef56 doc: update README
* 829841e jibri: add support for arm64
* 8d5a9cf jvb: fix not setting WS server ID
* cffab8f jibri: fix log location template
* 94833b5 doc: update README
* d3901ba build: also release a "stable" tag
* 9217b0a misc: working on unstable

## stable-7287-1

Based on stable release 7287-1.

* 22e727c build: adapt release process to multiarch builds
* be422c7 jibri: update Chrome to M102
* 1463df4 compose: add ability to override image versions
* 7c29b57 prosody: fix reservations API
* 8337c0b jicofo,prosody: migrate to new reservations system
* 70c5cbf misc: update dialin numbers url setup (#1298)
* 7790012 misc: define ENABLE_JAAS_COMPONENTS variable (#1297)
* 62ad172 misc: update env.example
* 74ef7de web,prosody: add support for JaaS components
* 902a673 misc: move security options in sample file
* 2a23095 misc: use the "unstable" tag between releases
* 741ec4a build: add native arch building support
* 68d97c8 ci: add GH action docker build caching
* 8b02b8a build,ci: add initial arm64 support
* 3b86df0 compose: add ability to change the JVB colibri REST API exposed port
* 458515c env: add link to handbook
* 261577c web: stop using the default config file
* ed6ef89 web: remove config option to control FLoC
* cb5a753 config: simplify configuration
* b505d58 misc: add stalebot
* 5ff2735 web: add e2eping support using env variables
* 6284167 web: add more audio quality options
* 515bd19 misc: working on latest

## stable-7287

Based on stable release 7287.

* 41d6a9a jibri: bump Chrome to version 101
* 88bb1bc feature: support multiple XMPP servers via list (#1276)
* 95af778 jicofo: add optional XMPP_PORT value (#1275)
* da0a43a misc: working on latest

## stable-7210-2

Based on stable release 7210-2.

* 2634e96 misc: working on latest

## stable-7210-1

Based on stable release 7210-1.

* a8e6a34 prosody: completely disable external components
* 8587d29 prosody: add mod_auth_cyrus from community libraries
* 3a070e6 misc: working on latest

## stable-7210

Based on stable release 7210.

* 1afa278 prosody: add temporary workaround for JWT auth
* 6fe240a prosody: update to 0.12
* 097558b ci: dry run Docker builds on PRs
* eca5d16 web: fix matching etherpad location
* 3afc1e3 prosody: update package version
* b0617c0 web: fix Etherpad when using multi-domain
* 0ce0f09 prosody: update version
* 201a1b4 prosody: pin to version 0.11 for now
* 29b4c23 prosody: use a more recent version of luarocks
* c5b049a jvb: forward port 8080 to docker host
* 6af7cd8 doc: update CHANGELOG
* dd7b70b misc: working on latest

## stable-7001

**IMPORTANT:** Starting with this release TCP has support has been removed from the JVB.

Based on stable release 7001.

* 6e0dd04 base: replace frep with tpl
* 1b51c77 feat: Enables polls for breakout rooms.
* 0b019ee feat: Enables tenants/subdomains by default.
* d50df67 fix: Fixes missing variable for prosody plugins.
* 88997f5 prosody: authentication by matrix user authentication service
* 7a93978 jvb: remove TCP support
* c37706c misc: fix label order in  dockerfiles
* 0de062b misc: add missing quotes to labels in dockerfiles
* 76424fd chore: add opencontainers labels to Dockerfiles
* 3b8ed7e misc: working on latest

## stable-6865

Based on stable release 6865.

* 8004ffe Use the new log formatters, clean up stale logging config.
* a862e84 web: cache versioned static files
* 48d499a web: configure remote participant video menu
* 78791ad env.example : ETHERPAD_PUBLIC_URL : incl. /p/ path
* a504b59 misc: working on latest

## stable-6826

Based on stable release 6826.

* 238a636 jibri: correct chromedriver mismatch
* 555a40e doc: update CHANGELOG
* 825b4cb misc: working on latest

## stable-6726-2

**IMPORTANT:** This version updates Prosody to version 0.11.12 to fix CVE-2022-0217: https://prosody.im/security/advisory_20220113/

Based on stable release 6726-2.

* ae3e7e7 jvb: make MUC_NICKNAME configurable
* 0be9c8f web: allow configuring buttons in toolbar and pre-join screen
* d9d12f0 jvb: fix resolving XMPP server aliases
* 81dc384 jigasi: allow jigasi guest participants
* a8a596b jicofo: configure trusted-domains for Jibri if ENABLE_RECORDING is set
* d250ad7 misc: working on latest

## stable-6726-1

Based on stable release 6726-1.

* 9ac7b59 jibri: update Chrome to version 96
* fb2326e prosody: add missing package libldap-common
* 0600ece sample: add  ENABLE_BREAKOUT_ROOMS to env.example
* 6cf0176 misc: working on latest

## stable-6726

Based on stable release 6726.

* e9275d5 jvb: remove deprecated option
* f40a8d5 jicofo: Handle special characters in password
* 6f56e5b web,prosody: add breakout rooms support
* 3208296 base: update base images to Debian Bullseye
* b02a689 env:  fix unexpected character bug with recent docker desktop
* b5dbfa0 misc: working on latest

## stable-6433

Based on stable release 6433.

* 487bcca jvb: try to use the correct IP as the default server ID
* 9e982fe examples: move to jitsi-contrib
* 192a623 jvb: add ability to configure the shutdown API
* 5dcf7b4 compose: changed REACTIONS env variable name in docker-compose file
* d94f4b6 jvb: remove unneeded alias
* 7cd71a2 jibri: default to recording in 720p
* bee4b6a jibri: use new configuration file
* 76a16a8 jvb: use modern config for ice4j
* 18ac85b jibri: allow graceful shutdown of the container
* 3c19ed6 jibri: uppdate Chrome to version 94
* b858b37 base-java: update to Java 11
* 2061b86 misc: enable features by default
* 343062b misc: fix/ improve shebang compatibility
* ff8c1c2 web: regenerate interface_config.js on every boot
* bda1502 prosody: simplify code
* cfd8d3c web: add config options for polls and reactions
* 537fcd5 misc: add support for sentry logging
* be1da0e misc: cleanup Dockerfiles
* 09cf0a8 web: add env variables for configuring vp9
* 3df32d9 web: persist crontabs for letsencrypt
* f748484 jicofo: add enable-auto-login config option
* 96419ba web: remove no longer needed code
* 1835d65 web: recreate interface_config.js on container restart
* b555d41 jicofo: fix boolean values in configuration file
* 6be198c misc: remove quotation marks from TURN configuration (#1111)
* 407a98d misc: working on latest

## stable-6173

Based on stable release 6173.

* c95f0d6 prosody: add support for A/V Moderation
* 856e414 prosody: add ability to configure external TURN server
* bcae3b1 prosody: add domain mapper options to default configuration
* cf90461 web: fix acme.sh pre and post hooks
* 65563d9 misc: working on latest

## stable-5963

Based on stable release 5963.

* 6f6fe77 prosody: enable limits
* db3d790 prosody: fix: restrict room creation to jicofo (#1059)
* 281db36 misc: working on latest

## stable-5870

Based on stable release 5870.

* d9b84cf jibri: set base URL for joining meetings
* a77a43e jibri: update default Chrome version to 90
* a90e4ce doc: drop confusing port number from PUBLIC_URL
* 8620caa doc: clarify env variable
* 6f52f71 web: add FLoC environment variable
* 014aa59 web: add default language variable
* ce25bf6 doc: update CHANGELOG
* 6bf1336 misc: working on latest

## stable-5765-1

Based on stable release 5765.

* 7a47202 jicofo: make sure client-proxy is properly configured
* 5c32833 web: add start environment variables START_WITH_AUDIO_MUTED; START_SILENT; START_WITH_VIDEO_MUTED
* 3d93f2b misc: working on latest

## stable-5765

Based on stable release 5765.

* 9bc262a prosody: fix building unstable images
* 0cbe0d9 web: add a env variable to enable/disable deep linking
* b22421b misc: publish nightly unstable images
* 78699fe web: allow to configure shard name using env variable
* a6853ef jvb: add octo configuration options
* d6fac8e jicofo: disable octo by default
* 1fa5048 doc: add link to Kubernetes setup
* e1cebcc web,jvb: add ability to disable web sockets for colibri
* 6c4dce1 jicofo: fix ENABLE_SCTP type
* 953a4d2 jicofo: use a client proxy connection
* d27336b web: always try to renew cert on container boot
* 73acbad web: remove deprecated config option
* cb4d941 web: removed duplicate host headers
* ec570ba k8s: fix PodSecurityPolicy
* c4fc3d3 web: make a custom interface config possible
* b45b505 web: always install acme.sh when container starts
* 94ca16d etherpad: remove quotes from all env vars
* c89ccc9 jicofo: reintroduce shibboleth auth
* a6486b4 examples: update traefik v2 example
* f4ec023 misc: working on latest

## stable-5390-3

Based on stable release 5390-3.

* a698da5 misc: add jicofo reservation env variables to compose
* 86c3022 web: brandingDataUrl -> dynamicBrandingUrl
* 88e950d jicofo: fix healthcheck
* 493cbdd misc: fix typo
* e12d7f2 web : Add DESKTOP_SHARING_FRAMERATE_MIN and MAX env vars
* fa98a31 examples: fix k8s example
* 88d1034 doc: add port to PUBLIC_URL
* c876b40 doc: update CHANGELOG
* 5cf14b0 misc: working on latest

## stable-5390-2

Based on stable release 5390-2.

* 3e04fb4 prosody: fix lobby when authentication is enabled
* 24781e3 misc: working on latest

## stable-5390-1

Based on stable release 5390-1.

* 3ac5397 misc: working on latest

## stable-5390

Based on stable release 5390.

* 0f541c8 jicofo: migrate to new config
* 12823cb prosody: fix jibri recording websocket error
* 7594ea2 jigasi: add ability to control SIP default room for incoming calls
* b0e653a jigasi: fix when using authentication
* 4564170 misc: working on latest

## stable-5142-4

Based on stable release 5142-4.

* 6f7b2b4 prosody: add internal domain name to default cross-domains list
* ada7b95 jvb: fix check for JVB_TCP_HARVESTER_DISABLED
* a7fb101 jibri: don't provide a non-existing finalizer path
* d013053 jibri: add missing dependency for `kill` command
* 0b25141 web: Add ENABLE_HSTS flag to disable strict-transport-security header
* f856037 web: add more config options
* eedac14 web: add ability to disable IPv6
* af6f3ac doc: update CHANGELOG
* e3bb5c1 misc: working on latest

## stable-5142-3

**Important:** This release should fix some update problems users found in -1 and -2 versions. The main problem observed is the introduction of XMPP WebSockets, which requires extra configuration for the /xmpp-wesocket route if a reverse proxy is used in front of this setup. Pure docker-compose installations don't need any changes.

Based on stable release 5142-3.

* c2c6460 prosody: fix cross-domain WS default value
* 8261f72 jicofo,jigase: add ability to extend the config file
* 6a4887d web: use env variables to set worker processes and connections
* 5679578 prosody: add env var to config cross domain settings
* effb30b prosody: always rebuild configs on start
* 905d431 jicofo,jigasi: always rebuild configs on start
* c52b64a misc: working on latest

## stable-5142-2

Based on stable release 5142-2.

* 700c04a web: properly handle acme.sh return codes
* 4cb181c web: install acme certs to persistent storage
* 1d2c68a web: fix running acme.sh on the right home directory
* 5c44a84 misc: stop using apt-key, it's deprecated
* 5f06c3a doc: update CHANGELOG
* 0f780b4 misc: working on latest

## stable-5142-1

**Important:** This release includes 2 major changes: migrating the base image to Debian Buster and replacing certbot with acme.sh for getting Letś Encrypt certificates. Please report any problems you find!

Based on stable release 5142-1.

* b0cb4a1 web: update TLS config to Mozilla security guidelines
* 0601212 web: replace certbot with acme.sh
* 43f678d build: refactor Makefile
* b00f92a web: use Python 3 only for certbot
* 880b9b0 core: update base image to Debian Buster
* ba01190 web: prevent s6 from restarting cron if it shouldn't be run
* 42a4346 etherpad: use official image and making skin full width
* c36c4d0 web: always rebuild nginx configs on start
* aea4411 Adds private server.
* 6b69576 web: add ability to configure tokenAuthUrl
* ff6d9bc Fix websocket
* e5746ae misc: add ENABLE_PREJOIN_PAGE to .env
* 465816b web,prosody: turn on XMPP WebSocket by default
* d747bfb web,prosody: add XMPP WebSocket / Stream Management support
* 130eb55 jvb: migrate to new config file
* 5290499 doc: updated link for running behind NAT
* 7cb470c misc: support/encourage usage of ShellCheck
* 04a210f misc: working on latest

## stable-5142

Based on stable release 5142.

* 7ab45bb web: add ability to configure prejoin page
* 0c95794 jvb: regenerate config on every boot
* 3ef2221 jvb: add ability to set the WS domain with an env var
* 79d2601 jvb: add ability to specify set the WS_SERVER_ID with an env var
* b277926 jvb: make colibri websocket endpoints dynamic for multiple jvbs
* 991f695 web: remove no longer needed settings
* 8b7cbc3 revert "jicofo: no auth URL in JWT auth mode"
* 33b386b jvb: add missing variable to docker-compose
* 087f024 web: configure brandingDataUrl with env variables
* a404653 web: configure startAudioOnly using environment variable
* e195cbf jvb: make jvb apis available from outside the container
* 409cade web: configure Matomo using environment variables
* b731c60 doc: update CHANGELOG
* 0fbf3b7 misc: working on latest

## stable-5076

**Important:** Starting with this release config.js is autogenerated with every container boot.
In addition, bridge channels now using WebSocket. Some setups may break on upgrade.

Based on stable release 5076.

* 5ceaf5f web: add IPv6 support
* aff3775 xmpp: allow recorders to bypass lobby
* ad5625b jvb: switch to WebSocket based bridge channels
* 8110336 web: add ability to configure the nginx resolver
* 2f47518 jicofo: no auth URL in JWT auth mode
* c149463 web: build config.js on each boot
* c792bbc base: update frep
* bec928c prosody: configure lobby on the guest domain is necessary
* bcbd977 jicofo: pass XMPP_MUC_DOMAIN through docker-compose.yml
* 8f9caa4 jicofo: set XMPP_MUC_COMPONENT_PREFIX
* 2a0120d web: set security headers also for non HTTPS
* e6586f2 jvb: set LOCAL_ADDRESS to the correct local IP (#630)
* 97f5e75 base: optimize size
* b78c89e misc: minor Dockerfile Improvements
* a754519 misc: working on latest

## stable-4857

Based on stable release 4857.

* a81ad73 prosody: add support for lobby
* baed605 web: fix removing closed captions button if transcription is enabled
* edecacd etherpad: add ability to use a external server
* a7563d4 jvb: use JVB_TCP_PORT for exposing the port
* b235ea1 prosody: disable s2s module
* 1d428a8 prosody: use a 2-stage build
* 613c26c misc: working on latest
* 4d72ee3 release: stable-4627-1
* 22b7063 examples: update Traefik v1 example
* 1381b08 prosody: fix installing dependdencies
* 2900c11 misc: add extra line to tag message
* c57a84b misc: working on latest

## stable-4627-1

Based on stable release 4627-1.

* 1381b08 prosody: fix installing dependdencies
* 2900c11 misc: add extra line to tag message
* c57a84b misc: working on latest

## stable-4627

Based on stable release 4627.

* fdf5030 prosody: update configuration
* afafe23 prosody: shrink container size
* 8e7ea34 base: fix setting timezone
* 58441ae doc: update README
* 3c12526 etherpad: update to version 1.8.4
* 0038e71 jibri: install extra dependency
* 0615ed6 doc: add missing volumes to quick start
* 2781865 doc: clarify usage of gen-passwords.sh
* a8d0b6c build: add PHONY target for "release"
* d4a35a6 misc: working on latest

## stable-4548-1

Based on stable release 4548-1.

* abf2f73 jicofo: fix setting incorrect auth URL scheme for JWT
* 3472ab0 jicofo: add ability to configure health checks
* ec3622b jibri: install jitsi-upload-integrations by default
* 0e7bc91 etherpad: pin image version
* 4fa50b9 jwt: do not load token_verification module with disabled authentication
* b0d76a2 jibri: add jq dep for upload integrations
* 53b58fd jvb: add jq, curl deps for graceful_shutdown.sh
* 2d063ad doc: update installation instructions
* e73df5f misc: working on latest

## stable-4548

Based on stable release 4548.

* a79fc0c misc: add release script
* 0f0adc8 compose: add image tag to compose files
* 0177765 misc: fix config volumes to work with SELinux
* eae3f5c jibri: chrome/driver 78 as a stopgap
* 78df6a4 doc: delete unnecessary dot
* 4426ed8 jibri: fix case when /dev/snd is not bound (https://github.com/jitsi/docker-jitsi-meet/issues/240#issuecomment-610422404)
* 125775a web: fix WASM MIME type
* e70975e web: enable GZIP compression for more file types
* 774aba5 misc: set ddefault timezone to UTC
* 3c3fc19 prosody: enable speaker stats and conferene duration modules
* f911df2 jvb: set JVB_TCP_MAPPED_PORT default value
* 1205170 jvb: allow `TCP_HARVESTER_MAPPED_PORT` to be configured
* f7796a1 prosody: add volume  /prosody-plugins-custom to docker-compose
* d44230e prosody: use hashed xmpp auth

## stable-4416

Based on stable release 4416.

* b039b29 web: use certbot-auto
* b95c95d web: improve nginx configuration
* 2dd6b99 k8s: specify namespace for secret
* 7aa2d81 ldap: avoid unnecessary copy
* e1b47db exampless: update Traefik v2 example with UDP
* 0940605 doc: fix typos and minor grammar issues in README
* 1c4b11c doc: correct minor mistake
* c06867b doc: added steps for updating kernel manually in AWS installation
* dc46215 web: remove DHE suites support
* 367621f prosody: remove no longer needed patch
* 34e6601 doc: clarify acronym
* 2c95ab7 web: revert using PUBLIC_URL for BOSH URL
* 7fd7e2b Add docker-compose.override.yml to .gitignore (#438)
* 67a941b misc: update gen-passwords.sh shell code
* 4e2cec6 misc: add configurable service restart policy
* 729f9d2 doc: fix typo in env.example

## stable-4384(-1)

**Important security note:** Previous releases included default passwords for
system accounts, and users who didn't change them are at risk of getting
the authentication system circumvented by an attacker using a system account
with the default password. Please update and use the provided script
(instructions on the README) to generate a strong password for each system
account.

Thanks joernchen for the security report.

<hr/>

Based on stable release 4384.

* 768b6c4 security: fail to start if using the old default password
* 1ffd472 security: add script to generate strong passwords
* a015710 security: don't provide default passwords
* aaec22d jigasi: fix typo in config
* ebfa142 docs: fix grammar and typos
* bab77e0 doc: update env.example
* 7652807 examples: traefik v2
* 10983b4 prosody: prevent item-not-found error in certain cases
* 3524a52 base: fail to start the container if the init script fails
* 7c0c795 jicofo: only configure Jigasi brewery if Jigasi is configured
* 40c2920 build: add prepare command
* 93ba770 prosody: fix installing prosody from the right repository
* 3c07d76 doc: improve wording of README
* ed410d9 doc: fix typo
* fabfb2a doc: fix typo
* 5e6face web: use PUBLIC_URL for etherpaad base and BOSH URLs
* 264df04 jvb: switch to using Jitsi's STUN server by default
* 655cf6b web,prosody,jvb: prepare for new stable release
* ebb4536 doc: update CHANGELOG
* 06c3a83 doc: fix references to running behind NAT in the README

## stable-4101-2

Based on stable release 4101.

* b15bb28 prosody: update to latest stable version
* 75cb31b doc: add build instructions to README
* 25dbde9 doc: fix typo
* badc2d4 doc: add examples/README
* f6f6ca6 Merge branch 'dev'
* 52a1449 doc: clarify DOCKER_HOST_ADDRESS
* f26c9e6 prosody: fix ldap config template
* cd4a071 web: check for certbot's success and exit in case of a failure
* dea8d6c doc: fix typo
* 573c6fa doc: update diagrams
* 29125fd examples: add minimal example to run jitsi behind traefik

## stable-4101-1

Based on stable release 4101.

* b0def9a prosody: use epoll backend
* 8fa9f94 web: update nginx config from upstream
* 2f17380 doc: clarify account registration command
* edfd8f2 ldap: actually fix anonymous binds (Fixes #234)
* f4ac7cc misc: remove bogus quotation marks
* 0a68be1 jibri: start once jicofo has started
* 76acc65 doc: add tip re. ports to open on firewall to README
* e92a00c ldap: fix anonymous binds
* df40447 ldap: add option for ldap starttls support
* 1ebc535 doc: make localhost link in README clickable
* 33abdf3 doc: add mkdir -p ~/.jitsi-meet-cfg/... to README
* 2c93dce doc: fix typo in README
* d7bb2e6 doc: clarify HTTP vs HTTPS in README
* a1df1e0 Revert "prosody: fix restart loop on rolling deployment"
* 986071b jigasi: add missing transcription volumes to dockerfile
* 01eca74 jigasi: generate google cloud credentials from env vars
* cc2c042 prosody: fix restart loop on rolling deployment
* 5423a8a examples: adding simple kubernetes example
* 6eebabd jicofo: set owner jicofo rights for /config directory
* 69ba9ff jigasi: Updates jigasi client default options.
* 2b9a13b jicofo: add support of reservation REST API
* 8bfe7fb jicofo: add support of reservation REST API
* 9b17c05 web: fix letsencrypt renewal
* 6234a18 web: fix letsencrypt renewal
