Router mode
1.	User mode ,    Router>              				 (ดูได้บางอย่าง ,set config อะไรไม่ได้)
2.	Privileged mode,  Router#            			  (ดูได้ทุกอย่าง ,set config อะไรไม่ได้)
3.	Global  configuration mode,  Router(config)#       	 (ดูไม่ได้เลย ,set config ได้ทั้งหมด)



Change mode:           	Router>enable
		  		Router#conf   t		
Router(config)#		

		*** พิมพ์ exit เพื่อย้อนกลับโหมดก่อนหน้า



Set IP address (Example)

Router0>enable
Router0#conf  t
Router0(config)#interface Fa0/0 
Router0(config-if)#ip address 192.168.10.1   255.255.255.0
Router0(config-if)#no shut
Router0(config-if)#interface Fa1/0
Router0(config-if)#ip address 192.168.20.1   255.255.255.0
Router0(config-if)#no shut
Router0(config-if)#int  S2/0
Router0(config-if)#ip address 192.168.20.1   255.255.255.0
Router0(config-if)#no shut
Router0(config-if)#clock rate 128000       (เฉพาะ Serial ที่เป็น DCE จ่ายสัญญาณ นาฬิกา ฝั่งเดียว)

คำสั่ง show
Router0#show run                (show running configuration)
Router0#show ip route       (show ตาราง Routing table)
Router0#show ip interface  brief    (show config ของ interface อย่างละเอีย
Router0#show int  fa0/0	(show interface อย่างละเอียด)

