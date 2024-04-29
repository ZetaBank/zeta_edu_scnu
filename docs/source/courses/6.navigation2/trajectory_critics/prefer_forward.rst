.. _configuring_dwb_prefer_forward:

PreferForwardCritic
===================

전방 이동을 보다 높게 점수화하는 궤적에 대한 점수를 매깁니다.

매개변수
**********

``<dwb plugin>``: :ref:`configuring_controller_server` 에서 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름입니다.

``<name>``: :ref:`dwb_controller` 에서 **<dwb plugin>.critics** 매개변수에 정의된 PreferForwardCritic 평가기의 이름입니다.

:``<dwb plugin>``.\ ``<name>``.penalty:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        후진 운동에 적용할 페널티.

:``<dwb plugin>``.\ ``<name>``.strafe_x:

  ====== =======
  타입   기본값
  ------ -------
  double 0.1 
  ====== =======
    
    설명
        페널티를 적용하기 전의 최소 X 속도.

:``<dwb plugin>``.\ ``<name>``.strafe_theta:

  ====== =======
  타입   기본값
  ------ -------
  double 0.2 
  ====== =======
    
    설명
        페널티를 적용하기 전의 최소 각도 속도.

:``<dwb plugin>``.\ ``<name>``.theta_scale:

  ====== =======
  타입   기본값
  ------ -------
  double 10.0 
  ====== =======
    
    설명
        각도 속도 구성요소에 대한 가중치.

:``<dwb plugin>``.\ ``<name>``.scale:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        평가기의 가중 스케일.