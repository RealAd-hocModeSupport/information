# What is wrong with ad-hoc mode support at the moment?

The proper implementation of ad-hoc is mostly dependent on device manufacturers, which almost never fully implement the IEEE 802.11 standard. Let us split the problem in two areas: wireless routers and end-devices.

## Wireless routers

## End-devices (smartphones, laptops, etc)

Are there any alternatives? Not really. Currently there are a few libraries for smartphones that implement device-to-device communication. However, they are either extremely faulty, limited or require infrastructure to work. Find more details in the sections below.

### Bluetooth

* Needs communication w/o pairing
* Reportedly some Android implementations are quite buggy, workarounds sometimes exist

### WiFi Direct

* Requires pairing the devices beforehand
* No real broadcast, one device becomes an Access Point

### Google Nearby

Google Nearby is a fairly recent Android API that allows nearby phones to exchange data among them. Quite absurdly, this mechanism requires an Internet access. In other words: it is not infrastructureless, hence it cannot replace ad-hoc mode.

### Ad-Hoc Mode

* does not exist in iOS
* Not available via the API on Android


### 802.11s

* No support on mobile phones so far

## Conclusion

* When only using mobile phones, Bluetooth is the only option
* Possibly use an external device which can be an Access Point and mesh with other devices simultaneously
