# liberty-city-qbcore-qb-multicharacter

# นี้คือ qb-multicharacter สำหรับ liberty city

> ไปที่ qb-multicharacter\client\main.lua 
> ```js
>RegisterNetEvent('qb-multicharacter:client:chooseChar', function()
>    SetNuiFocus(false, false)
>    DoScreenFadeOut(10)
>    Wait(1000)
>    -- local interior = GetInteriorAtCoords(Config.Interior.x, Config.Interior.y, Config.Interior.z - 18.9)
>    -- LoadInterior(interior)
>    -- while not IsInteriorReady(interior) do
>    --     Wait(1000)
>    -- end
>    FreezeEntityPosition(PlayerPedId(), true)
>    SetEntityCoords(PlayerPedId(), Config.HiddenCoords.x, Config.HiddenCoords.y, Config.HiddenCoords.z)
>    Wait(1500)
>    ShutdownLoadingScreen()
>    ShutdownLoadingScreenNui()
>    openCharMenu(true)
>end)
>```
![Discord ](https://media.discordapp.net/attachments/1156702604324261959/1231389459434438676/image.png?ex=6636c7cd&is=662452cd&hm=979fc970a0514dcf4413fd0d3b03a130f559dca394d1faf637df34bb040d5d4a&=&format=webp&quality=lossless&width=1022&height=340)
---


> ไปที่ qb-apartments\config.lua
> ```js
>RegisterNetEvent('qb-multicharacter:client:chooseChar', function()
>    Apartments.Starting = false
>end)
>```
![Discord ](https://media.discordapp.net/attachments/1156702604324261959/1231389503990661120/image.png?ex=6636c7d7&is=662452d7&hm=3c769ad79bc370a3bfca6d9aeef5d7e155e11c9c1bee43eb4708bbc8cdf2b0e6&=&format=webp&quality=lossless&width=985&height=472)
---

>ไปที่ server.cfg
>```js
>set gamebuild to 2189
>set sv_enforceGameBuild 2189
>```
![Discord ](https://media.discordapp.net/attachments/1156702604324261959/1231389575083986995/image.png?ex=6636c7e8&is=662452e8&hm=d5a56d420df372b98b8ba2578d104f36b647b466bb6baaaf9799b9351ead933a&=&format=webp&quality=lossless&width=376&height=44)
---

> ไปที่ [gameplay]\[maps] 
> ```js
> delete fivem-map-skater
> delete fivem-map-hipster
>```
![Discord ](https://media.discordapp.net/attachments/1156702604324261959/1231389656931893370/image.png?ex=6636c7fc&is=662452fc&hm=23d13b2fb62c899367b27ecc43cccf7cce993b9af1ca09f16a88e5aaa74e1dd1&=&format=webp&quality=lossless&width=1190&height=392)
---

* ขอให้สนุกถ้าหากมีปัญหาติดต่อฉันที่ Discord where_we_are 
* อีเมล kawiaxnyyat@gmail.com
