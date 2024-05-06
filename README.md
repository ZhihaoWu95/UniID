# Pytoch implementation of "UniID: Spoofing Face Authentication with Universal Identity" (NDSS 2024)

## What is UniID?
Face authentication systems are widely employed in access control systems to ensure the security of confidential facilities. Recent works have demonstrated their vulnerabilities to adversarial attacks. However, such attacks typically require adversaries to wear disguises such as glasses or hats during every authentication, which may raise suspicion and reduce their attack impacts.
In this work, we propose **the UniID attack**, which allows multiple adversaries to perform face spoofing attacks without any additional disguise by enabling an insider to register a universal identity into the face authentication database by wearing an adversarial patch.
To achieve it, we first select appropriate adversaries through feature engineering, then generate the desired adversarial patch with a multi-target joint-optimization approach, and finally overcome practical challenges such as improving the transferability of the adversarial patch towards black-box systems and enhancing its robustness in the physical world.
We implement UniID in laboratory setups and evaluate its effectiveness with six face recognition models (FaceNet, Mobile-FaceNet, ArcFace-18/50, and MagFace-18/50) and two commercial face authentication systems (ArcSoft and Face++). 
Simulation and real-world experimental results demonstrate that UniID can achieve a max attack success rate of $100\%$ and $79\%$ in 3-user scenarios under the white-box setting and black-box setting respectively, and it can be extended to more than 8 users.

Details of algorithms and experimental results can be found in our paper: [UniID: Spoofing Face Authentication with Universal Identity](https://www.ndss-symposium.org/wp-content/uploads/2024-1036-paper.pdf)

**Please CITE** our paper whenever this repository is used to help produce published results or incorporated into other software.
