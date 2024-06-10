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
> ไปที่ qb-multicharacter\client\main.lua 
> ```js
>Config = {}
>Config.Interior = vector3(-814.89, 181.95, 76.85) -- Interior to load where characters are previewed
>Config.DefaultSpawn = vector3(2543.96, 975.03, 6.09) -- Default spawn coords if you have start apartments disabled
>Config.PedCoords = vector4(-1785.67, 642.47, 12.05, 271.5) -- Create preview ped at these coordinates
>Config.HiddenCoords = vector4(-1780.06, 651.51, 13.32, 273.36) -- Hides your actual ped while you are in selection
>Config.CamCoords = vector4(-1782.49, 642.66, 12.05, 92.92) -- Camera coordinates for character preview screen
>Config.EnableDeleteButton = true -- Define if the player can delete the character or not
>Config.customNationality = false -- Defines if Nationality input is custom of blocked to the list of Countries
>Config.SkipSelection = true -- Skip the spawn selection and spawns the player at the last location
>Config.DefaultNumberOfCharacters = 5 -- Define maximum amount of default characters (maximum 5 characters defined by default)
>Config.PlayersNumberOfCharacters = { -- Define maximum amount of player characters by rockstar license (you can find this license in your server's database in the player table)
>    { license = "license:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx", numberOfChars = 2 },
>}
>```
---


> ไปที่ qb-apartments\config.lua
> ```js
>Apartments.Starting = false
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
