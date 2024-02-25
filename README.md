se# Buliding a SSH Honeypot lab 
<img src="https://github.com/Tripati3000/ssh-honeypotlab/assets/160244601/973e8a91-c640-4d6e-8107-11aa9ee5d01f    " height="80%" width="80%" alt="SIEM System steps"/>

# What is a SSH Honeypot ?
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

1. **After its done use command** `cd endlessh`

2. **After changing directory Use the command** `make`

3. **Install the sudo package** `sudo apt install libc6-dev`

4. **Move the folder to usr/local/bin** `sudo mv endlessh /usr/local/bin/`

5. **Verify your folder by this command** `which endlessh` & `ls`

6. **After Verification of folder Run this command to copy the file to another folder**

              `sudo cp util/endlessh.service /etc/systemd/system`
 
 <img src="https://github.com/Tripati3000/ssh-honeypotlab/assets/160244601/26d97806-44a5-47be-9da1-b355243f1c5a" height="80%" width="80%" alt="SIEM System steps"/>

7. **Enable the systemd server**
 
                 `sudo systemctl enable endlessh`

8. **Create a configuration file**

                 `mkdir -p /etc/endlessh`

 9. **Create a folder in etc/endlessh/config**

                 `sudo nvim /etc/endlessh/config`
