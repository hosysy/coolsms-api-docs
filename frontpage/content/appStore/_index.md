+++
title = "쿨에스엠에스 앱 스토어 "
description = ""
date = "2017-09-14T18:36:24+02:00"
weight = 40
+++


## 쿨에스엠에스 앱 스토어란?

쿨에스엠에스를 이용하여 문자 발송 시 해당 프로그램의 개발자들에게 수익금을 적립 해드리는 서비스 입니다.

수익금은 **20,000원** 이상이 되면 출금 가능하며 출금요청 후 확인기간(7일)이 지난 뒤에 [정산정보](https://www.coolsms.co.kr/app_cash_manager)에 입력된 계좌번호로 입금 됩니다.<br />

{{%notice info%}}
이 문서에서 지칭하는 **앱**은 쿨에스엠에스 **앱 스토어**를 이용하는 문자 솔루션을 얘기합니다.
{{%/notice%}}

## 적용 방법

#### 1. 정산정보 입력
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[정산정보](https://www.coolsms.co.kr/app_provider)페이지에서 정산정보를 등록합니다.

#### 2. 내 앱 만들기
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[앱 관리](https://www.coolsms.co.kr/my_app_list)페이지에서 **앱 등록**버튼을 클릭한 뒤 각각 폼에 맞게 입력 후 **생성**버튼을 클릭합니다.

#### 3. 앱 아이디 확인
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
앱 생성을 완료한뒤 [앱 관리](https://www.coolsms.co.kr/my_app_list)페이지에서 앱 아이디를 확인합니다.


![find_app_id.png](/images/find_app_id.png)

#### 4. 문자 발송 코드내에 앱 아아디 입력
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[REST API v1, v2](https://www.coolsms.co.kr/REST_API)의 경우 **srk**, [REST API v3](http://sms-api-v3.readthedocs.io/ko/latest/)는 **app_id**필드에 위에서 발급받은 **앱 아이디**값을 넣어주시면 됩니다.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
{{<button href="https://google.com" >}} REST API v1 사용방법 바로가기 {{< /button >}}
{{<button href="https://google.com" >}} REST API v2 사용방법 바로가기{{< /button >}}
{{<button href="https://google.com" >}} REST API v3 사용방법 바로가기{{< /button >}}

## 수익금 종류

문자발송 건당 발생하며 **기본수익금**과 **추가수익금** 두가지로 구분 되며 각각 설명은 아래를 참고 부탁드립니다.

* 기본수익금 : <br />
&nbsp;&nbsp;
기본적으로 발생하는 수익으로 [REST API v1, v2](https://www.coolsms.co.kr/REST_API)이용시 **1원** [REST API v3](http://sms-api-v3.readthedocs.io/ko/latest/) 이용시 **2원**이 적립됩니다.

* 추가수익금 : <br />
&nbsp;&nbsp;
[REST API v3](http://sms-api-v3.readthedocs.io/ko/latest/) 이용시에만 적용되며 **앱 개발자가 지정한 단가 - 기본단가의 차익**만큼 추가로 적립됩니다. <br />

{{%notice note%}}
  개발자가 추가 수익금을 10원으로 했다면 [REST API v3](http://sms-api-v3.readthedocs.io/ko/latest/)이용시 실제로 차감되는 금액은 **(기본단가(20원) + 추가수익금(10원) = 총 30원)**이며
  이중 **(추가수익금(10원) + 기본수익금 (2원) = 총 12원)**은 앱 개발자에게 적립됩니다.
{{%/notice%}}

## 수익금 확인 및 출금 요청 방법

[캐쉬 매니저](https://www.coolsms.co.kr/app_cash_manager)에서 수익금 확인을 실시간 확인 할 수 있으며, 마찬가지로 같은 페이지의 '출금요청'탭에서 출금요청이 가능합니다.
{{%notice note%}}
  수익금은 **20,000원** 이상이 되면 출금 가능하며 출금요청 후 확인기간(7일)이 지난 뒤에 [정산정보](https://www.coolsms.co.kr/app_cash_manager)에 입력된 계좌번호로 입금 됩니다.<br />
  출금 수수료는 [앱 스토어 출금수수료율](https://coolsms.zendesk.com/knowledge/articles/115000666032/ko?brand_id=7472347&return_to=%2Fhc%2Fko%2Farticles%2F115000666032)에서 확인 가능합니다.
{{%/notice%}}
