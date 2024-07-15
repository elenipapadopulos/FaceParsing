# Facing Face Parsing: U-Net and variations on LaPa dataset

Face parsing, the task of segmenting a human face into its constituent parts by predicting per-pixel semantic labels, is foundational for numerous computer vision applications, including biometric authentication, surveillance, and augmented reality. Unique challenges in face parsing involve highly restricted input images and ambiguous boundaries between facial components. We have trained from scratch four U-Net based models for face parsing, including a baseline U-Net, Residual U-Net (RESUNet), depthwise Separable Residual U-Net  (SRUNet), and a conditional Generative Adversarial Network (cGAN) using U-Net as the generator.

The models were evaluated on the LaPa dataset, which consists of over 22,000 images with pixel-level annotations for 11 facial categories. Due to computational constraints, a subset of 1,620 images was used for training, validation, and testing, augmented through random rotations, horizontal flips, and other techniques.
Performance metrics included Pixel Accuracy, mIoU, and Dice coefficient.

The cGAN model achieved the highest mean IoU and Dice coefficient, indicating superior segmentation performance. Overall, the cGAN with U-Net as the generator demonstrated the best balance of computational efficiency and segmentation accuracy among the proposed architectures, substantiating its potential for real-world face parsing applications.
