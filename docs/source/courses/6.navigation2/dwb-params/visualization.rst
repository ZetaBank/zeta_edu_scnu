.. _dwb_publisher:

Publisher
=========

매개변수
----------

``<dwb plugin>``: :ref:`configuring_controller_server` 의 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름.

:``<dwb plugin>``.publish_evaluation:

  ==== =======
  타입 기본값
  ---- -------
  bool true      
  ==== =======

  설명
    로컬 계획 평가를 발행할지 여부.

:``<dwb plugin>``.publish_global_plan:

  ==== =======
  타입 기본값
  ---- -------
  bool true      
  ==== =======

  설명
    전역 계획을 발행할지 여부.

:``<dwb plugin>``.publish_transformed_plan:

  ==== =======
  타입 기본값
  ---- -------
  bool true      
  ==== =======

  설명
    오도메트리 프레임에서 전역 계획을 발행할지 여부.

:``<dwb plugin>``.publish_local_plan:

  ==== =======
  타입 기본값
  ---- -------
  bool true      
  ==== =======

  설명
    로컬 플래너의 계획을 발행할지 여부.

:``<dwb plugin>``.publish_trajectories:

  ==== =======
  타입 기본값
  ---- -------
  bool true      
  ==== =======

  설명
    디버그 경로를 발행할지 여부.

:``<dwb plugin>``.publish_cost_grid_pc:

  ==== =======
  타입 기본값
  ---- -------
  bool false      
  ==== =======

  설명
    비용 그리드를 발행할지 여부.

:``<dwb plugin>``.marker_lifetime:

  ============== =======
  타입           기본값
  -------------- -------
  double         0.1    
  ============== =======

  설명
    마커가 유지될 시간.

이 위의 내용은 Publisher를 설명합니다.