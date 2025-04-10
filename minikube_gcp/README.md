# kubernete-shell
#### Overview
This shell script sets up a Kubernetes Master node on a physical machine running Ubuntu 22.04 LTS. It installs all required dependencies, configures the system, and initializes a Kubernetes cluster.

#### How to Use
1. **Download the Script**
   - Save the script as `minikube.sh`.

2. **Make it Executable**
   - Run this command:
     ```
     chmod +x minikube.sh
     ```

3. **Run the Script**
   - Execute it with `sudo`:
     ```
     sudo ./minikube.sh
     ```
   - Follow the prompts to confirm or enter the Master node IP.

4. **Check the Results**
   - After completion, check the cluster status:
     ```
     kubectl get nodes
     ```
   - View the log file if there are issues:
     ```
     cat kubeadm_init.log
     ```
   - Find the Worker node join command:
     ```
     cat k8s-join-command.txt
     ```

#### Troubleshooting
- If the IP detection fails, manually enter the correct IP when prompted.
- For hardware errors, ensure your machine meets the minimum requirements.

---
