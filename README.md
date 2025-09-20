# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date: 20-09-2025
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>
<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/813813a7-5719-4b01-b7f2-699e7f7dd915" />
<img width="1918" height="1016" alt="Screenshot 2025-09-20 133702" src="https://github.com/user-attachments/assets/a8a37210-cd96-400f-85e3-9e8fd2922d8b" />
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/802ae412-a655-4fb4-8c61-dd9533aa0bae" />
<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/90066d20-93de-4e2d-bc4c-4736ff597c83" />



•	PDU details for remote communication<br>
<img width="1919" height="1015" alt="Screenshot 2025-09-20 132707" src="https://github.com/user-attachments/assets/96511e05-f264-49ce-a4a4-e5ce3f7affb0" />
<img width="1919" height="1016" alt="Screenshot 2025-09-20 132722" src="https://github.com/user-attachments/assets/3f6c2589-6572-4921-981c-4ebbb42297df" />
<img width="1918" height="1018" alt="Screenshot 2025-09-20 132825" src="https://github.com/user-attachments/assets/265e65ce-d118-4a11-b116-27a47734e055" />
<img width="1919" height="1014" alt="Screenshot 2025-09-20 132844" src="https://github.com/user-attachments/assets/0920ca1b-5c3c-4c02-9554-0c6913e8fee2" />
<img width="1919" height="1020" alt="Screenshot 2025-09-20 132859" src="https://github.com/user-attachments/assets/c368af40-1072-4396-9eb0-625ec6d0b4f8" />
<img width="1919" height="1018" alt="Screenshot 2025-09-20 132917" src="https://github.com/user-attachments/assets/aef07f6a-ddf1-4198-9bfa-054c2ec58ce6" />

•	Tables showing MAC/IP changes through each device<br>

<img width="532" height="132" alt="Screenshot 2025-09-20 133134" src="https://github.com/user-attachments/assets/666284e1-27ca-490f-b26d-5785573d2d72" />
<img width="615" height="133" alt="Screenshot 2025-09-20 133102" src="https://github.com/user-attachments/assets/51fb0547-3c35-471e-bf51-8fe84bd205ac" />

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

