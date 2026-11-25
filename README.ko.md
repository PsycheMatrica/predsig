# predsig: 예측적 유의성 검정 소프트웨어

[English](README.md) · **한국어**

**저자** Gyeongcheol Cho · [g.cho@psychematrica.org](mailto:g.cho@psychematrica.org)

predsig 0.3.0은 확증적 선형회귀에서 각 예측변수의 예측 기여도를 추정하고,
회귀계수 유의성과 예측적 유의성을 함께 보고합니다.

## MATLAB

Windows의 MATLAB R2026a Update 4에서 검증했습니다. 이전 릴리스의
호환성은 확인하지 않았습니다.

1. [predsig_matlab_0.3.0.mltbx](MATLAB/predsig_matlab_0.3.0.mltbx)를
   내려받아 MATLAB에서 열고 **설치**를 선택합니다.
2. `setup_predsig`를 한 번 실행해 포함된 C 엔진을 컴파일합니다. MATLAB에서
   지원되는 컴파일러를 선택해야 하면 `mex -setup C`를 먼저 실행합니다.
3. `fitlm`으로 모형을 적합한 뒤 `predsig.run`에 넘깁니다. 모형 적합에는
   Statistics and Machine Learning Toolbox가 필요합니다.

## R

[predsig_0.3.0.tar.gz](R/predsig_0.3.0.tar.gz)를 내려받고 파일이 있는
폴더에서 아래 명령을 실행합니다.

```sh
R CMD INSTALL predsig_0.3.0.tar.gz
```

설치에는 C 컴파일 환경과 `readxl`, `digest` 패키지가 필요합니다.
`lm`으로 모형을 적합한 뒤 `predsig::run`에 넘깁니다.

## 인용 및 보충자료

> Cho, G. (2026). *predsig: Software for predictive significance testing* [Computer software]. https://github.com/PsycheMatrica/predsig/

분석에 사용한 버전을 명시합니다. [`CITATION.cff`](CITATION.cff)에서 인용
정보를 확인하거나 R에서 `citation("predsig")`를 실행할 수 있습니다. 논문의
[보충자료와 재현 코드](https://doi.org/10.5281/zenodo.24521729)는 Zenodo에서
제공합니다.

## 라이선스

저자가 작성한 코드와 문서는 CC BY-NC-SA 4.0을 따릅니다. 생성 코드와 제3자
구성 요소에 대한 고지는 각 설치 파일에 포함되어 있습니다.
