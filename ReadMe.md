# NAYU : for elderly people living alone

I'm not good at English

![1](C:\Users\bolt6281\programming\Python\Team Projects\2019 ICT_COC Hackathon\1.png)

### Introduction

'NAYU'는 독거노인을 위한 1대1 랜덤 통화 매칭 서비스이며 AI Speaker에 탑재되도록 설계된 시스템입니다.

NAYU is 1v1 random voicetalk matching system for elderly people living alone and

desgined to be mounted on AI speaker.



외로움은 다른 사람의 도움 없이는 치료되기 어럽습니다. 하지만 독거노인은 대부분 새로운 사람을 만나는 것을 원하지 않으려하며, 정부기관이나 봉사단체에서 모든 독거노인을 관리하기는 어렵습니다. 이러한 이유로
아직도 많은 사람이 하루하루를 힘들게 보내고 있습니다.

Loneliness is very hard to be cured without other person. But elderly people are tend not to meet new people and any volunteers or government organizations can't cover all of the elderly living alone.
So many people are still having a hard time every day by day.



NAYU는 생활 속에서 사용자의 외로움을 감지하고 랜덤 매칭 통화 서비스를 통해 사용자가 우울감, 슬픔에서 벗어나도록 도와줍니다. 동시에 외로움을 느끼고 있는 사람과 매칭되어 서로의 외로움을 달랠 수 있습니다.

This system detects user's loneliness in life and help them to get out of depression and sadness from loneliness through random voicetalk matching system(just like Azar). User will be matched to another person who feels loneliness in the same time so that they can relieve each other's loneliness.



## Detect loneliness

- SpeechRecognition.py : If detects words that related to loneliness or saddness, run chat_client.py

GCP Speech2Text is used here



## Voice chat

- chat_server.py : run socket server | wait for client

- chat_client.py : run socket client : connect to server | voicechat starts

- mic_info.py : for check device index of mic