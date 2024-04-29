.. _configuring_dwb_oscillation:

OscillationCritic
=================

로봇이 단순히 전후로 이동하지 않도록 합니다.

매개변수
**********

``<dwb plugin>``: :ref:`configuring_controller_server` 에서 **controller_plugin_ids** 매개변수에 정의된 DWB 플러그인 이름.

``<name>``: :ref:`dwb_controller` 에서 **<dwb plugin>.critics** 매개변수에 정의된 OscillationCritic 평가자 이름.


:``<dwb plugin>``.\ ``<name>``.oscillation_reset_dist:

  ====== =======
  타입   기본값
  ------ -------
  double 0.05  
  ====== =======
    
    설명
        오실레이션 감시 재설정을 위한 최소 이동 거리 (m).

:``<dwb plugin>``.\ ``<name>``.oscillation_reset_angle:

  ====== =======
  타입   기본값
  ------ -------
  double 0.2  
  ====== =======
    
    설명
        오실레이션 감시 재설정을 위한 최소 각도 이동 거리 (rad).

:``<dwb plugin>``.\ ``<name>``.oscillation_reset_time:

  ====== =======
  타입   기본값
  ------ -------
  double -1  
  ====== =======
    
    설명
        재설정이 호출될 수 있는 지속 시간. -1이면 재설정이 불가능합니다.

:``<dwb plugin>``.\ ``<name>``.x_only_threshold:

  ====== =======
  타입   기본값
  ------ -------
  double 0.05  
  ====== =======
    
    설명
        X 속도 방향에서 확인할 임계값.

:``<dwb plugin>``.\ ``<name>``.scale:

  ====== =======
  타입   기본값
  ------ -------
  double 1.0 
  ====== =======
    
    설명
        평가자에 대한 가중 스케일.