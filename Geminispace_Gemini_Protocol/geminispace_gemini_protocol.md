---
marp: true
theme: gaia
class:
  - lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://cdn.gyptazy.ch/images/background.svg')
headingDivider: 1
header: '![left: 5% 5%](https://cdn.gyptazy.ch/images/gyptazy64.png)'
footer: '*(C) 2024 @gyptazy <<contact@gyptazy.ch>>*'
---


# Geminispace / Gemini Protocol
![bg right:40% 80%](https://cdn.gyptazy.ch/images/gemini_logo.png)

What is the Geminispace and the Gemini protocol?


# TOC
![bg right:40% 80%](https://cdn.gyptazy.ch/images/toc.png)
* Introduction
* Motivation
* Protocol
  * Overview
  * Examples
* Software
  * Client
  * Server 


# Introduction
* Introduced in 2019
* Gemini is an application-layer internet communication protocol
  * Similarities to HTTP & Gopher
  * It should co-exist to them and not replace them
* Focussing on:
   * simplicity
   * lightweight 
   * security 


# Motivation
![bg right:40% 80%](https://cdn.gyptazy.ch/images/annyoing.png)
##### Who doesn't know the struggle...
Advertising, Cookie banner, random pop-ups, auto-play music & video, Tracking, Privacy violations, long loading, newsletter subscriptions,  Captchas, slow responses, too much JavaScript, Cookies, not mobile friendly, structureless, annoying site preloader, unreadability, [...]

# Motivation
![bg right:40% 80%](https://cdn.gyptazy.ch/images/more.png)
##### What happened?
##### Features over Content!
## "The more - the better!"

# Motivation
##### Solutions...
* Protocol for serving lightweight hypertext
* Being conservative & standardized but secure
* Simplicity and finite scope are very intentional design
* Focussing on content
###### Like a radically stripped down web stack!

# Protocol
##### Overview
* Works as a request-response protocol
* Run on tcp/1965 (Gemini mission 1965)
* Enforces TLS encryption
* URI-scheme: gemini://
* Response header consists of:
  * 2 digit status code
  * A space
  * Meta field

# Protocol
##### Content - Overview
* File structure similar to HTML
* File formats: .gmi, .gmni, .gemini
* Media type: text/gemini (unofficial)
* Type code: TEXT


# Protocol
##### Gemtext - Syntax
* Gemtext is a text format
* Very limited set of features
* Similar to Markdown
  * Links are in a special format
  * Links can be relative (foo.gmi) or absolute (gemini://gyptazy.ch)

# Protocol (Gemtext Syntax)
```
Headers:
# Big
## Smaller
### Smallest

Lists:
*

Quotes:
> Initial response

Links: 
=> gemini://gyptazy.ch Visit gyptazy.ch
```

# Protocol
##### Content - Example: index.gmi
```
  __ _ _   _ _ __ | |_ __ _ _____   _
 / _` | | | | '_ \| __/ _` |_  / | | |
| (_| | |_| | |_) | || (_| |/ /| |_| |
 \__, |\__, | .__/ \__\__,_/___|\__, |
 |___/ |___/|_|                 |___/
# Welcome
Welcome to my Gemini Capsule on gyptazy.ch!
[...]
## Links
=> ./contact/          ./contact            - Contact
=> ./motiviation/      ./motivation         - Why to run a Gemini capsule
```

# Protocol
##### Content - Static only?
* Well, no!
* Dynamic integrations via CGI

# Protocol
##### Client
![bg right:60% 90%](https://cdn.gyptazy.ch/images/gyptazy_gemini_geminiprotocol_geminispace.jpg)
```gemini://gyptazy.ch/```

# Protocol
##### Server
```
20 text/gemini
# Welcome
Welcome to the Gemini capsule on gyptazy.ch.

## Links
=> gemini://gyptazy.ch   Home Home
=> ./contact             Contact Contact
=> ./gpg                 GPG GPG
```

# Software
##### Overview
* Supports all OS
  * Windows, Linux, BSD, Mac, Android, iPhone, Windows Mobile,...
* Styles
  * GUI
  * CLI

There's a client for almost all OS in all languages!

# Software
##### Clients
| Software | OS | Lang | Mode |
|---|---|---|---|
| Amfora | All | Go | Text (CLI)|
| Bollux | All | Bash | Text (CLI)|
| Agregire | All | Electron | GUI|
| Elaho | iOS | Swift | GUI|
| Xenia | Android | Java | GUI|


# Software
##### Server
| Software | OS | Lang | Mode |
|---|---|---|---|
| gmid | All | C | Simple and secure Gemini server. |
| gmnd | All | Python | Support for CGI and indexing. |
| Hydepark | All | Rust | Forum application for Gemini. |

# Software
##### Misc
* There are http/gemini proxies (comitium)
* There are feed generator (gemgen)
* There are HTML -> Gemini converters (geminize)
* There are site generators (Gempress)
* There is a search engine: gemini://geminispace.info

# Resources
##### Gemini
 * Protocol Insights: https://geminiprotocol.net/docs/protocol-specification.gmi
 * Software overview: https://github.com/kr1sp1n/awesome-gemini
 * Example game: gemini://tictactoe.lanterne.chilliet.eu

 ##### Presentation
* https://gyptazy.ch/talks/


# Thanks!
![bg right:40% 80%](https://cdn.gyptazy.ch/images/thankyou.png)
<br>
Web: &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://gyptazy.ch
Gemini: &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gemini://gyptazy.ch
Twitter: &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;@gyptazy
Fediverse: @gyptazy@gyptazy.ch
Matrix: &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;@gyptazy:gyptazy.ch

# Credits
* image(annyoing.png): Image from Flaticon.com
* image(more.png): Image from Flaticon.com
* image(gemini_logo.png): Image from Flaticon.com
* image(toc.png): Image from Flaticon.com