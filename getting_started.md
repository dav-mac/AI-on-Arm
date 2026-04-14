# **Getting Started**

## **Lab 1: Optimizing Generative AI on Raspberry Pi**

1. **Run the setup script**  
   Open a terminal in the project directory and execute the setup script:  
   ```bash
   ./setup_pi5.sh
   ```
   Please Note: This can take around 30 minutes to complete this step. 

2. **Login to a Hugging Face account**
   ```bash
   huggingface-cli login
   ```
3. **Open the course material**  
   The course material is provided as Jupyter notebooks. To access the content:
   ```bash
   source pi5_env/bin/activate
   jupyter lab
   ```

4. Follow the instructions provided in `lab1.ipynb` to complete the lab.

## **Lab 2: Optimizing Generative AI on Arm Servers**

1. **Launch an AWS EC2 instance**  
   - Go to Amazon EC2 and create a new instance.
   - **Select key pair**: Create a key for SSH connection (e.g., `yourkey.pem`).
   - **Choose an AMI**: Use the `Ubuntu 22.04` AMI as the operating system.
   - **Instance type**: Select `m7g.xlarge` (Graviton-based instance with Arm Neoverse cores).
   - **Storage**: Add 32 GB of root storage.

2. **Connect to the instance via SSH**  
   Use the following command to establish an SSH connection (replace with your instance details):
   ```bash
   ssh -i "yourkey.pem" -L 8888:localhost:8888 ubuntu@<ec2-public-dns>
   ```

3. **Clone the repository**  
   Once connected to the instance, clone the repository:
   ```bash
   git clone https://github.com/arm-university/AI-on-Arm.git
   ```

4. **Run the setup script**  
   Change to the repository directory and run the setup script:
   ```bash
   ./setup_graviton.sh
   ```

5. **Activate the virtual environment and log in to Hugging Face**  
   After the setup completes, activate the virtual environment:
   ```bash
   source graviton_env/bin/activate
   huggingface-cli login
   ```
   (You will need to log in to Hugging Face to download the required large language model.)

6. **Launch the lab**  
   Start Jupyter Lab by running:
   ```bash
   jupyter lab
   ```
   Copy the link provided in the terminal output, open it in your local browser, and follow the instructions in the notebooks.

## **Lab 3: Comparative Inference Benchmarking on Arm Server and Edge Devices**

1. Follow the setup steps for `lab1` on your local Raspberry Pi.
2. Follow the setup steps for `lab2` on your Raspberry Pi, to create and connect to a cloud instance.
3. Open `lab3.ipynb` to find the instructions for completing the lab.
