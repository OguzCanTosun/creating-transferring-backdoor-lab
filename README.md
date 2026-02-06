# Creating a Backdoor – Lab

## Payload Analysis and Selection

In this step, the available payload options were analyzed using the msfvenom tool.
The goal was to identify a suitable payload for a Windows target system.
The selected payload uses a Meterpreter reverse TCP connection, which allows the target system to initiate a connection back to the attacker.
This approach is commonly used in penetration testing due to its effectiveness in bypassing firewall restrictions.

![1](https://github.com/user-attachments/assets/4055ac02-b519-4fbe-bcff-a4bed7944cd8)

## Network Verification

Before creating the payload, the attacker machine’s network configuration was verified.
The IP address of the Kali Linux system was identified to be used as the LHOST parameter.
Ensuring correct network configuration is critical for successful reverse connections in a lab environment.

![2](https://github.com/user-attachments/assets/3932906c-76b2-495b-bd95-473dffb7ffc8)

## Backdoor Payload Creation

After configuring the required parameters, a Windows executable backdoor payload was generated.
This executable is designed to establish a reverse connection to the attacker machine when executed on the target system.
The payload was successfully created using msfvenom without errors.

![3](https://github.com/user-attachments/assets/7aecd17a-c4b4-45a0-8a52-2171a3093b78)

## Output Verification

In the final step, the generated executable file was verified to exist in the local filesystem.
This confirms that the backdoor creation process was completed successfully.
The file is now considered ready for transfer within the controlled lab scenario (theoretical

![4](https://github.com/user-attachments/assets/54f6f2be-022a-4baf-9dd9-1d918ebd6c44)

##Ethical Disclaimer

This project was conducted strictly for educational purposes in a controlled virtual lab environment.
No real systems were targeted, and no unauthorized access was performed.
The purpose of this lab is to understand attacker techniques in order to improve defensive security awareness.
