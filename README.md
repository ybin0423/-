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
   
## 백엔드 개념 

1. Call by reference : 참조에 의한 호출, 메소드에 변수를 전달할 때 변수의 참조 전달, 메소드 내에서 변수를 수정하면 호출자의 변수도 변경 
   - Call by value; 자바에서 메서드 호출 시 스프링이 따르는 방법.
     값에 의한 호출 -> 메소드에 변수를 전달할 때 해당 변수 값이 복사되어 사용.
     변수의 값이 변결되지 않음.
2. Override vs Overload
   - Override; 상위 클래스의 매서드를 재정의하는 것. (메서드의 이름, 파라미터의 개수, 타입)

     ->Occurs bw superclass and subclass; have same signature(name & method arguments)
   - Overload; 매서드의 이름은 같고 파라미터의 개수나 타입이 다른 함수를 정의 하는것

     -> Occurs bw methods in same class; hav same name but diff parameters

3. JVM (Java Virtual Machine) - 자바 프로그램을 실행하는 가상 머신
4. Java가 컴파일되는 과정
   
   '''
     1. 로드 (load)
        클래스 파일을 가져와 JVM의 메모리에 로드하는 과정
        자바 소스 코드 (.java) -> 자바 컴파일러가 이 소스 코드를 읽어 바이트 코드 (.class)로 컴파일 -> 클래스로더에게 전달 (클래스 로더는 필요한 클래스들을 링크해 jvm메모리에 업로드해 런타임 데이터를 구성)
     2. 검증 - 자바 어
     3. 검증
  
   '''
