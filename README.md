## CP21xx Silicon labs. USB2UART adapter used in multi-port USB and fixed COM port number on PC

#### CP21xx 在同一台PC下使用多個COM port 但共用windows driver 不同的COM port各自有固定號碼(fixed COM port number)

首先插上設備的USB(想要變更的設備)到PC USB port(只要是使用CP21xx IC 都可以), 目的就是要變更裝置的SN號碼使driver 可以分辨在同一個VID/PID下的USB IC, 如此就可以共用同一個電腦下的同一隻driver可以擁有各自獨立的Port number.

. 按原廠指示的確可以完成這樣的訴求:

https://www.cubeatsystems.com/ifx-49/resources/datasheets/AN721.pdf

. 軟件下載地址:

https://www.silabs.com/support/resources.ct-application-notes.ct-example-code.p-interface

AN721: CP210x/CP211x Device Customization Guide	        6.7.5	    Example Code


. 執行Utility變更SN number(其他都不要變更), 操作上一張圖解決了你的疑問:
![快照](CP210x修改SN共用相同driver不同COM號碼不變的方式.jpg)