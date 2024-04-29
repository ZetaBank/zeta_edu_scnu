.. _configuring_dwb_path_dist:

PathDistCritic
==============

PathDistCritic는 글로벌 플래너에서 제공한 경로에 대한 궤적을 얼마나 정렬시키는지에 따라 점수를 매깁니다.

매개변수
**********

``<name>``: :ref:`dwb_controller` 에서 **<dwb plugin>.critics** 매개변수에 정의된 경로 거리 평가기의 이름입니다.

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
        평가기의 가중 스케일.