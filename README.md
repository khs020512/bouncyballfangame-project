# bouncyballfangame-project
2022-07-15
> 캐릭터 구성


>> 점프,w/a/s/d를 이용한 움직임
![기본 움직임](https://user-images.githubusercontent.com/97209803/179245168-accb6cae-f3bd-4f66-a9e0-aa84b2be068a.PNG)
Tick 이벤트를 이용해 캐릭터가 무한히 점프할 수 있도록 구성
축 매핑을 통해 w/a/s/d의 입력량을 받아와 캐릭터를 움직일 수 있도록 구성

>> 마우스를 이용한 캐릭터 회전 변경
![마우스를 이용한 캐릭터 회전](https://user-images.githubusercontent.com/97209803/179245594-7eaa08eb-6eec-4d19-89b0-358d1c5312a6.PNG)
Yaw(z축)을 회전시켜 좌우로 캐릭터를 회전시킴
Spring Arm의 Pitch(Y축)을 회전시켜 캐릭터가 직접 회전하지는 않고 카메라가 회전하게 해 위 아래의 시야를 확인할 수 있게함.
Spring Arm의 회전값(Rotator)을 반환받아 회전의 최댓값과 최솟값을 지정한 후 값을 넘어가면 최댓값과 최솟값에서 시야를 고정시킴.
