!SLIDE
# PhoneGap

!SLIDE
# Virrvarr av språk
### Skal man bruke native code må man forholde seg til:
* iOS: Objective C
* Android: Java "Harmony" / C++
* BlackBerry: JavaJ2ME / C++
* webOS: HTML, CSS & JS
* WinPhone7: .NET

!SLIDE
##Fordeler med
#PhoneGap

* Et felles Javascript-API for forskjellige platformer. 
* Man trenger kun en felles kodebase


!SLIDE
#PhoneGap API
##Gir tilgang til:
*   Sensorer
*   Data
*   Events

!SLIDE
# Sensorer
* GPS
* akselerometer
* Kompass
* Nettverk
* Kamera

!SLIDE
#DATA
* Kontakter
* Media
  * Video
  * Audio
* Notifications

!SLIDE
#EVENTER
* OnDeviceReady
* OnNativeReady
* OnResume
* OnPause

!SLIDE
#I BRUK
## Asynkrone kall
    @@@ javascript
navigator.geolocation.getCurrentPosition(
	function(position){
	
	},
	function(){
	
	}
);