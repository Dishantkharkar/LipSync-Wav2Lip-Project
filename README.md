# LipSync-Wav2Lip-Project

This repository contains code for lip synchronization using Wav2Lip, a deep learning-based model.

## How to Use this Code for Lip Synchronization

### **Step 1: Clone the Repository**

```bash
git clone https://github.com/Dishantkharkar/LipSync-Wav2Lip-Project.git
cd LipSync-Wav2Lip-Project
```

### **Step 2: Install Requirements**

```bash
pip install -r requirements.txt
```

### **Step 3: Download Pretrained Model**

Download the pretrained model from [s3fd.pth](https://github.com/Rudrabha/Wav2Lip/releases/download/weights/sfd.pth) and save it in the `face_detection/detection/sfd/` folder.

### **Step 4: Obtain Additional Weights**

Navigate to the [official Wav2Lip repository](https://github.com/Rudrabha/Wav2Lip) and follow the instructions in the README to obtain additional weights.

### **Step 5: Add Video and Audio**

Place your video and audio files in the folder shown below:
![Folder Structure](https://github.com/Dishantkharkar/LipSync-Wav2Lip-Project/assets/130529528/10ff2c29-7621-4f2e-a987-e51cfe76bd44)

### **Step 6: Lip Synchronization**

Run the following command to perform lip synchronization:

```bash
python inference.py --checkpoint_path <path_to_pretrained_model> --face <path_to_face_video> --audio <path_to_audio_file>
```

Replace `<path_to_pretrained_model>`, `<path_to_face_video>`, and `<path_to_audio_file>` with the appropriate paths.

Example using `newscript.txt` file:

![Example](https://github.com/Dishantkharkar/LipSync-Wav2Lip-Project/assets/130529528/c9142f3f-96a2-4edb-8b58-c59cf1398224)


The result will be stored in the `Result` folder with the name `result_audio`. 
![image](https://github.com/Dishantkharkar/LipSync-Wav2Lip-Project/assets/130529528/e8a11079-73a3-44fd-9008-5e98ae0341ce)

you got like this :![image](https://github.com/Dishantkharkar/LipSync-Wav2Lip-Project/assets/130529528/fd8721d6-3b41-4b35-9b09-68c14d35adfb)



### **Evaluation**

For evaluating the model, you can use the provided evaluation script:

```bash
python evaluation/evaluate.py --model_path <path_to_model> --data_path <path_to_evaluation_data>
```

Replace `<path_to_model>` and `<path_to_evaluation_data>` with the paths to your trained model and evaluation dataset, respectively.

## **Additional Information**

For more details and updates, refer to the [original Wav2Lip README](https://github.com/Rudrabha/Wav2Lip?tab=readme-ov-file).

## **Contributors**
- [Dishant Kharkar](www.linkedin.com/in/dishant-kharkar-17b508273)

