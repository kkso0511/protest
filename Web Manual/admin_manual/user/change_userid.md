---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/user/change_userid
---

# 사용자 ID를 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

‘계정 관리’ 메뉴에서 사용자를 추가할 때 등록한 사용자 ID는 사용자 정보 편집 화면에서는 변경할 수 없습니다.\
사용자 ID를 변경하려면, 변경하려는 사용자를 한 번 삭제한 후 변경할 사용자 ID로 사용자를 새로 추가해야 합니다.이 매뉴얼에서는 사용자 ID를 변경하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* 사용자를 삭제하면 해당 사용자와 연결된 접근 제어 설정 정보, 기능 제한 설정 정보, 접근 권한 설정 정보도 함께 삭제되므로 주의해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**사용자 ID를 변경하려는 경우**
{% endhint %}

1. [사용자를 삭제하는 방법](https://help.directcloud.net/admin_manual/user/delete_user)의 단계에 따라 사용자 ID를 변경하려는 사용자를 삭제합니다.
2. [사용자를 추가하는 방법](https://help.directcloud.net/admin_manual/user/add_user)의 단계에 따라 만들려는 사용자 ID로 사용자를 새로 추가합니다.



{% hint style="warning" %}
**관리자의 ID를 변경하려는 경우**
{% endhint %}

1. 계약 담당 관리자로 관리자페이지에 로그인하고 [일반 관리자의 권한을 해제하는 방법](https://help.directcloud.net/admin_manual/user/remove_admin_permission) 의 단계에 따라 사용자 ID를 변경하려는 관리자의 권한을 해제합니다.
2. [사용자를 삭제하는 방법](https://help.directcloud.net/admin_manual/user/delete_user)의 단계에 따라 1단계의 사용자를 삭제합니다.
3. [사용자를 추가하는 방법](https://help.directcloud.net/admin_manual/user/add_user)의 단계에 따라 만들려는 사용자 ID로 사용자를 새로 추가합니다.
4. [사용자에게 일반 관리자 권한을 추가하는 방법](https://help.directcloud.net/admin_manual/user/add_admin_permission)의 내용에 따라 3단계에서 추가한 사용자에게 관리자 권한을 설정합니다.



{% hint style="warning" %}
**계약 담당 관리자의 ID를 변경하려는 경우**
{% endhint %}

1. 계약 담당 관리자로 관리자 페이지에 로그인한 후, [일반 관리자에게 계약 담당 관리자 권한을 위임하는 방법](https://help.directcloud.net/admin_manual/user/delegate_contract_admin)의 절차에 따라 일반 관리자에게 계약 담당 관리자 권한을 위임합니다.
2. 위의 1. 에서 새로 계약 담당 관리자가 된 사용자로 관리자 페이지에 로그인한 뒤, [일반 관리자의 권한을 해제하는 방법](https://help.directcloud.net/admin_manual/user/remove_admin_permission) 의 절차에 따라 사용자 ID를 변경하려는 관리자의 권한을 해제합니다.
3. [사용자를 삭제하는 방법](https://help.directcloud.net/admin_manual/user/delete_user)의 절차에 따라 사용자 ID를 변경하려는 사용자를 삭제합니다.
4. [사용자를 추가하는 방법](https://help.directcloud.net/admin_manual/user/add_user)의 절차에 따라 생성하려는 사용자 ID를 사용하여 사용자를 새로 추가합니다.
5. [사용자에게 일반 관리자 권한을 추가하는 방법](https://help.directcloud.net/admin_manual/user/add_admin_permission)의 절차에 따라, 절차 4에서 추가한 사용자에게 관리자 권한을 설정합니다.
6. [일반 관리자에게 계약 담당 관리자 권한을 위임하는 방법](https://help.directcloud.net/admin_manual/user/delegate_contract_admin)의 절차에 따라, 절차 5에서 설정한 일반 관리자에게 계약 담당 관리자 권한을 다시 위임합니다.
