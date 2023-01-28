# HP Elitebook 850 G2 Hackintosh (Broadwell - 5th Gen.)

## Hardware
- Processor: Intel Core i7 5500U @2,4Ghz, Turbo@3,0Ghz, TDP: 15W
- iGPU: Intel HD Graphics 5500
- dGPU: AMD Radeon R7 M260X - 1GB Shared Memory GDDR5
- Display: FullHD 1920x1080
- RAM: 2x8GB DDR3L DualChannel SDRAM - 16GB in Total
- Audio: ALC280
- Ethernet: Intel I218LM Gigabit Networkadaptor
- WiFi & Bluetooth: Intel Dualband Wireless AC7265 B/G/N 2,4/5Ghz
- Trackpad: MultiTouch Synaptics
- SDCard Reader: Realtek RTS5227
- Webcam: HP HD Camera
- Fingerprint Sensor: Synaptics (PID003f)
- Mobile Network: HP-ltxxx LTE/3G/2G Module 
- USB: 5x 3.0
- Misc: Wireless Buttons/FN Keys Functions

## Requirements
- min. 16GB USB Drive
- Network Connection
- Brain.exe

## Installation 
1. Prepare your UEFI
   - Load Default Settings
   - Disable VT-d (already Disabled via OpenCore Config (DisableIOMapper))
   - Enable VT-x
   - Disable Fastboot
   - Disable SecureBoot
   - Enable XHCI USB 
   - SATA Mode: AHCI
   - DVMT Pre-Allocated Memory set to 64MB or Higher

2. Download MacOS Monterey from AppStore 
3. Prepare your USB Stick
   - Format via Disk Utility your USB-Drive in GUID and MacOS(HFS)
   - Run Terminal and enter following code to Create the Installer Medium: `sudo /Applications/Install\ macOS\ Monterey.app/Contents/Resources/createinstallmedia --volume /Volumes/yourusbname` | Replace yourusbname with your created USB Drive Name
4. run via Terminal: `sudo diskutil list` then find your USB Device e.g. disk0sX (u must have 2 Partitions e.g. EFI and Install Monterey) Pick the EFI and run `sudo diskutil mount diskXsX`. Now u have mounted your EFI Partition.
5. Copy the EFI Folder to the USB Drive. The Structure must be: /drive/EFI/EFI/OCandBOOT/
6. Reboot your PC and Boot from it via F9 Key!

## Downloads

## Working

## Not Working

> - coming soon - 
