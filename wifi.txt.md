 

 	// This codes works on showing wifi pass on your own laptop or maybe Pc





 

 	 - step 1: Run CMD as an Administrator



 	 - Step 2: Types the command to show all wifi

 

#    **( netsh wlan show profile )**



\*\*//\*\* The code in step 2 only shows the available wifi on your laptop










 	- Step 3: Type this command in your terminal to download the wifi information





# **( netsh wlan export profile folder=C:\\ key=clear )**





\*\*// After that command all the wifi will be downloaded in the C drive then open it as a Notepad to see the pass\*\*



	\*\*// Example of the wifi with xml code\*\*




	<?xml version="1.0"?>


<WLANProfile xmlns="http://www.microsoft.com/networking/WLAN/profile/v1">

 	<name><!\[CDATA\[EMMA WI-FI ]]></name>

 	<SSIDConfig>

 		<SSID>

 			<hex>454D4D412057492D464920</hex>

 			<name>EMMA WI-FI </name>

 		</SSID>

 	</SSIDConfig>

 	<connectionType>ESS</connectionType>

 	<connectionMode>auto</connectionMode>

 	<MSM>

 		<security>

 			<authEncryption>

 				<authentication>WPA3SAE</authentication>

 				<encryption>AES</encryption>

 				<useOneX>false</useOneX>

 				<transitionMode xmlns="http://www.microsoft.com/networking/WLAN/profile/v4">true</transitionMode>

 			</authEncryption>

 			<sharedKey>

 				<keyType>passPhrase</keyType>

 				<protected>false</protected>

 				// The wifi password

 				**<keyMaterial>00012669</keyMaterial>**

 			</sharedKey>

 		</security>

 	</MSM>

 	<MacRandomization xmlns="http://www.microsoft.com/networking/WLAN/profile/v3">

 		<enableRandomization>false</enableRandomization>

 		<randomizationSeed>3112956689</randomizationSeed>

 	</MacRandomization>

</WLANProfile>













 

