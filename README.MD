DeadEndRP -

Welcome to the Purge! In this event once its triggered either via command or by an event call made triggered from another script; Players will hear a gently modified version of the warning from the purge. 

After the alarm and warning has done ALL NPC's will pull out a random weapon that can be configured in the Config.lua file and start coming after other NPC's and Players. Lock your doors! They will try and pull you from your vehicle or enter your home. They are truely out for blood! 

Command: /togglepurge
You can start or stop the purge event (admin) with this command. When you end the event, there will be NPC's still agro'd. 

Key Features:
The Alarm brings true emmersion. If you mix it with the thunderstorm weather it truely adds to the experience! The Standalone script is synced across all players and when new players are loading into the server they will be met with the same warning and the NPC's wont attack them until the warning is done. 

Config:
Config = {}

-- Weapon list for NPCs during purge
Config.Weapons = {
    "WEAPON_KNIFE",
    "WEAPON_BAT",
    "WEAPON_CROWBAR",
    "weapon_golfclub",
    "WEAPON_hammer",
    "WEAPON_MACHETE",
    "WEAPON_hatchet",
    "weapon_battleaxe",
    "weapon_poolcue"
}

-- Audio Alert Settings
Config.Volume = 50


-- Mask models for NPCs (GTA V mask props)
Config.Masks = {
    "prop_mask_test_01",      -- Hockey mask
    "prop_mask_scarecrow_01", -- Scarecrow mask
    "prop_mask_scarecrow_02",
    "p_mask_01",             -- Skull mask
    "p_mask_02",
    "prop_aviators_01"       -- Aviator glasses
}

-- In your config.lua
Config.MaxTrackedPeds = 50 -- Prevent memory issues
Config.ScanInterval = 3000 -- More frequent updates

-- Interval (ms) to check for new NPCs to convert into purgers
Config.ScanInterval = 10000

-- Enable debug prints
Config.Debug = true
--[[
Use these triggers to enable or disable the script from another resource

TriggerEvent('purge:SetPurgeStatus', true)  -- Start the purge
TriggerEvent('purge:SetPurgeStatus', false) -- End the purge

]]

Installation is simple! Just Drop the event into your resourses and Ensure PurgeServerEvent! 
The script sits idle waiting for the greenlight with either the command or a trigger

Find this script on my tebex store!
https://www.deadendrp.tebex.io
