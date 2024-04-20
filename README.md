# liberty-city-qbcore-qb-multicharacter

# นี้คือ qb-multicharacter สำหรับ liberty city

> 
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
![Discord ](https://media.discordapp.net/attachments/1156702604324261959/1231389459434438676/image.png?ex=6636c7cd&is=662452cd&hm=979fc970a0514dcf4413fd0d3b03a130f559dca394d1faf637df34bb040d5d4a&=&format=webp&quality=lossless&width=577&height=192)
> ```

> 
> ไปที่ qb-apartments\config.lua
> ```js
> Apartments.Starting = false
> ```

> ไปที่ server.cfg
> ```js
> set gamebuild to 2189
- set sv_enforceGameBuild 2189
> ```

> ไปที่ [gameplay]\[maps] 
> ```js
> ลบ fivem-map-skater
> ลบ fivem-map-hipster
> ```

