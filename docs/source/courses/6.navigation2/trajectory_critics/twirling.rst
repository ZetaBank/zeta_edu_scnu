.. _configuring_dwb_twirling:

TwirlingCritic
==============

목표 지점으로 이동하는 동안 홀로노믹 로봇이 회전하는 것을 방지합니다.

매개변수
**********

``<dwb plugin>``: :ref:`configuring_controller_server` 에서 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름입니다.

``<name>``: :ref:`dwb_controller` 에서 **<dwb plugin>.critics** 매개변수에 정의된 TwirlingCritic 평가기의 이름입니다.

:``<dwb plugin>``.\ ``<name>``.scale:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        평가기의 가중 스케일.



