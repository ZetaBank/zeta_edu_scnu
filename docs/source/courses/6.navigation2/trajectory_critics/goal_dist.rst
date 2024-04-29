.. _configuring_dwb_goal_dist:

GoalDistCritic
==============

로봇이 목표 포즈에 도달할 때 Trajectory에 점수를 매깁니다.

매개변수
**********

``<dwb plugin>``: :ref:`configuring_controller_server` 에서 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름.

``<name>``: :ref:`dwb_controller` 에서 **<dwb plugin>.critics** 매개변수에 정의된 GoalDistCritic 평가자 이름.


:``<dwb plugin>``.\ ``<name>``.aggregation_type:

  ====== =======
  타입   기본값
  ------ -------
  string "last" 
  ====== =======
    
    설명
        마지막, 합계 또는 곱셈 결합 방법.

:``<dwb plugin>``.\ ``<name>``.scale:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        평가자에 대한 가중 스케일.