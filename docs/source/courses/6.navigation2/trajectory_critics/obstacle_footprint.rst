.. _configuring_dwb_obstacle_footprint:

ObstacleFootprintCritic
=======================

로봇의 풋프린트를 따라 모든 점이 코스트맵에서 표시된 장애물에 닿지 않는지를 확인하여 Trajectory에 점수를 매깁니다.

매개변수
**********

``<dwb plugin>``: :ref:`configuring_controller_server` 에서 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름.

``<name>``: :ref:`dwb_controller` 에서 **<dwb plugin>.critics** 매개변수에 정의된 ObstacleFootprintCritic 평가자 이름.


:``<dwb plugin>``.\ ``<name>``.sum_scores:

  ==== =======
  타입   기본값
  ------ -------
  bool false 
  ==== =======
    
    설명
        점수를 합산할 수 있는지 여부.

:``<dwb plugin>``.\ ``<name>``.scale:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        평가자에 대한 가중 스케일.