# 1. DMZ
DMZ는 2022년 7월부터 8월까지 개발된 프로젝트입니다.<br>
신조어 번역을 위한 챗봇을 구축하는 것을 목표로 합니다.<br>
다양한 언어모델을 사용하여 사용자가 제시하는 신조어를 빠르게 이해하고 번역하는 역할을 수행합니다.<br>

# 2. 신조어 챗봇 서비스 개발

* 서비스 대상 모든 세대의 사람들을 대상 언어적으로 다양한 세대 간의 소통을 원활하게 돕는 유용한 도구
* KLUE/BERT모델을 통한 문장 평가및 GPT API를 이용하여 증강을 통해 기능 언어 학습을 강화 및 자연스러운 문장 추출
* 
# 3. Information Architecture
<div align="center">
  <img width="80%" height="80%" src="https://github.com/xoos0420/dmz/assets/131944211/312d9305-745c-4206-881b-c3268785c694"/>
</div>
<br>
  1. 사용자가 신조어와 함께 문의를 입력합니다.<br>
  2. 챗봇은 입력된 문장을 이해하기 위해 언어모델을 활용합니다.<br>
  3. 챗봇은 신조어의 의미를 파악하고, 가능한 번역 결과를 생성합니다.<br>
  4. 생성된 번역 결과를 사용자에게 제공하여 사용자가 해당 신조어의 의미를 이해할 수 있도록 도움을 줍니다.<br>
# 4. GPT API 대 DMZ 챗봇 비교

GPT API: GPT 언어모델은 강력한 자연어 이해 능력을 가지고 있지만, 사용자가 특정한 문맥을 설명하지 않을 경우에도 제한된 지식으로 답변할 수 있습니다.<br>
DMZ 챗봇: DMZ 팀의 챗봇은 신조어 번역에 특화된 기능을 가지고 있으며, 사용자가 신조어와 관련된 문맥을 제공할 경우 보다 정확한 번역 결과를 제공할 수 있습니다.

# 4. INSTALL
gpt api
```
!git clone https://github.com/xoos0420/dmz
%cd 0808_BERT_GPT
!pip install -r requirements.txt

%cd dmz_back
uvicorn app:app --reload
```
masked
```
!git clone https://github.com/xoos0420/dmz
%cd 0808_masked
!pip install -r requirements.txt

%cd dmz_back
uvicorn app:app --port 5000 --reload
```
# 5. 작동
<div align="center">
  <img width="40%" height="20%" src="https://github.com/xoos0420/dmz/assets/131944211/5fa46d4d-6326-4a6a-8a89-7d9a0b3a0b29"/>
</div>
