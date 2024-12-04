# Picktalk

# 프로젝트의 목적

## 프로젝트가 해결하고자하는 문제

일본어 회화를 공부하고자하는 학생들은 흔히 다음과 같은 문제에 직면합니다.

1. 일본의 다양한 일상 생활 속에서 마주하게되는 문제와 상황에 대한 회화를 연습하고 싶으나 다양한 상황을 쉽게 상정하기가 어렵다.
2. 다양한 상황에서의 회화 연습을 기록하고 복습하기 어렵다.
3. 다양한 상황에서의 적법한 회화를 직접 알아내기가 어렵다.
4. 회화는 본래 상대가 필요한 것이나 회화를 개인적으로 연습하고자할 때 상대를 찾기가 어렵다.

본 프로젝트는 이 문제를 IT Solution을 통해 해결하고자 합니다.

# 프로젝트가 사용자에게 제공하는 것

최종 사용자가 사용할 수 있는 웹-인터페이스

# 사용자의 유즈케이스(유저 시나리오)

`유즈케이스란?`

`유즈케이스는 사용자가 실제로 제품,프로젝트 등을 사용하는 실제 상황을 가정하여 만든 일종의 시나리오이다. 유즈케이스를 상정하는 것을 통해 제품에서 요구되어지는 기능의 주요 목적과 필요되는 기능, 사용자의 제품 사용 경험을 예측하여 보다 고품질의 소프트웨어를 생산할 수 있다.`

### 1. 처음 방문한 유저

유저는 처음 본 웹 사이트를 방문하여, 웹 사이트의 랜딩페이지를 탐색합니다. 랜딩 페이지에서는, 본 웹사이트에서 어떤 기능을 제공하는지, 사용자는 무엇을 기대할 수 있는지를 사용자가 볼 수 있습니다.

본 서비스를 사용해보고자 결정한 사용자는, 로그인 버튼을 클릭하여 로그인을 시도합니다. 사용자는 로그인 페이지로 이동합니다.

로그인 페이지에 도달한 사용자는, 로그인 폼을 볼 수 있고, 로그인 폼의 하단에 “처음이신가요? 회원가입을 진행하세요”라는 메시지를 볼 수 있습니다. 이 사용자는 이번에 처음 방문한 것이므로, 당연히 회원가입을 시도합니다. “회원가입”링크를 클릭한 사용자는 회원가입 페이지로 이동합니다. 회원가입 페이지로 이동한 사용자는 회원가입 폼을 볼 수 있습니다. 폼을 모두 채운 사용자가 “회원가입” 버튼을 누르면 회원가입이 진행되고, 회원가입이 완료되면 사용자는 로그인 페이지로 이동됩니다.(폼을 모두 채우지 않으면 진행되지 않습니다, 에 부적절한 정보, 예를들어 이미 사용중인 아이디, 잘못된 이메일 등을 입력한 경우에도 회원가입이 진행되지 않습니다.)

다시 로그인 페이지에 도달한 사용자는, 회원가입 시 기입한 정보를 사용하여 로그인을 시도합니다. 로그인에 성공하면 본 서비스의 메인 페이지로 이동합니다.

처음 메인 페이지에 도달한 사용자는, 각 기능별 도움말을 보게됩니다.

## 2. 다시 방문한 유저

다시 방문한 유저는 짧은 시간(약 2주)내에 방문한 경우, 별도의 로그인 절차 없이 로그인이 되어 본 서비스에 접속시, 바로 서비스 메인 페이지로 이동됩니다.

그렇지 않은경우(2주 이상 경과)에는, 다시 처음 방문한 경우처럼 랜딩페이지로 자동으로 이동됩니다.(리다이렉션)

## 3. 메인 페이지에 방문한 유저

메인 페이지에 방문한 유저는 크게 다음과 같은 작업을 수행할 수 있습니다.

1. 나의 계정정보 확인
   1. 나의 계정 정보는 “마이페이지” 페이지로 이동하여 확인 가능하며, 마이페이지에서는 다음과 같은일을 할 수 있습니다. 나의 계정정보 수정, 회원 탈퇴, 내가 등록한 대화 정보 확인, 내가 등록한 대화에 포함된 단어 정보 확인
2. 대화 생성
   1. 새로운 대화를 생성할 수 있습니다.
   2. 대화 생성 후, 각 대화별 탭으로 이동하게 되며, 추가하고 싶은 단어를 대화 별로 추가하여 이후 발화 생성에 사용할 수 있습니다.
3. 대화 생성 탭으로 이동
   1. 대화 생성 탭으로 이동한 유저는 대화에 새로운 단어(토큰)을 추가할 수 있습니다.
   2. 추가한 토큰을 기반으로 “랜덤 발화 생성” 버튼을 눌러 새로운 발화를 생성할 수 있습니다.
   3. 발화에 대한 답변을 입력하면 답변이 저장됩니다. 이후 이 답변은 “내 대화 보기”에서 질문과 답변으로 확인할 수 있습니다.
   4. “토큰 보기” 버튼을 눌러 현재 대화에 포함된 토큰을 보고, 추가하거나 제거할 수 있습니다.
   5. 유저는 답변 시, “인공지능 추천받기” 버튼을 눌러, 제시된 주제에 대한 인공지능 추천 답변을 제공받을 수 있습니다. 인공지능 추천받기는 최대 3회로 제한됩니다.
   6. 유저는 자신이 만든 문장(발화)에 대해 인공지능 첨삭을 받을 수 있습니다.

# 테크 스택

- [Next.js](https://nextjs.org/)
  - 프론트엔드 서버입니다. 클라이언트 애플리케이션 서빙을 담당합니다.
  - 사용하는 이유: 프론트엔드를 백엔드와 분리하여 개발하기 위함입니다.
- [Springboot](https://spring.io/projects/spring-boot) 3.xx
  - 백엔드 서버입니다. 핵심 비즈니스 로직과 데이터 접근을 담당합니다.
  - 사용하는 이유: 핵심 비즈니스 로직을 빠르게 개발하기 위함입니다.
- [Mysql](https://www.mysql.com/) 8.xx, 9.xx
  - 데이터베이스입니다. 데이터베이스 서빙과 데이터 저장을 담당합니다.
  - 사용하는 이유: 안정성있는 RDBMS로, 오라클보다 사용하기 쉽고 성능이 뒤떨어지지 않습니다.
- [AWS](https://aws.amazon.com/ko/?nc2=h_lg), [GCP](https://cloud.google.com)
  - 클라우드 플랫폼입니다. 클라우드에 서비스 구성요소를 업로드하여 유지하는 것을 담당합니다.
  - 사용하는 이유: 가상머신을 사용하여 안정적으로 서비스를 운영하기 위함입니다.

# 문서화

문서화는 소프트웨어에서 중요한 부분 중 하나입니다.

기록을 통해 산출물과 기획 의도와의 정합성을 확인할 수 있으며, 차후에 산출물에 대한 부가정보로 활용할 수 있습니다.

문서화는 버전관리와도 통합될 수 있습니다. 예를 들어 소프트웨어가 버전 1.0.0이라면, 그에 해당하는 1.0.0문서가 존재하고, 이후에는 버전이 올라갈 때마다 기존 버전과 달라진점만 문서화하면서 문서를 간소화할 수 있습니다.

본 프로젝트에서 문서화를 통해 얻고자하는 것은, 문서화를 통해 차후 포트폴리오로 사용될 때, 부가적인 정보를 제공하는 것과, 본 서비스를 이용하는 유저에게 제공되는 소프트웨어의 상태를 기술하는 것, 그리고 팀 프로젝트의 현황을 기록하여 팀원 간의 공유되는 의견및지식의 불일치를 해소하고, 프로젝트를 진행해가며 재검토할 수 있는 여지를 남겨두는 것입니다.