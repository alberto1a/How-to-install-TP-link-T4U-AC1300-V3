# How-to-install-TP-link-T4U-AC1300-V3
  It seems that T4U AC1300 V3 with a USB3  is quite difficult to make it work inLinux system since so no reported method could work 
  and rare efforts to make an edit to let it work.
  
  I got difficulty in findg a driver for it in Linux system, moreover, i am a retired materialist knowing computer science little.
  
  But i need to have double wireless networks in series to have a Big Hacker leave me alone.
  I made my best to analyze the structure of a drive and tried to find solutions somehow.
  So far I am still not knowing much about how to create a driver,i.e. the necessary elements, 
  but i spent a lot of time to campare several almost but no successful drivers at that time
  and made some modifications to make them work the first time for T4U ac1300 v3.
  
  Of course the original author knew their driver much more than me. However, i do my best and a lot
  of time testing drivers seriously and not one only but still found severals as the followings, even
  moreover, some drivers can work for all 3 adapters, i.e. T4U ac1300 but also for dwa 172 and dwa 171
  very popular in Taiwan or Mainland. 
  All of working drivers are special thanks to The EDITORS IN GIBHUB.COM who help to make them as formal drivers.

            How to install drivers for  TP-Link T4U ac1300 v3 USB3 in Linux system
     7 Drivers for TP-Link T4U ac1300 v3 USB3 (organized or created from June 27/2019)

  The Installation of TP-link-T4U-AC1300-V3 USB3
      sudo apt-get install dkms -y
      sudo apt-get install build-essential linux-headers-generic linux-headers-`uname -r` -y
      sudo git clone   https://github.com/alberto1a/rtl8812AU_8821AU_linux.git
      cd  rtl8812au_8821au_linux 
      make clean
      make install -j8
      sudo modprobe cfg80211 
                    
                  
   In such situations the drivers for adapters TP-Link T4U ac1300 v3 USB3 can be done successfully. 
   Some of drivers can work for 2 or 3 adapters, ( including D'Link DWA 172 and DWA 171) which makes users apply very easily and conviently.
        
        by        alberto1a/How-to-install-TP-link-T4U-AC1300-V3
                  
                  alberto1a/wifi172-171-t4u                                                      
                            (One driver for 3 wireless adapters)
                  alberto1a/rtl8812AU_8821AU_linux forked from abperiasamy/rtl8812AU_8821AU_linux
                            (One driver for 3 wireless adapters)
                  
                  wifi171-172-abperiasamy,  
                             (One driver for 2 wireless adapters)
           
                   its-izhar/rtl88x2bu-driver
                   cilynx/rtl88x2BU_WiFi_linux_v5.3.1_27678.20180430_COEX20180427-5959 (an excellent and best driver for T4u ac1300)
                   Asus_USB-AC53_rtl8822bu 
                             (One driver for TP-link-T4U-AC1300-V3 adapters)
                  
   That's it for all friends need it in this free Linux world and under the editor's request writing down my short experiences.
                   I am from friendly Taiwan.
                  
                  
