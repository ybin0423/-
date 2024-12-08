## 이미지 복구 알고리즘

**Algorithm Steps:**
1. Preprocessing: Load the dataset of black-and-white damaged images and their corresponding ground truth images.
   
2. Image Restoration: Implement an algorithm for denoising and repairing the damaged images (e.g., using neural networks such as convolutional autoencoders).
   
3. Image Colorization: Use colorization techniques to predict the color version of the restored images (e.g., using models like DeOldify or GANs).
   
4. Evaluation: Calculate SSIM scores between the restored/colorized images and the ground truth.
   
5. Submission: Output the colorized images in the correct format for submission.
   
Next Steps:

1. Processing the Image: I can assist with processing or analyzing the uploaded image for restoration or colorization if it is part of the dataset.
   
2. Dataset Handling: You would need the dataset (train_input, train_gt, train.csv, etc.) for training the model and testing its performance. You can either upload the dataset or run the code locally to train and test the model.

1. UMAP을 활용한 이미지 클러스터링
   
   - 이미지 임베딩 생성
     
   - CLIP 모델을 활용하여 이미지 특징을 추출
     
   - UMAP을 사용하여 이미지 임베딩을 축소
     
2. 모델 학습 준비
   
   - 데이터 분리 및 전처러 (train, test dataset 준비, 학습에 필요한 입력  이미지 생성)
   - SSIM 및 히스토그램 유사도를 계산하는 함수를 정의하여 전체 이미지 또는 특정 마스크 영역에 대한 유사도 계산

3. 성능 향상:
   
   -n_neighbours 값 증가
   -Batch_size 값 줄이기
   -추가 전처리
   
