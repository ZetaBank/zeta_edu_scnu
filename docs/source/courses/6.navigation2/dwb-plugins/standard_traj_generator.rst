.. _configuring_dwb_stand_traj_gen_plugin:

StandardTrajectoryGenerator
===========================

매개변수
**********

``<dwb plugin>``: :ref:`configuring_controller_server` 의 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름.

:``<dwb plugin>``.sim_time:

  ====== =======
  타입   기본값
  ------ -------
  double 1.7
  ====== =======
    
    설명
        (s) 앞으로 시뮬레이션할 시간.

:``<dwb plugin>``.discretize_by_time:

  ==== =======
  타입 기본값
  ---- -------
  bool false
  ==== =======
    
    설명
        True인 경우 시간에 따라 전진 시뮬레이션합니다. False인 경우 선형 및 각도 증분에 따라 전진 시뮬레이션합니다.

:``<dwb plugin>``.time_granularity:

  ====== =======
  타입   기본값
  ------ -------
  double 0.5
  ====== =======
    
    설명
        전진할 시간.

:``<dwb plugin>``.linear_granularity:

  ====== =======
  타입   기본값
  ------ -------
  double 0.5
  ====== =======
    
    설명
        전진할 선형 거리.

:``<dwb plugin>``.angular_granularity:

  ====== =======
  타입   기본값
  ------ -------
  double 0.025
  ====== =======
    
    설명
        전진할 각도.

:``<dwb plugin>``.include_last_point:

  ==== =======
  타입 기본값
  ---- -------
  bool true
  ==== =======
    
    설명
        Trajectory에 마지막 포인트를 포함할지 여부.


여기까지 StandardTrajectoryGenerator의 설명입니다.