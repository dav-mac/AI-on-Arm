# **Optimizing Generative AI on Arm Processors**

![learn_on_arm](./img/Learn%20on%20Arm_banner.png)

## Course overview
Welcome to **Optimizing Generative AI on Arm Processors**, a hands-on course designed to help you optimize generative AI workloads on Arm architectures. Through practical labs and structured lectures, you will learn how to deploy AI models efficiently across different Arm-based environments.

## Who is this for?
This course is designed for intermediate machine learning practitioners who want to bridge the gap between model design and deployment efficiency. Rather than revisiting ML fundamentals, you will dive straight into performance engineering for generative AI on Arm-based platforms, including edge and cloud environments.

The course is suitable for learners with a foundational understanding of machine learning and some familiarity with Python-based AI workflows, Jupyter notebooks, and command-line tools.

## What will you learn?
By the end of this course, you will have a strong foundation in deploying high-performance AI models on Arm hardware.

You will learn how to optimize AI inference using Arm-specific techniques such as SIMD (SVE, Neon) and low-bit quantization. The course covers practical strategies for running generative AI efficiently on mobile, Edge, and Cloud-based Arm platforms. You will also explore the trade-offs between cloud and edge deployment, gaining both theoretical knowledge and hands-on skills.

## Prerequisites
### Knowledge and skills
This course assumes a foundational understanding of machine learning, including completion of a basic introductory course, such as one at the undergraduate level.
### Hardware and software
To run the laboratory exercises, you will need to have access to a Raspberry Pi 5 and an Arm-based cloud instance. We have validated this on an AWS Graviton instance but it is expected to work through other cloud service providers.

## Course structure
This course consists of three hands-on labs and four lectures.

### Hands-on labs
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

---

## 🚀 Start here

> **New to this course? Do this:**
>
> Clone this repo, then follow the setup guide to get your environment ready and launch your first lab:
>
> 👉 [getting_started.md](https://github.com/dav-mac/AI-on-Arm/blob/main/getting_started.md)

---

# Additional notes

## Don't forget
- After completing Labs 2 and 3, remember to terminate the EC2 instance to avoid unnecessary charges.

## Special thanks
**✍️ Primary Author:** AI researcher, [Oliver Grainge](https://github.com/OliverGrainge).

## License
You are free to fork or clone this material. See `LICENSE.md` for the complete license.

## Inclusive language commitment
Arm is committed to making the language we use inclusive, meaningful, and respectful. Our goal is to remove and replace non-inclusive language from our vocabulary to reflect our values and represent our global ecosystem.
 
Arm is working actively with our partners, standards bodies, and the wider ecosystem to adopt a consistent approach to the use of inclusive language and to eradicate and replace offensive terms. We recognise that this will take time. This course may contain references to non-inclusive language; it will be updated with newer terms as those terms are agreed and ratified with the wider community. 
 
Contact us at education@arm.com with questions or comments about this course. You can also report non-inclusive and offensive terminology usage in Arm content at terms@arm.com.
