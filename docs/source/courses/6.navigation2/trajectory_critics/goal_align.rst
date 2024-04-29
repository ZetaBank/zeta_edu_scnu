.. _configuring_dwb_goal_align:

GoalAlignCritic
===============

목표 포즈와의 정렬 정도에 따라 Trajectory에 점수를 매깁니다.

매개변수
**********

``<dwb plugin>``: :ref:`configuring_controller_server` 에서 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름.

``<name>``: :ref:`dwb_controller` 에서 **<dwb plugin>.critics** 매개변수에 정의된 GoalAlignCritic 평가자 이름.

:``<dwb plugin>``.\ ``<name>``.forward_point_distance:

  ====== =======
  타입   기본값
  ------ -------
  double 0.325 
  ====== =======
    
    설명
        로봇 앞의 점으로, 이 점부터 목표 포즈까지의 각도 변경을 계산하는 데 사용됩니다.

:``<dwb plugin>``.\ ``<name>``.aggregation_type:

  ====== =======
  타입   기본값
  ------ -------
  string "last" 
  ====== =======
    
    설명
        last, sum 또는 product 결합 방법.

:``<dwb plugin>``.\ ``<name>``.scale:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        평가자에 대한 가중 스케일.