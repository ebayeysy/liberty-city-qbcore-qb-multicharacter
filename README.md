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
```

> ไปที่ qb-apartments\config.lua
> ```js
>RegisterNetEvent('qb-multicharacter:client:chooseChar', function()
>    Apartments.Starting = false
>end)
```

>ไปที่ server.cfg
>```js
>set gamebuild to 2189
>set sv_enforceGameBuild 2189
```

> ไปที่ [gameplay]\[maps] 
> ```js
> delete fivem-map-skater
> delete fivem-map-hipster
```

* ขอให้สนุกถ้าหากมีปัญหาติดต่อฉันที่ where_we_are 
* อีเมล kawiaxnyyat@gmail.com
