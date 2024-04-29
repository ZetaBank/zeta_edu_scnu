.. _configuring_dwb_path_align:

PathAlignCritic
===============

전역 경로 기반 경로가 얼마나 잘 정렬되었는지에 따라 경로를 평가합니다.

매개변수
**********

``<name>``: :ref:`dwb_controller` 에서 **<dwb plugin>.critics** 매개변수에 정의된 PathAlignCritic 평가자 이름.


:``<dwb plugin>``.\ ``<name>``.forward_point_distance:

  ====== =======
  타입   기본값
  ------ -------
  double 0.325 
  ====== =======
    
    설명
        로봇 앞의 지점, 각 변화를 계산하기 위해 전방으로 볼 거리입니다.

:``<dwb plugin>``.\ ``<name>``.aggregation_type:

  ====== =======
  타입   기본값
  ------ -------
  string "last" 
  ====== =======
    
    설명
        마지막, 합계 또는 곱셈 조합 방법.

:``<dwb plugin>``.\ ``<name>``.scale:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        평가자에 대한 가중 스케일.