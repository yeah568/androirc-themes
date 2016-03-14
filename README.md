# androirc-themes
A collection of themes for AndroIRC.

Pull requests for fixes and new themes highly appreciated.

## Installation
Place ```{theme}.xml``` in ```/sdcard/AndroIRC/themes```.
Choose the theme in the AndroIRC settings at Settings -> Settings -> Theme.

## Current Themes

### Monokai
Based on the [HexChat Monokai theme](https://hexchat.github.io/themes.html).

![Monokai screenshot](/Monokai/Monokai_screenshot.png?raw=true "Monokai screenshot")


## Development

### Attribute Guide

- __text_light__: Main text colour.
- __error__: 
- __information__: Informational messages? Includes "Foo has said your nick on #Bar".
- __misc__: 
- __highlight__: Text colour for messages containing a highlight word.
- __join__: User join message. (Foo has joined #Bar)
- __part__: User part message. 
- __away__: /away - Away message. (You are now away, You're no longer away)
- __quit__: 
- __mode__: 
- __nick__: /nick - Nick change message. (Foo is now known as Bar)
- __invite__: 
- __topic__: /topic - Topic/MOTD colour.
- __whois__: /whois - Whois message.
- __ping__: 
- __ctcp__: 
- __notice__: 
- __raw__: 
- __connexion__: 
- __disconnexion__: 
- __stars__: 
- __state_hl__: 
- __state_newmessage__: 
- __state_systemmessage__: 
- __title__: 
- __operator__: Admin and op colour in userlist.
- __half_operator__: Voiced user colour in userlist. __NOTE:__ Yes, voiced user. It appears that hop and voice colours are switched.
- __voice__: Half-op colour in userlist. __NOTE:__ Yes, half-op. It appears that hop and voice colours are switched.

### Message Formatting

Currently, only standard and ACTION messages can be styled.

For standard messages, use:
```xml
<pattern name="message"></pattern>
```

For ACTION (/me) messages, use
```xml
<pattern name="action"></pattern>
```

Place the pattern inside the tag.

The following placeholders can be used:
- ```%rank%``` - Symbol for the rank of the user. 
- ```%nick%``` - User's name.
- ```%message%``` - The actual text.

In addition, ```<bold></bold>```, ```<backgroundcolor color="#c01025"></color>``` and ```<color color="#c01025"></color>``` can be used to style text in the patterns.