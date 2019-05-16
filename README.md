# HeLP Challenge Contest 2018
### Train

- 터미널에서 `sh train.sh`

  > path 설정 및 에폭 설정 후 실행

### Inference

- 터미널에서 `sh inference.sh`

  > path 설정 및 실행

---

### ISSUE

- model Instancenormalization 이슈 발생 시

  - ```
    pip install git+https://www.github.com/keras-team/keras-contrib.git
    ```

- 그래도 keras.layer에서 이슈 발생 시

  - ./site-packages/keras-contrib/layers/normalization/instancenormalization.py 접근
  - 인스턴스 노말라이제이션 Class 복사
  - ./site-packages/keras/layers/normalization.py에 접근
  - 복사한 인스턴스노말라이제이션 클래스 붙여넣기

