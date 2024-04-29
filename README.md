## <랭체인으로 LLM 서비스 만들기 소스 코드>
: 현직 AI Specialist에게 배우는 RAG! 랭체인, 오픈AI API, 스트림릿으로 8가지 서비스 구현까지
</br>
</br>

#### 소스 코드 수정(2024.4.1)
● 아나콘다, 랭체인의 변화로 작동하지 않는 코드를 발견 => 수정</br>
● 전체 코드 재검증</br>
</br>

#### 소스 코드 수정(2024.3.19)
● 랭체인 설치 시 버전을 지정(0.0.35)할 경우 작동하지 않는 코드를 발견 => 수정</br>
● 전체 코드 재검증</br>
</br>

#### 대상 독자
● 인공지능에 대한 지식은 별로 없지만 LLM을 이용한 서비스를 만들어보고 싶거나,</br>
● 개발은 잘 모르지만 역시 LLM을 이용한 서비스를 만들어보고 싶은 사람</br>
</br>

#### 다양한 실습 시나리오
● ‘LLM을 이용한 간단한 챗봇’ 만들기</br>
● ‘랭체인과 챗GPT로 RAG 기반의 챗봇’ 만들기</br>
● ‘PDF를 요약해주는 웹사이트’ 만들기</br>
● ‘PDF 파일에 대한 독립형 질문을 하는 챗봇’ 만들기</br>
● ‘대화형 챗봇’ 만들기</br>
● ‘LLM을 이용해서 CSV 파일 분석’하기</br>
● ‘번역 서비스’ 만들기</br>
● ‘메일 작성기’ 만들기</br>


conda create -n llm phthon=3.8
conda env list
conda activate llm
conda env remove -n llm

# 가상환경에서 주피터 노트북 설치
pip install ipykernel
# 가상환경에 커널 연결.
python -m ipykernel install --user --name llm --display-name "llm"
jupyter notebook

!pip install langchain==0.0.350