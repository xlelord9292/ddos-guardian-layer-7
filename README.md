## DDOS Guardian
- Layer 7 Version


## What is this?
- This Provide protection toward layer 7 attacks meaning websites attacks

- It works by adding a firewall that goes through ddos guardian then sent to the server if the request is friendly 

- To Setup Look below


## Once u have set up ddos guardian
- How to install ddos guardian https://github.com/xlelord9292/ddos-guardian

- Once u do that then go to /etc/nginx/conf.d/ddos-guardian-layer-7 and edit protection.lua where there is a variable named white list add your server IP if u got IPV4 and IPV6 do this

"IP",
"IP" 

- This will allow your server to send all requests and ignore every firewall we have added

- After you downloaded all of this and edited that then scroll down to 
  <div class="g-recaptcha" data-sitekey="SITE-KEY" data-callback="onSubmit"></div> 
change where it says SITE-KEY to the cloudflare KEY


## How to get the cloudflare key?
- Go To Cloudflare

- Go to Turnstile 

- press Add Site

- give it a name, domains, Managed then No and then press create then it will say Site KEY

- copy and paste the SITE key and replace where it says SITE-KEY in the code with that key then save 

- once u did all of that then go down below

## How to Link this to nginx?
* there is 2 ways u can do this

1. u can edit nginx.conf and add the 
```access_by_lua_file /etc/nginx/conf.d/protection/protection.lua;``` 
line below http {

2. u can edit the files and add it below the location / {
line 

## Now what
- after that then your done and then test if it doesn't work pls contact support

## Warning!
- YOU MAY NOT REMOVE THE POWERED BY DDOS GUARDIAN CREDIT

- YOU MAY NOT RESELL OR TAKE THIS PROJECT REGARDING ANY COPYRIGHT TO DDOS GUARDIAN

- YOU MAY NOT TELL EVERYBODY U OWN THIS PROJECT

## Credits
* Relational Hosting

* Relational Throne

## Support?
https://discord.gg/relationalhosting or https://discord.gg/ax4cnbPY
