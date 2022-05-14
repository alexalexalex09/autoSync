# AutoSync

A template for ESP-Now devices to sync with each other freely

## Rationale

Most ESP-Now tutorials require you to know the MAC addresses of each device you plan to sync with. This is fine for installations in place, but in many applications it might be helpful to be able to sync on the fly, in an ad-hoc sort of way.

## What this template does

1. Allow ad-hoc syncing of an arbitrary number of arbitrary devices
2. Set up a procedure for syncing: when multiple devices hold down a button and the let that button go within 3 seconds of each other, they are added to each other's peer list
3. Divide the main loop() function into two while loops: the first to wait for a sync, the second once a sync has been attempted
