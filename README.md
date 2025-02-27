# HOWTO: Create a Blinking LED application project for S32K344 using S32 RTD AUTOSAR By KOUKI FEDI

Here will be a detailed guide to make a blinking LED from scratch 

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











