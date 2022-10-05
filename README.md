![github](https://user-images.githubusercontent.com/102712296/193993615-b74284f6-aa4e-49ec-aa3a-f97f1554da42.png)

# Git이 필요한 이유
## 1. 버전관리

#### - 무언가를 만드는 과정에서 계속해서 무언가를 빼고 고치고 수정 작업등을 거치게되는데 나중에 이전 기능을 다시 가져오게 될 수도 있고 누군가 실수로 잘못된 코드를 섞으면 복원해야 할 때도 있고 코드의 어디가 어떻게 바뀌었는지 과거 내역을 확인해야 할 때도 있을 것이다 ( 바뀌기 전의 내용들도 중간중간 저장을 해 줘야 함 )


## 2. 협업

#### - 여러 사람이 하나의 소스를 작업해도 충돌 방지/해결이 가능하며, 누가 어떤 작업을 진행했는지 확인이 가능하다.



# 사용 예시
![git commit](https://user-images.githubusercontent.com/102712296/193999045-34f25246-fe25-4b04-9ac1-131773868ee3.png)
![숨김폴더git](https://user-images.githubusercontent.com/102712296/193999187-e20885ee-7c52-4dcd-8cf1-aa17f1e39767.png)
#### - git init을 입력하면 현재있는 폴더의 모든 수정 내역들이 저장되는 .git이라는 숨김폴더가 생깁니다.
#### - git add -A로 백업에 포함할 파일들을 모두로 설정합니다.
#### - git commit -m "(작업수행 내용)" : 작업수행 내용을 기록 후 commit를 실행하면 이 폴더의 전체 내용들이 카메라처럼 찍히고 저장이 됩니다. 그 이후로도 프로젝트에 변화가 생긴다면 commit를 통해서 변화과정을 찍어줍니다.
#### - 이때! 이 과정을 여러번 한다고해서 용량을 몇 배로 차지하는게 아닌 변경사항들만을 기록하기 때문에 용량이 많이 차지하지도 않는다.

![git log](https://user-images.githubusercontent.com/102712296/194000042-2a4ed403-da23-4651-af72-54facf0e9e8e.png)
#### - git log 이때까지의 저장 내용들을 확인 가능합니다.


![reset](https://user-images.githubusercontent.com/102712296/194000313-8bfec60b-1d62-4029-9911-ebccb888ee91.png)
#### - git reset --hard 이름(앞의 몇 자만 입력해도 가능)
#### - 이때 고른 로그의 기록으로 되돌아가는데 reset이라는 뜻과 동일하게 과거로 돌아가지만, 과거로 돌아온 이후의 기록들은 모두 사라지게 됩니다.
#### - revert는 똑같이 과거로 이동하지만 이력을 남겨두고 원하는 시점으로 돌아갑니다.


# 그림 이해
## ●reset
![reset그림이해](https://user-images.githubusercontent.com/102712296/194001821-3a83098e-2711-45bd-bf85-a73414d8cff1.png)

## ●revert
![revert그림이해](https://user-images.githubusercontent.com/102712296/194001855-b1ba716c-884d-43bf-bc87-ef2a9ff2c2d3.png)


## Git 파일의 3가지 상태에 대하여

### Modified : 파일은 수정했으나 아직 commit하지 않은 것을 의미합니다.
### Staged : 수정한 파일들중 commit 할 것이라고 표시한 상태를 의미합니다.
![Staged](https://user-images.githubusercontent.com/102712296/194005537-942a1d38-c89d-4b6d-b9e2-345c4aa6105d.png)
### commit 대상을 목록으로 담아주는 장바구니 같은 영역이다.
#### 이렇게 commit할 파일들을 선택해주는 이유는 저장소안의 모든 파일들을 Commit하게 되면 수정이 없거나 사용하지 않는 파일들까지 모두 저장하게되어 저장소가 어지러워져 불편해집니다. 그렇다고 저장할때마다 불필요한 파일들을 내보냈다가 가져오기도 불편하기 때문이죠 Git은 이것을 Commit하기 전에 Stage라는 별도의 단계를 둬서 해결했습니다.

### Committed : Staged 상태의 파일들이 로컬 데이터베이스에 안전하게 저장됐다는 것을 의미합니다.
![git3가지 영역](https://user-images.githubusercontent.com/102712296/194007612-726ae381-e77e-4d08-b395-2b4638ab37b0.png)



# 깃허브
![깃허브](https://user-images.githubusercontent.com/102712296/194002852-891e0738-827a-49cc-a498-1187ba69e068.png)

#### 깃은 버전 관리를 위한 소프트웨어였다면, 깃허브는 깃들이 저장되는 공간을 제공해주는 [서비스]입니다.
### 깃 = 카메라 , 깃허브 = 유튜브 라고 생각하면 편합니다.
