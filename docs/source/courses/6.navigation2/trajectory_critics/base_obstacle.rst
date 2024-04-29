.. _configuring_dwb_base_obstacle:

BaseObstacleCritic
==================

경로가 비용 맵을 통과하는 위치를 기반으로 Trajectory에 점수를 매깁니다. 
이를 올바르게 사용하려면 비행 로봇의 반경으로 장애물을 팽창시키는 비용 맵의 팽창 레이어를 사용해야 합니다.

매개변수
**********

``<dwb plugin>``: :ref:`configuring_controller_server` 의 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름.

``<name>``: :ref:`dwb_controller` 에서 정의된 **<dwb plugin>.critics** 매개변수에 정의된 BaseObstacleCritic 평가자 이름.

:``<dwb plugin>``.\ ``<name>``.sum_scores:

  ==== =======
  타입 기본값
  ---- -------
  bool false 
  ==== =======
    
    설명
        점수의 합산을 허용할지 여부.

:``<dwb plugin>``.\ ``<name>``.scale:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        평가자에 대한 가중 스케일.