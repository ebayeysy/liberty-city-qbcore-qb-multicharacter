# liberty-city-qbcore-qb-multicharacter

# นี้คือ qb-multicharacter สำหรับ liberty city

> ไปที่ qb-multicharacter\client\main.lua  ค้นหา qb-multicharacter:client:chooseChar
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

---
> ไปที่ qb-multicharacter\client\main.lua ค้นหา qb-multicharacter:client:spawnLastLocation
> ```js
>RegisterNetEvent('qb-multicharacter:client:spawnLastLocation', function(coords, cData)
>    QBCore.Functions.TriggerCallback('apartments:GetOwnedApartment', function(result)
>        if result then
>            TriggerEvent("apartments:client:SetHomeBlip", result.type)
>        end
>
>        local ped = PlayerPedId()
>        SetEntityCoords(ped, coords.x, coords.y, coords.z)
>        SetEntityHeading(ped, coords.w)
>        FreezeEntityPosition(ped, false)
>        SetEntityVisible(ped, true)
>        local PlayerData = QBCore.Functions.GetPlayerData()
>        local insideMeta = PlayerData.metadata["inside"]
>        DoScreenFadeOut(500)
>
>        if insideMeta.house then
>            TriggerEvent('qb-houses:client:LastLocationHouse', insideMeta.house)
>        elseif insideMeta.apartment.apartmentType and insideMeta.apartment.apartmentId then
>            TriggerEvent('qb-apartments:client:LastLocationHouse', insideMeta.apartment.apartmentType, insideMeta.apartment.apartmentId)
>        end
>        
>        TriggerServerEvent('QBCore:Server:OnPlayerLoaded')
>        TriggerEvent('QBCore:Client:OnPlayerLoaded')
>        Wait(2000)
>        DoScreenFadeIn(250)
>    end, cData.citizenid)  
>end)
>```

---

---
> ไปที่ qb-multicharacter\config.lua
> ```js
>Config = {}
>Config.Interior = vector3(-814.89, 181.95, 76.85)
>Config.DefaultSpawn = vector3(2543.96, 975.03, 6.09) 
>Config.PedCoords = vector4(-1785.67, 642.47, 12.05, 271.5)
>Config.HiddenCoords = vector4(-1780.06, 651.51, 13.32, 273.36) 
>Config.CamCoords = vector4(-1782.49, 642.66, 12.05, 92.92) 
>Config.EnableDeleteButton = true
>Config.customNationality = false
>Config.SkipSelection = true
>Config.DefaultNumberOfCharacters = 5
>Config.PlayersNumberOfCharacters = {
>    { license = "license:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx", numberOfChars = 2 },
>}
>```

---


> ไปที่ qb-apartments\config.lua
> ```js
>Apartments.Starting = false
>```

---

>ไปที่ server.cfg
>```js
>set gamebuild to 2189
>set sv_enforceGameBuild 2189
>```

---

> ไปที่ [gameplay]\[maps] 
> ```js
> delete fivem-map-skater
> delete fivem-map-hipster
>```

---

* ขอให้สนุกถ้าหากมีปัญหาติดต่อฉันที่ Discord shifulls
* อีเมล kawiaxnyyat@gmail.com
