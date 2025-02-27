# HOWTO: Create a Blinking LED application project for S32K344 using S32 RTD AUTOSAR By KOUKI FEDI

Here will be a detailed guide to make a blinking LED from scratch on S32K344EVB-T172

![image](https://github.com/user-attachments/assets/6acd5aba-1832-4a7a-8d15-a5c31e6a6190)


# Installing S32 Design studio 

1. You will find the link for S32 studio here : [Download](https://nxp.flexnetoperations.com/control/frse/download?element=6443311)

![image](https://github.com/user-attachments/assets/eb6be968-e634-420c-b944-6c2d02ffe351)

2. Press **I Agree**

![image](https://github.com/user-attachments/assets/1d76db8c-8c7f-471f-a38b-1d5e21f811be)

3. Download **S32DS_3.6.0_win32.x86_64.exe**

4.  Before Runnig the installation Press : **Windows+R** then Search for **`services.msc`**

![image](https://github.com/user-attachments/assets/de7e86a6-984e-4907-84c1-1f2d076bd435)

5.  Search for **Server** (**Serveur**)

![image](https://github.com/user-attachments/assets/c97247e8-4237-4586-8820-cbd9a613160b)

6.  Right CLick on Server -> Properties ( Propriétés ) 

![image](https://github.com/user-attachments/assets/f5d7539d-c6f3-4ff5-8d88-a9d766396203)

7.  Startup Type (Type de démarage) : 

![image](https://github.com/user-attachments/assets/2f8bf993-993f-4feb-ab1b-eeefb698b55c)


8.  Know go and Run **S32DS_3.6.0_win32.x86_64.exe**
9.  If Everything work properly you will get this window after launching s32 studio 

![image](https://github.com/user-attachments/assets/9235db9d-06c3-4013-8a21-c912bcd8c03b)


# Preparing The s32 Studio 

We need to install some packages on S32 Studio 

1. Go to **HELP**
2. Go to **S32ds Extensions and Update**

![image](https://github.com/user-attachments/assets/fb5a5700-fb34-47dc-b67a-a9712648732e)

![image](https://github.com/user-attachments/assets/3d6e33ae-c8f1-4ab6-91a2-2abb89a7304c)

3. For **S32K3XX Real-TimeDrivers AUTOSAR R21-11 Version 5.0.0 Package** You need to add it mannualy 
4. Go to RTD NXP from this link : [**Automotive SW - S32K3/S32M27x - Real-Time Drivers for Cortex-M**](https://nxp.flexnetoperations.com/control/frse/product?child_plneID=830617)
5. Download **SW32K3_S32M27x_RTD_4.4_4.0.0_P24_D2405.exe** and **SW32K3_S32M27x_RTD_4.4_4.0.0_P24_DS_updatesite_D2405.zip**

![image](https://github.com/user-attachments/assets/352f8474-67ee-4d0a-8c47-f8cdd5282cec)


6. IF In the installation you need the License that you can find under **License Keys Panel**

![image](https://github.com/user-attachments/assets/c8100911-ff75-4bff-a532-ebe257f06a76)


7. Then GO S32 Studio and in **S32ds Extensions and Update** Press **Add Update Sites**

![image](https://github.com/user-attachments/assets/adc11261-c009-4aeb-b70b-b17601e8b205)

8. Ten look for **SW32K3_S32M27x_RTD_4.4_4.0.0_P24_DS_updatesite_D2405.zip**
9. Finally the **S32K3XX Real-TimeDrivers AUTOSAR R21-11 Version 5.0.0 Package**  Should appear

## Let's Start Our application 

1. Open S32 Design Studio
2. Go to **File** > **New** > **S32DS Project From Example**

![image](https://github.com/user-attachments/assets/6cbb2070-c3a6-4b81-8e58-4a26fb797d41)

3. This window should appear

![image](https://github.com/user-attachments/assets/cb4a5a7f-87b7-466a-8166-5c0bee836cbb)

4. Look for **Port_Example**

![image](https://github.com/user-attachments/assets/29150ccf-e53d-4298-bb70-42c3d16db08a)

5. Open `**.mex file**`

![image](https://github.com/user-attachments/assets/a68d8404-327f-4403-8a38-ced2f7d72855)

![image](https://github.com/user-attachments/assets/71b89a6b-622f-4702-a424-6c3cd62bcefc)


6. We need now to specify our Board , Go to  **Window > Show View > Package**

![image](https://github.com/user-attachments/assets/fef1f4af-f68f-48dc-8bfe-cbafafffb362)

7. this window should appear

![image](https://github.com/user-attachments/assets/6670eede-4477-43e8-b657-9986269c6ae7)


8. Go to **Switch Package**

![image](https://github.com/user-attachments/assets/fa5cc95b-caf1-41c8-943d-03f7d1bc5ebf)

### Select the S32K344_172HDQFP - HDFQP 172 package  because we are working with this board 

![image](https://github.com/user-attachments/assets/0106d0e6-9ad8-4565-8020-6f80abebcafe)

![image](https://github.com/user-attachments/assets/33688cbe-a686-49f2-a88d-d092a7dd0afe)

![image](https://github.com/user-attachments/assets/75a1b9d8-599c-4611-bcf9-4f9fe6109758)

## Let's Build this Code 

1. First, **Update the Code**

![image](https://github.com/user-attachments/assets/ee83ca6c-e3f1-4a18-90a3-d29cc843a60f)

2. If every thing is OK, you should have a **GRAY Icon** on **Update Code** and **0 Problem** in **Problems Panel**

![image](https://github.com/user-attachments/assets/d5173709-a6c3-479b-aa7a-36ea1cda7b95)


3. Now We should Go to **Resource**, If the icon is not already existed
follow this steps 

![image](https://github.com/user-attachments/assets/5c1064f8-846f-452a-9009-dc0c36296ae5)

### Select Resource and Click open 

![image](https://github.com/user-attachments/assets/fdec6e82-6b55-4ace-9337-2f6f698d923e)

4. You should get somthing like this 

![image](https://github.com/user-attachments/assets/a247fb9a-d3a8-49b8-bc87-ddc74b86e90c)


5. Right click On the **project name** in **Project Explorer Panel** then **Build Project**

![image](https://github.com/user-attachments/assets/eb6bba11-ae93-4f01-9332-e6c8e8db33e4)


6. If Everything is Ok 

![image](https://github.com/user-attachments/assets/f50faa4c-cd22-42a8-9203-e19cd73c7daf)

### A Debug_FLASH Should be Created 

![image](https://github.com/user-attachments/assets/ff12852a-c893-40b3-9810-5142c39a3fa3)

7. Now Let's prepare for debug
8. Connect the USB to **S32K3x4EVB**  

![image1](https://github.com/user-attachments/assets/0bbbaf5f-5b98-4d71-8227-2ff2367153e3)

9. **Right Click** on the project 

![image](https://github.com/user-attachments/assets/237adac7-ce57-4c37-acdb-76ef8953bf86)

![image](https://github.com/user-attachments/assets/792cf090-a4eb-4f21-924f-ea4705306ac4)

10. Then Press **Debug** This error should appear

![image](https://github.com/user-attachments/assets/bb4017a1-7d89-449f-888d-dfefd22c0c07)


11. Plug the **External power Supply ( 12 V , >= 2.0 A )** to the Evaluation Board 

![image2](https://github.com/user-attachments/assets/f51106db-5b90-497f-a197-023899125da6)

12. Turn on the Switcher Like this 

![image](https://github.com/user-attachments/assets/3e97b927-ab6e-4d93-b318-8b21c0f6cab6)

13. The LED on TOP RIGHT Corner should be ON 

 ![image3](https://github.com/user-attachments/assets/92412944-db87-4e7e-a632-8ddd6f8c5156)

14. Redebug the project  

![image](https://github.com/user-attachments/assets/c0101157-4674-4bf1-ad9c-43a63e601400)


![image](https://github.com/user-attachments/assets/73c71a08-2289-4f34-aa84-d2afdc5aa13d)

15. you can try for example Run ( The RED LED Will blink 10 Times ) 

![image](https://github.com/user-attachments/assets/5f9f13af-7673-4a0b-b94f-2a9089e316c2)

![image](https://github.com/user-attachments/assets/cf949a75-f2e4-4d44-ad9f-729f40ff717b)

![image](https://github.com/user-attachments/assets/1bca246b-fa4a-436e-8062-3746f55d0e92)


https://github.com/user-attachments/assets/03ce6c31-20da-44f4-97b9-31346889f6bc

## Let's Toggle The Blue & Green Led Together

before we started we have some necessary docs : 

1. [S32K3X4EVB-T172_Hardware User Manuel ](https://github.com/user-attachments/files/19009350/S32K3X4EVB-T172_PackRevB2_HW_User.Manual.pdf)
2. [S32K3X4EVB-T172_Schematic ](https://github.com/user-attachments/files/19009368/S32K3X4EVB-T172_PackRevB2_Schematic.pdf)

## S32K344 PORTA PINOUT : 

![image](https://github.com/user-attachments/assets/816e9c4d-913d-4cb6-ad34-efd10a11a3a2)

## S32K344 PORTB PINOUT :

![image](https://github.com/user-attachments/assets/6702fee6-8485-4512-b784-b65eb0712022)

## S32K344 PORTC PINOUT :

![image](https://github.com/user-attachments/assets/503ca0da-dccf-4ed3-8ca9-30e888897fee)


## S32K344 PORTD PINOUT :

![image](https://github.com/user-attachments/assets/db58ee34-4ea9-4337-b29e-0889b400a67d)


## S32K344 PORTE PINOUT :

![image](https://github.com/user-attachments/assets/340e0e8c-783d-4d59-867e-59adf2bb3aa4)

## Default Configuration 

![image](https://github.com/user-attachments/assets/f68fa0d5-9aa2-4ead-8ef9-1c2e84ebe6d0)

Let's Start : 

1. we are Going to use PTA30 and PTA31

![image](https://github.com/user-attachments/assets/531b27f7-039f-4258-a684-a7f5935009f4)


2. Open **example_Port.mex** and then **Routing Detail**

![image](https://github.com/user-attachments/assets/e6ac8e75-ec3c-4553-82c6-1cca317c856d)

### If routing Details is not in your workspace follow this steps 

![image](https://github.com/user-attachments/assets/6417f412-dc78-4334-b42e-c1cd5a942472)

3. Add New Row

![image](https://github.com/user-attachments/assets/b9ed6301-a53e-4673-ac49-2c0b3f4e8385)


4. For **Routed pin : PTA30**

![image](https://github.com/user-attachments/assets/f2f1aa07-a5fb-48bd-aecb-445f0222e99a)


5. For **Signal : GPIO 30** 

You can Find it by holding the cursor on the top of PTA30  

![image](https://github.com/user-attachments/assets/1c49edd2-85aa-4cf0-8993-6d22acab8d71)

6. For **Peripheral : SIUL2** and **Direction : INPUT/OUTPUT**

![image](https://github.com/user-attachments/assets/60854579-a252-4b1a-9130-130d3e5cfd57)


7. Open **Components Panel**



8. 

