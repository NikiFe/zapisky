# HTTP flood attacks mitigation

##  HTTP flood attacks

- subset of (D)DoS attacks
- aiming to degrade server service quality
- targets exhausting resources
- seemingly casual requests
- zombie devices (often IoT)
- easy attack

## Severity of DDoS attacks

- an average of 3% of the websites registered in .com, .net and .org were involved with attacks daily (according to 2017 stats)

## TCP connection

- reliable connection
- both sides know each other's IP address
- starts with TCP handshake
- gets more complicated when NAT gets involved

## HTTP flood attacks levels

- LEVEL 1 -  only send HTTP request
- LEVEL 2 - browser emulations
- LEVEL 3 - real user imitation
  - add mouse movements, key presses, attempt at captcha

## Defense

- reliable not found yet

### State of the art

- machine learning
- HTTP redirect
- surveys on HTTP flood attacks

### Machine learning

- system tries to find rules for packets
- based on decision tree
  - a lot of advantages
- more DDoS types - not only HTTP flood

#### Machine learning problems

- high false positive rate (even 1% is too much)
- decision are (could be) made on packet attributes and timing
  - attributes - IP header, TCP header, HTTP request
- all the relevant attributes could be adjusted (except maybe timing)
- finding datasets with real attacks is difficult
  - noone is willing to conduct attacks and record them, nor release already done ones



### HTTP redirect papers

- system tries to distinguish IoT attacking devices
- based on HTTP redirect
- for refirecting uses IP address
  - URL contains that IP address

### HTTP redirect

- assumption: IoT devices do not implement whole HTTP
  - IoT devices do not react to HTTP response
- reaction costs computational resources

### HTTP redirect papers - problems

- using IP addresses
  - lack of IP addresses at all
  - small number of possible URLs
- only one "redirector"
- solves only IoT

### Surveys on HTTP flood attacks

- techniques solving particular problems
- nothing about complex system
- examples of usable information:
  - button after a while
  - definition of normal server load (under 40%)
  - definition of maximum number of real client's requests (30/s)

### Contribution

- system solves named problems
  - circumvent machine learning problems
  - does not use IP addresses for redirection
  - scalability
- more complex system mitigating more types (levels) of attacks

### Real client and attacking machine differences

- real client uses a browser
  - complete HTTP implementation
  - javascript implementation
- computing power
- real client can pass CAPTCHA test
- real client's location (based on service)

## Proposed system

- aims to serve real clients, block attacking machines
- parts of the system
  - client
  - detecting program(s)
  - firewall
    - has whitelist and blacklist with IP addresses that activates upon attack
    - if client on whitelist can go through
    - if on blacklist it gets blocked
    - if not identified, client redirected on an auxiliary server
  - web server

## Another tasks

- CAPTCHA
- DOM need
- task for JS (computational demands)
  - also more work for attacker

## Firewall - possible extensions

- rules for IP addresses based on country of origin
- time limit for items on lists
- could find malicious IP addresses itself
- load regulation

## Detection program

- not crucial, defense could be still active
- could find malicious IP addresses itself
- other options:
  - system load monitoring
  - machine learning based monitor

## Auxiliary server

- easy HTTP server
- does not have to implement whole HTTP
- tasks assignment can be prepared in memory

## Experiments

- BoNeSi (DDoS botnet simulator)
  - AS can handle 668/s requests (VirtualBox, Python)
- computationally demanding task

### Response duration without defense

- BoNeSi 2500 requests/s
- quite bad results, client can notice

### Response duration with defense

- same conditions, better for the client
- slower when client not verifies, but when client gets verified its not noticeable

## Future work

- get closer to real situation
  - HTTPS, other HTTP versions
  - incorporate other types of flood attacks (SYN flood)
  - other types of desired response (API, Ajax)