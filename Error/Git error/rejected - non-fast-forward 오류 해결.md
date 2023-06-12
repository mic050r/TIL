# Eclipse rejected - non-fast-forward 오류

오늘 이클립스에서 푸쉬를 할려 했는데 rejected - non-fast-forward 오류가 났다.

<img src="https://github.com/mic050r/TIL/assets/103114387/27b19128-1ffb-457f-8bc3-513355bfc4c1"  width="400" height="290">

<br>

## 해결 방안 
1. Window → Show View → Other → Git Repositories 선택

2. 해당하는 저장소의 Remotes → origin →  github주소 우클릭 → configure Fetch 클릭

3. Ref mappings가 존재 → Advanced 클릭

  - 없을 경우 Add를 눌러 추가

4. 기존에 있는 Source Ref 를 Remove(휴지통 모양)을 눌러 지워주기

5. Add create/update specification 안에서 Source ref: 지정(master[branch] 선택하면 자동입력) → Add Spec 클릭

6. Finish 클릭 → Save and Fetch 누르기

7. Branches → Local 에 있는 가지를 우클릭해서 Merge 클릭

8. 다시 프로젝트에서 Team - Remote - Push

9. Push하면 완료
<br>

## 참고 블로그
아래의 블로그를 참고하였다.
> https://hanyda.tistory.com/36
>
