---



copyright:
  years: 2017
lastupdated: "2017-10-24"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}


# 기존 가상 서버 다시 구성
{: #reconfiguring-virtual-servers}

가상 서버가 프로비저닝된 후에는 언제든지 해당 구성을 업그레이드하거나 다운그레이드할 수 있습니다.   

**중요 참고:** 사전 설정된 특색에는 사용 가능한 다양한 공용 가상 서버가 있습니다. 제한된 시간 동안, 사용자는 사전 설정된 특색이 사용되기 전에 사용 가능했던 모든 가상 서버를 수정할 수 있습니다. 그 후에는 기존 인스턴스를 마이그레이션하거나, 이를 취소하고 다시 주문해야 합니다.  

특색을 사용하는 가상 서버의 개별 코어, RAM 및 디스크 크기는 수정할 수 없습니다. 사용자는 자신이 필요로 하는 사전 설정된 코어 수, RAM 및 디스크 크기를 갖춘 다른 특색을 선택해야 합니다. 사용자가 선택하는 공용 가상 서버의 특색이 유효 코어 수, RAM 및 디스크 크기를 결정합니다.  

전용 가상 서버의 사용자 정의 범위는 더 넓으며, 따라서 사용자가 개별 코어, RAM 및 디스크 크기를 수정할 수 있습니다. 

기존 가상 서버를 다시 구성하려면 다음 단계를 수행하십시오.
{:shortdesc}

## 기존 가상 서버(사전 설정된 특색 사용) 수정
1. 고유 신임 정보를 사용하여 [{{site.data.keyword.slportal_full}} ![외부 링크 아이콘](../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com/)에 액세스하십시오. 
2. 디바이스 목록에서 다시 구성할 가상 서버의 이름을 클릭하십시오. 
3. **구성** 탭에서 **수정** 또는 **디바이스 구성 수정**을 클릭하여 다음 항목을 업데이트할 수 있습니다.  
  <dl>
  <dt>크기</dt>
  <dd>새 크기를 선택하십시오. </dd>
  <p><note>참고: 로컬 스토리지를 사용하는 특색을 수정하는 경우에는 로컬 스토리지가 아닌 스토리지를 사용하는 특색으로 전환할 수 없습니다. 마찬가지로, 로컬 스토리지가 아닌 스토리지를 사용하는 특색을 수정하는 경우에는 로컬 스토리지를 사용하는 특색으로 전환할 수 없습니다.
  </note></p>
  </dl>
4. 가상 서버에 대한 변경사항을 지정한 후에는 구성 업데이트를 완료하십시오. 
  <dl>
  
  <dt>업그레이드 날짜</dt>
  <dd>즉시 선택란을 클릭하여 즉각적 업데이트를 수행하거나, 업데이트가 활성 상태가 되는 시간을 스케줄할 수 있습니다. </dd>

  <dt>업그레이드 시간</dt>
  <dd>업데이트가 활성 상태가 되는 날짜(YYYY-MM-DD)를 입력하십시오. </dd>

  <dt>참고</dt>
  <dd>사용자의 디바이스에 해당되는 참고사항을 입력하십시오. </dd>
  </dl>

5. **계속**을 클릭하십시오. 
6. 주문 확인이 정확한지 검토하십시오. 업그레이드를 편집하려면 **편집**을 클릭하십시오. 
7. 주문을 확인하고 변경사항을 디바이스에 적용하려면 **확인**을 클릭하십시오. 

## 기존 가상 서버(사전 설정된 특색 사용 전) 또는 전용 가상 서버 수정
1. 디바이스 목록에서 다시 구성할 가상 서버의 이름을 클릭하십시오. 
2. **구성** 탭에서 **코어 또는 RAM 업그레이드** 링크를 클릭하여 다음 항목을 업데이트할 수 있습니다. 
  
|   업그레이드 옵션       |  설명                                                                                                     |
| ----------------------- | ----------------------------------------------------------------------------------------------------------- |
| 업그레이드 날짜         | 업데이트가 활성 상태가 되는 날짜(YYYY-MM-DD)를 입력하십시오. |
| 업그레이드 시간         | 업데이트를 활성화할 하루 중 시간에 대한 드롭 다운 상자에서 시간을 선택하거나 즉각적으로 업데이트하려면 **즉각적** 선택란을 클릭하십시오.|
| 코어 수| 해당되는 경우, 업데이트할 코어 수를 선택하십시오. |
| RAM| 해당되는 경우, 업데이트하기 위해 디바이스에 적용할 RAM의 양을 선택하십시오. |
| 업링크 포트 속도        | 해당되는 경우, 디바이스의 새 업링크 포트 속도를 선택하십시오. |
| 공용 대역폭             | 해당되는 경우, 디바이스의 공용 대역폭 양(GB)을 선택하십시오. |
| 첫 번째 디스크 - 다섯 번째 디스크 | 해당되는 경우, 첫 번째 디스크에 대한 디스크 공간/스토리지 옵션을 선택하십시오. 자세한 정보는 아래의 **디스크 참고**를 참조하십시오.|
| 참고| 사용자의 디바이스에 해당되는 참고사항을 입력하십시오. |
{: caption="표 1. 배치 옵션" caption-side="top"}   
  
  **디스크 참고:**
  * 로컬 및 SAN 스토리지 둘 다 사용 가능합니다. 스토리지 옵션이 올바른지 확인하려면 선택사항을 확인하십시오.
  * 공용 가상 서버의 경우, 로컬 스토리지를 업그레이드하면서 더 많은 코어 또는 RAM을 필요로 하는 경우에는 보조 디스크가 유실될 수 있습니다. 로컬 스토리지를 사용하는 가상 서버 특색을 수정하는 경우, 해당 특색은 사용자를 위해 사전 설정된 것이며 호환되지 않는 특색은 선택할 수 없습니다.
3. **계속**을 클릭하십시오. 
4. 주문 확인이 정확한지 검토하십시오. 업그레이드를 편집하려면 **편집**을 클릭하십시오. 
5. 주문을 확인하고 변경사항을 디바이스에 적용하려면 **확인**을 클릭하십시오. 