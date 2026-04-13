# **Optimizing Generative AI on Arm Processors**

![learn_on_arm](./img/Learn%20on%20Arm_banner.png)

## Course Overview
Welcome to **Optimizing Generative AI on Arm Processors**, a hands-on course designed to help you optimize generative AI workloads on Arm architectures. Through practical labs and structured lectures, you will learn how to deploy AI models efficiently across different Arm-based environments.

## Intended Audience
This course is designed for developers, ML engineers, and technically confident students who want practical experience deploying and optimizing generative AI workloads on Arm platforms. It is best suited to learners with a foundational understanding of machine learning and some familiarity with Python-based AI workflows, Jupyter notebooks, and command-line tools.

The course is particularly relevant for those interested in running AI inference efficiently across edge and cloud environments, including devices such as Raspberry Pi 5 and Arm-based cloud servers.

## What You'll Learn
By the end of this course, you will have a strong foundation in deploying high-performance AI models on Arm hardware.

You will learn how to optimize AI inference using Arm-specific techniques such as SIMD (SVE, Neon) and low-bit quantization. The course covers practical strategies for running generative AI efficiently on mobile, Edge, and Cloud-based Arm platforms. You will also explore the trade-offs between cloud and edge deployment, gaining both theoretical knowledge and hands-on skills.

## Course Structure
This course consists of three hands-on labs and four lectures.

### Hands-On Labs
| Part  | File       | Focus                                                                      |
|-------|------------|----------------------------------------------------------------------------|
| Lab 1 | [lab1.ipynb](https://github.com/arm-education/AI-on-Arm/blob/main/lab1.ipynb) | Optimizing generative AI on mobile devices, such as the Raspberry Pi 5.    |
| Lab 2 | [lab2.ipynb](https://github.com/arm-education/AI-on-Arm/blob/main/lab2.ipynb) | Deploying AI workloads on Arm-based cloud servers, including AWS Graviton. |
| Lab 3 | [lab3.ipynb](https://github.com/arm-education/AI-on-Arm/blob/main/lab3.ipynb) | Comparing Cloud vs. Edge inference, analyzing challenges and trade-offs.   |


### Lectures
Inside the `slides/` folder, you will find four lectures covering the key concepts and challenges in AI inference on Arm:

| Part      | Title                                                | File          | Focus                                                                                                 |
|-----------|------------------------------------------------------|---------------|-------------------------------------------------------------------------------------------------------|
| Lecture 1 | **Challenges Facing Cloud and Edge GenAI Inference** | [chapter1.pptx](https://github.com/arm-education/AI-on-Arm/blob/main/slides/chapter1.pptx) | Understanding the limitations and constraints of AI inference in different environments.              |
| Lecture 2 | **Generative AI Models**                             | [chapter2.pptx](https://github.com/arm-education/AI-on-Arm/blob/main/slides/chapter2.pptx) | Exploring model architectures, training methodologies, and deployment considerations.                 |
| Lecture 3 | **ML Frameworks and Optimized Libraries**            | [chapter3.pptx](https://github.com/arm-education/AI-on-Arm/blob/main/slides/chapter3.pptx) | A deep dive into AI software stacks, including PyTorch, ONNX Runtime, and Arm-specific optimizations. |
| Lecture 4 | **Optimization for CPU Inference**                   | [chapter4.pptx](https://github.com/arm-education/AI-on-Arm/blob/main/slides/chapter4.pptx) | Techniques such as quantization, pruning, and leveraging SIMD instructions for faster AI performance. |

## Pre-requisites
### Knowledge and Skills
This course assumes a foundational understanding of machine learning, including completion of a basic introductory course, such as one at the undergraduate level.
### Hardware and Software
To run the laboratory exercises, you will need to have access to a Raspberry Pi 5 and an Arm-based cloud instance. We have validated this on an AWS Graviton instance but it is expected to work through other cloud service providers. 

## **Additional Notes**
- For Lab 2 and 3 make sure to terminate the EC2 instance when you're done to avoid unnecessary charges.

## Special Thanks
* **✍️ Primary Author:** AI researcher, [Oliver Grainge](https://github.com/OliverGrainge)
---

# **Getting Started**
### **Lab 1: Optimizing Generative AI on Raspberry Pi**

1. **Run the setup script**  
   Open a terminal in the project directory and execute the setup script:  
   ```bash
   ./setup_pi5.sh
   ```
   Please Note: It can take around 30 minutes to complete this step. 

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

### **Lab 2: Optimizing Generative AI on Arm Servers**

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

### **Lab 3: Comparative Inference Benchmarking on Arm Server and Edge Devices**

1. Follow the setup stpes for `lab1` on your local Raspberry Pi.
2. Follow the setup stpes for `lab2` on your Raspberry Pi, to create and connect to a cloud instance.
3. Open `lab3.ipynb` to find the instructions for completing the lab 



