[README.md](https://github.com/user-attachments/files/22510006/README.md)
# EKS Custody Alarm

A simple, immersive, and lightweight custody alarm for FiveM using `ox_target`.

## Features
- Multiple stations, each with named activation and deactivation points
- Third-eye interaction: **Activate Alarm** / **Turn Off Alarm**
- Looped alarm audio (`panicstrip.ogg`) for anyone within 30m (configurable)
- Plain-text `ox_lib` notifications for anyone within 60m (configurable)
- Discord webhooks on **activate** and **deactivate** including:
  - Username only 
  - **Date** and **Time** 
  - Station and **Area**

## Installation

1. Drag and drop the folder into your `resources/` directory.

2. Add the following to your `server.cfg` (ensure order):

ensure ox_lib
ensure ox_target
ensure EKS_CustodyAlarm

3. Open `config.lua` and set:

- `Config.Webhook` to your Discord webhook URL.
- (Optional) `Config.Debug = true` while testing.

4. (Optional) Edit `config.lua` to customize:

- `Config.Alarm.SoundRadius` (default 30.0)
- `Config.Alarm.NotifyRadius` and `NotifyDuration`
- `Config.Alarm.Volume` and `Loop`
- `Config.UseUTC` and `Config.TimeFormat`
- `Config.SendDeactivationEmbed`
- `Config.Stations` (add your stations and named points)

## Support

For help or customization, open a ticket through EKS.

https://discord.gg/busQ9w6dqa
