# hat-glasses 
Create file example.lua  in small resources and put this into that. 
I don't know it is working or not so you can check tell me also because i don't have hosting for check this thing
 
 
 BTW for people that don't know there is a native for loosing hat/glasses when punched.🙂 
 
``print(help) 
Citizen.CreateThread(function ()
    SetPedCanLosePropsOnDamage(PlayerPedId(), false, 0)
end)

--Better example
local lastped = nil

Citizen.CreateThread(function ()
    while true do
        if PlayerPedId() ~= lastped then
            lastped = PlayerPedId()
            SetPedCanLosePropsOnDamage(PlayerPedId(), false, 0)
        end
        Wait(100)
    end
end
)
``

![image](https://user-images.githubusercontent.com/90241955/148762542-468f6d79-6402-4ff9-9ac3-cc56c6571dd4.png)
like this
All credits goes to kristian770#1702 this person
