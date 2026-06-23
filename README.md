# 폴더 설명

- 실행 코드와 데이터셋은 midivae 폴더 안에 있습니다.
- output_sample은 모델을 사용하여 만들어본 1분짜리 샘플들입니다.

# 실행 전 유의사항

1. midivae/data/1.zip, midivae/data/2.zip을 압축해제한 후, 안에 있는 mood 폴더들을 data 디렉토리 밑에 위치시키기

```sh
mv midivae/data/1/* midivae/data/
mv midivae/data/2/* midivae/data/
rm midivae/data/*.zip
```

2. midivae 폴더를 구글드라이브 루트 폴더에 업로드(다른 디렉토리에 위치할 시, 코드 내 디렉터리, 파일 경로를 수정해주셔야 합니다.)

3. 모델 학습은 train.ipynb입니다. 런타임은 T4 GPU로 바꿔주세요.

4. 마인크래프트를 실행하며 실시간으로 음악을 만드는 파일은 midivae/generation_realtime.ipynb입니다.  
게임을 실행하지 않고 음악만 생성하기 위해선 midivae/generation_mp3.ipynb 파일을 실행해주세요.  
마찬가지로 런타임은 T4 GPU로 바꿔주세요.

- preprocessing은 실행할 필요 없습니다. 전처리된 data 파일들로 업로드하였습니다.

# 모드 적용

1. Fabric API 설치

2. contextmod-1.0.0.jar 파일을 .minecraft/mods 폴더에 넣기  

2. 런처에서 fabric API profile로 게임 실행