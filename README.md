# 실행 전 유의사항

1. midivae/data/1.zip, midivae/data/2.zip을 압축해제한 후, 안에 있는 mood 폴더들을 data 디렉토리 밑에 위치시키기

```sh
mv midivae/data/1/* midivae/data/
mv midivae/data/2/* midivae/data/
rm midivae/data/*.zip
```

2. midivae 폴더를 구글드라이브 루트 폴더에 업로드(다른 디렉토리에 위치할 시, 코드 내 디렉터리, 파일 경로를 수정해주셔야 합니다.)

3. 모델 학습은 train.ipynb입니다.

4. 게임을 실행하며 실시간으로 음악을 만드는 파일은 midivae/generation_realtime.ipynb입니다.  
게임을 실행하지 않고 음악만 생성하기 위해선 midivae/generation_mp3.ipynb 파일을 실행해주세요.

- preprocessing은 실행할 필요 없습니다. 전처리된 data 파일들로 업로드하였습니다.