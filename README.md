<p align="center">
<img src="https://github.com/user-attachments/assets/07a5ebb0-51c9-4de2-8f40-5fb1ffa2ee1b"/>
</p>

<h1>Port Forwarding: Setup and Configuration</h1>
This tutorial outlines the steps required to setup and configure port forwarding on a local network.
<br> This tutorial with also showcase how to port forward on a dual-NAT setup.</br>

<h2>Environments and Technologies Used</h2>

- Chrome (Web Browser for managing Router/Modem)
- Command Prompt (Windows CMD)
- Router Hardware
- Modem Hardware
- Port Forwarding
  
<h2>Operating Systems Used</h2>

- Windows 10 Home</b> 22H2

<h2>Prerequisites</h2>

- Modem and/or Router Username and Password

<h2>Setup Porcedure</h2>

<h3>Step 1: Finding the Default Gateway</h3> 

- To find the Default Gateway, open the Start menu, type “CMD,” and open Command Prompt.
- Once in the Command Prompt, type the command “ipconfig” and press Enter.
- Locate the Network Adapter that is currently in use, and note down the Default Gateway.
  > <img width="50%" height="50%" alt="CMD - ipconfig" src="https://github.com/user-attachments/assets/02734df0-407c-4b6c-a0bf-e559efbbe240" />


  </br>

<h3>Step 2: Opening the Router/Modem Admin Panel</h3>

- To open the Router/Modem Admin Panel, open any web browser, and type the Default Gateway address into the Address Bar at the top of your browser.
- When prompted, enter the login credentials for your router/modem and press Enter.
  > <img width="50%" height="50%" alt="Router - Login" src="https://github.com/user-attachments/assets/b9ca4cc2-efee-4cfa-99a7-70f562074957" />

</br>

<h3>Step 3: Locating Port Forwarding For Your Router/Modem</h3>

- Every router/modem has a different layout, so finding port forwarding isn’t something that can be directly guided to in a generalized tutorial like this.
- Common places where port forwarding can be found include: advanced, administration, firewall, or security.
- Once you’ve found the Port Forwarding tab, enter it.
  > <img width="50%" height="50%" alt="Router - Port Forwarding Tab" src="https://github.com/user-attachments/assets/f9113343-6496-48e6-9262-b80133ec1a6d" />



</br>

<h3>Step  4: Service Rule Configuration</h3>

- Depending on your router/modem, you may need to click a button before you can input a service rule.
- Title the rule an appropriate name.
- Pick the protocol(s) for your desired service.
- Pick the internal port(s) for your desired service.
- Pick the external port(s) for your desired service.
- Select or input the IPv4 address of the device on which the service resides.
- Once done, click “Apply.”
  > <img width="50%" height="50%" alt="Router - Service Configuration" src="https://github.com/user-attachments/assets/d3592e78-6ee0-4d96-82cc-f57971e676e3" />



</br>

<h3>You have successfully made a port forward rule on your router/modem.</h3>

<br><h3>If you’re running a dual-NAT setup, you aren’t finished yet.</h3></br>

<h3>Step 5: Finding Your Other Default Gateway</h3>

- If you are running a dual-NAT setup, you will need to find the other Default Gateway on your network.
- To find the other Default Gateway, open Command Prompt again.
- In CMD, input the command “tracert 8.8.8.8” and press Enter.
- The first two lines of the trace indicate the two Default Gateways on a dual-NAT setup.
- Note down the other Default Gateway.
  > <img width="50%" height="50%" alt="CMD - tracert" src="https://github.com/user-attachments/assets/93de4eeb-49f1-44c0-8941-9e47c1681812" />


  </br>

<h3>Step 6: Port Forwarding on the Second Gateway</h3>

- Using the new Default Gateway, follow steps 2-4 again, inputting all of the same service rule configurations as the first gateway.
  > <img width="50%" height="50%" alt="Modem - Login" src="https://github.com/user-attachments/assets/26c8abc6-e7d7-4caf-82ef-ef40c8cb836c" />

  > <img width="50%" height="50%" alt="Modem - Port Forwarding" src="https://github.com/user-attachments/assets/f92079a6-14ce-481b-87b6-fd6e8afbed0f" />




</br>

<h3>Congrats! You’ve set up Port Forwarding on a dual-NAT network.</h3>
<img width="50%" height="50%" alt="Port_Forward_List" src="https://github.com/user-attachments/assets/132f4cd1-ba3a-4cb1-a531-409b8121cce2" />

