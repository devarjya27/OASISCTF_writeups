# Description
You decrypt the code and follow all the commands. However, as you think you have breached the firewall, the screen goes black and random numbers start glitching on the screen. You realize that the OASIS realizes that they have left admin privileges and are messing with the computer in order for you not to be able to perform the final push.
# My Solve
Opened the .git folder through the terminal.
```
cat HEAD
ref: refs/heads/master
```
the file path seemed promising. executed cat `/refs/head/master` got some sort of random value which i searched for in each folder (because i am dumb). then found the same `/refs/heads/master` path in the `logs` folder.
```
cd logs
devarjya27@devarjya27-VirtualBox:~/CFT/research/.git/logs$ cat refs/heads/master
0000000000000000000000000000000000000000 a95414405501304d74e659704109609201d98705 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit (initial): O
a95414405501304d74e659704109609201d98705 9d4b23badf043d2a9fff178da857691ebf481f74 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: A
9d4b23badf043d2a9fff178da857691ebf481f74 72ba645a7f2460d0c6e69d7b004a0822de7da488 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: S
72ba645a7f2460d0c6e69d7b004a0822de7da488 e47bb41db3d68d52d8f2d10196124b729d05dd42 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: I
e47bb41db3d68d52d8f2d10196124b729d05dd42 337fc5333c604688da157a296869116ea4355b85 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: S
337fc5333c604688da157a296869116ea4355b85 27633260203b0a9c623158ab4f680cb263b8e0a9 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: {
27633260203b0a9c623158ab4f680cb263b8e0a9 40acf5db7c2e98c70fd3a491e5d70a7f873da7e9 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: g
40acf5db7c2e98c70fd3a491e5d70a7f873da7e9 91f80016136c2767ed84ff7a3c8c91905365eeaf lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: 3
91f80016136c2767ed84ff7a3c8c91905365eeaf eb0fcea0ba96c3fe36c5da488f098bf6ed6e3ff8 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: t
eb0fcea0ba96c3fe36c5da488f098bf6ed6e3ff8 e66d08b985d46afa3f2a524618742f653fced247 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: _
e66d08b985d46afa3f2a524618742f653fced247 2382eea1bf2f3f4e120d1330ef033d6756e31d7f lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: g
2382eea1bf2f3f4e120d1330ef033d6756e31d7f 70a6990713fbcf3d8ca75918c7dd18bcf0b8ae23 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: u
70a6990713fbcf3d8ca75918c7dd18bcf0b8ae23 e5a31476c210ee90f07cc53d147a76fffb594531 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: 6
e5a31476c210ee90f07cc53d147a76fffb594531 f5c50c5f9af1132890081862ddf192d1860a988d lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: 6
f5c50c5f9af1132890081862ddf192d1860a988d 6cfec586a9f63d0b7f4b704b3c66201b1e3266c2 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: 3
6cfec586a9f63d0b7f4b704b3c66201b1e3266c2 d9e63d40a51682d7211dfc1b6864c4f4cae101c9 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: r
d9e63d40a51682d7211dfc1b6864c4f4cae101c9 a79de3e4c5f5b6b5abb01184db648a7034aa60aa lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: _
a79de3e4c5f5b6b5abb01184db648a7034aa60aa 52de07d59b88ef566a90101f69f4aaf9838f3b28 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: 4
52de07d59b88ef566a90101f69f4aaf9838f3b28 a319495a15199ee967d75860695632afc37718ba lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: t
a319495a15199ee967d75860695632afc37718ba d8391837fd525ee4fc9c3592452abefabae923c1 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: _
d8391837fd525ee4fc9c3592452abefabae923c1 8515a9716b2d24bb1c9d7b806dcbba767c961d48 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: g
8515a9716b2d24bb1c9d7b806dcbba767c961d48 52b58986e1945aa88a4d187d89895d5385080627 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: !
52b58986e1945aa88a4d187d89895d5385080627 2e487b56ce6940105cd751c2606375dffd7463d2 lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: t
2e487b56ce6940105cd751c2606375dffd7463d2 03b220bfa6264822e65dc2637cd1aef74b91d69d lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: !
03b220bfa6264822e65dc2637cd1aef74b91d69d 5aa3b6e72af6c0b80a6d8db7331da9160402deea lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: !
5aa3b6e72af6c0b80a6d8db7331da9160402deea 6272ed41c16b23755c88af32b3b8b69d1b99efaa lucky-vers <vermalucky2004@gmail.com> 1724088665 +0530	commit: }
```
and voila we get the flag.
