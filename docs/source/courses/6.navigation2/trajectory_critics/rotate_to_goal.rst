.. _configuring_dwb_rotate_to_goal:

RotateToGoalCritic
==================

로봇이 목표 위치에 충분히 가까울 때만 목표 방향으로 회전하도록 허용합니다.

매개변수
**********

``<dwb plugin>``: :ref:`configuring_controller_server` 에서 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름입니다.

``<name>``: :ref:`dwb_controller` 에서 **<dwb plugin>.critics** 매개변수에 정의된 RotateToGoalCritic 평가기의 이름입니다.

:``<dwb plugin>``.xy_goal_tolerance:

  ====== =======
  타입   기본값
  ------ -------
  double 0.25 
  ====== =======
    
    설명
        목표 달성 기준을 충족하는 허용 오차 (m).

:``<dwb plugin>``.trans_stopped_velocity:

  ====== =======
  타입   기본값
  ------ -------
  double 0.25 
  ====== =======
    
    설명
        이하 속도는 허용 오차에 도달하여 정지한 것으로 간주됩니다 (rad/s).

:``<dwb plugin>``.\ ``<name>``.slowing_factor:

  ====== =======
  타입   기본값
  ------ -------
  double 5.0 
  ====== =======
    
    설명
        목표로 회전하는 동안 로봇 이동 속도를 감소시키는 요소입니다.

:``<dwb plugin>``.\ ``<name>``.lookahead_time:

  ====== =======
  타입   기본값
  ------ -------
  double -1 
  ====== =======
    
    설명
        > 0인 경우 충돌을 감지하기 위해 앞으로 볼 시간량입니다.

:``<dwb plugin>``.\ ``<name>``.scale:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        평가기의 가중 스케일.