Project Title:
Prostate Cancer Detection Using EfficientNetB3 with Augmented and Synthetic MRI Images (T2 and DWI Modalities)
📖 Project Summary:
This project applies deep learning techniques for classifying prostate cancer using MRI scans. Leveraging EfficientNetB3, a state-of-the-art convolutional neural network, the model is trained on both real and synthetically generated grayscale T2-weighted and DWI (Diffusion-Weighted Imaging) scans. The use of synthetic data helps enhance model generalization and overcome limited dataset constraints often present in medical imaging applications.
🎯 Objectives:
    Classify prostate cancer presence from MRI images (T2-weighted and DWI).
    Improve model accuracy using synthetic image generation and data augmentation.
    Leverage EfficientNetB3 for high performance with fewer training epochs.
📂 Dataset:
    Real MRI images (T2 and DWI formats).
    Synthetic grayscale MRI images generated using prompt-based diffusion methods to simulate tumor and healthy cases.
🛠️ Key Components of the Code:
    Image preprocessing: resizing, normalization, grayscale handling.
    Data augmentation: flipping, rotation, brightness, zoom.
    CNN model: EfficientNetB3 with fine-tuning.
    Training-validation-test splitting.
    Performance metrics: Accuracy, Loss, Confusion Matrix.
📌 How to Use:
    Place your dataset folders under the directory ./data/ with subfolders:
        ./data/train/
        ./data/validation/
        ./data/test/ Each subfolder should contain T2 and DWI formatted images labeled accordingly.
    Run the notebook cells sequentially:
        Load and preprocess image data
        Define and compile EfficientNetB3 model
        Train the model using model.fit()
        Evaluate model performance on test data
    For synthetic data:
        Make sure generated images are added to the appropriate class folder during training.
        You can extend the dataset using the previously generated synthetic MRI images.
📈 Expected Outcomes:
    Trained classifier capable of identifying prostate cancer features from MRI scans.
    Accuracy improvement from additional synthetic images.
    Visualization of learning curves and confusion matrices.
📌 Applications:
    Assisting radiologists in detecting prostate cancer
    Medical imaging research
    Automated clinical decision support systems


Generation Method Used
The method used was:
    OpenAI's image generation model (via prompt-based synthesis) which learned patterns from large datasets including medical-like imaging.
    Prompt: "A grayscale MRI (Magnetic Resonance Imaging) scan showing symmetrical brain or pelvic structures with soft tissue contrast in axial view, dark muscle layers and central soft tissue mass, 256x256 resolution, medical scan texture."
This prompt ensured:
    Anatomical symmetry
    Soft tissue gradients and signal intensity variation
    Monochrome MRI-style output suitable for AI model augmentation
🛠 Use in AI Training
The generated image can be used for:
    Data augmentation in small medical datasets
    Pretraining or fine-tuning models to increase robustness
    Creating synthetic validation or test sets
