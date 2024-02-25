# Buliding a SSH Honeypot lab 
<img src="https://github.com/Tripati3000/ssh-honeypotlab/assets/160244601/973e8a91-c640-4d6e-8107-11aa9ee5d01f    " height="80%" width="80%" alt="SIEM System steps"/>

# What is a SSH Honeypot is ?
A SSH honeypot is a security mechanism designed to detect and deflect unauthorized access attempts to a network or server by mimicking a legitimate SSH (Secure Shell) service. It operates by presenting a fake SSH server that appears real to potential attackers, enticing them to interact with it. The honeypot logs all activities, enabling administrators to analyze intrusion attempts, gather information about attackers, and enhance their overall cybersecurity defenses.

# Tools 
# Overview of the tasks
Creating an SSH Endlessh honeypot involves several steps:

1. **Setting up a Linux system**: Start by setting up a Linux system where you'll run the Endlessh honeypot. You can use a virtual machine or a dedicated server for this purpose.

2. **Installing Endlessh**: Clone the Endlessh repository from GitHub or download the source code. Compile it on your Linux system following the instructions provided in the repository's README file.

3. **Configuring Endlessh**: Once compiled, configure Endlessh according to your preferences. This typically involves specifying the port on which Endlessh will listen for incoming connections and adjusting any other settings as needed.

4. **Starting Endlessh**: After configuring Endlessh, start the honeypot service. You can do this by running the Endlessh executable with appropriate command-line arguments or by creating a systemd service unit if you're using a systemd-based Linux distribution.

5. **Monitoring and analyzing logs**: Monitor the logs generated by Endlessh to track incoming connection attempts. Analyze these logs regularly to identify potential attackers and understand their tactics.

6. **Enhancing security**: Consider implementing additional security measures such as firewall rules, intrusion detection systems, and regular software updates to further secure your honeypot environment.

By following these steps, you can set up an SSH Endlessh honeypot to detect and deter potential attackers while gathering valuable insights into their activities.

# Step 1
**Go to your Linux or Virtual machine and copy paste this code.**
`git clone https://github.com/skeeto/endlessh`

**After its done use command** `cd endlessh`
