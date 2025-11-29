### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow
    
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. Click on the add gateway 
 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. Click on the lora options , lora - frequency plan 

5. Click on channels and create a new channel after which you can add a new end device
   
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)

6. Add the attributes in the end device as  shown below 

 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
 
7.Using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT :
<img width="1901" height="1146" alt="Screenshot 2025-11-29 212504" src="https://github.com/user-attachments/assets/69309f84-94b0-4478-b396-99bcc857a3b7" />

<img width="1920" height="1200" alt="Screenshot (2)" src="https://github.com/user-attachments/assets/930d8480-187c-467e-8807-36b5ed44a5dc" />

<img width="1915" height="1087" alt="image" src="https://github.com/user-attachments/assets/ff357cee-9285-40f5-a3b7-e0c5de6c7399" />


<img width="1920" height="1200" alt="Screenshot (5)" src="https://github.com/user-attachments/assets/1e03a12e-9f11-4844-89c0-7e472c5d0d48" />

<img width="1920" height="1200" alt="Screenshot (6)" src="https://github.com/user-attachments/assets/12d33d40-500f-4c9a-9f90-d7e6f31fb2da" />


<img width="1919" height="1199" alt="Screenshot 2025-11-29 102138" src="https://github.com/user-attachments/assets/36d6833b-b6aa-4e9e-b491-d9d296a64970" />

<img width="1912" height="1199" alt="Screenshot 2025-11-29 102158" src="https://github.com/user-attachments/assets/27152e33-3967-4d86-af58-bb908e50a999" />

<img width="1919" height="1197" alt="Screenshot 2025-11-29 102219" src="https://github.com/user-attachments/assets/2ea8c596-9939-4466-8f2b-dc37aaa48259" />

<img width="1919" height="1199" alt="Screenshot 2025-11-29 102238" src="https://github.com/user-attachments/assets/8692a8c3-b12b-4d66-a227-1e94fb250837" />


<img width="1918" height="1145" alt="Screenshot 2025-11-29 102306" src="https://github.com/user-attachments/assets/8cfed862-003e-4b45-9aca-ea6a93cca31e" />

<img width="1901" height="1159" alt="Screenshot 2025-11-29 102353" src="https://github.com/user-attachments/assets/afcb7692-2a47-44e5-af92-e03ad222779a" />

<img width="1919" height="1199" alt="Screenshot 2025-11-29 102459" src="https://github.com/user-attachments/assets/4460335e-d690-4ca3-83d8-f0cc0f64e671" />


<img width="1919" height="1174" alt="Screenshot 2025-11-29 102556" src="https://github.com/user-attachments/assets/5671db20-3a61-480a-a0ad-b03db309029d" />

<img width="1911" height="1198" alt="Screenshot 2025-11-29 102640" src="https://github.com/user-attachments/assets/0b26a409-d8a0-4249-95cd-efd4a38cf0fa" />

<img width="1915" height="1199" alt="Screenshot 2025-11-29 102700" src="https://github.com/user-attachments/assets/24760609-4c18-4585-a510-69423df4e7df" />

## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
