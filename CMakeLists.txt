cmake_minimum_required(VERSION 3.28)
project(qt_programming_2024)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)


find_package(Qt6 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(qt_programming_2024 src/main.cpp
        src/MyGame.cpp
        src/MyGame.h
        src/Items/Item.cpp
        src/Items/Item.h
        src/Items/Characters/Character.cpp
        src/Items/Characters/Character.h
        src/Items/Characters/Link.cpp
        src/Items/Characters/Link.h
        src/Items/Armors/Armor.cpp
        src/Items/Armors/Armor.h
        src/Items/HeadEquipments/HeadEquipment.cpp
        src/Items/HeadEquipments/HeadEquipment.h
        src/Items/LegEquipments/LegEquipment.cpp
        src/Items/LegEquipments/LegEquipment.h
        src/Items/HeadEquipments/CapOfTheHero.cpp
        src/Items/HeadEquipments/CapOfTheHero.h
        src/Items/Armors/OldShirt.cpp
        src/Items/Armors/OldShirt.h
        src/Items/LegEquipments/WellWornTrousers.cpp
        src/Items/LegEquipments/WellWornTrousers.h
        src/Scenes/Scene.cpp
        src/Scenes/Scene.h
        src/Scenes/BattleScene.cpp
        src/Scenes/BattleScene.h
        assets/assets.qrc
        src/Items/Maps/Map.cpp
        src/Items/Maps/Map.h
        src/Items/Maps/Battlefield.cpp
        src/Items/Maps/Battlefield.h
        src/Items/Mountable.cpp
        src/Items/Mountable.h
        src/Items/Armors/FlamebreakerArmor.cpp
        src/Items/Armors/FlamebreakerArmor.h

        src/Scenes/IceScene.h
        src/Scenes/IceScene.cpp
        src/Items/Maps/Icefield.h
        src/Items/Maps/Icefield.cpp
        src/Items/Weapons/Shabby_Pistol.cpp
        src/Items/Weapons/Weapon.h
        src/Items/Weapons/Weapon.cpp
        src/Items/Weapons/Shabby_Pistol.h
        src/Scenes/SettingsScene.h
        src/Scenes/SettingsScene.cpp
        src/GameEnums.h
        src/Items/Maps/Settingsfield.h
        src/Items/Maps/Settingsfield.cpp
        src/Items/HeadEquipments/Helmet_of_the_Paladin.h
        src/Items/HeadEquipments/Helmet_of_the_Paladin.cpp
        src/Items/Bullets/Bullet.h
        src/Items/Bullets/Bullet.cpp
        src/Items/Bullets/Shabby_Pistol_bullet.h
        src/Items/Bullets/Shabby_Pistol_bullet.cpp









)
target_link_libraries(qt_programming_2024
        Qt::Core
        Qt::Gui
        Qt::Widgets
)

