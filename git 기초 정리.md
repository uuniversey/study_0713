
# Git 이란?
    - 분산 버전 관리 시스템이다.



# Git은 3개의 영역이 존재
    1. Working Directory
        * 현재 작업하고 있는 영역
    2. Staging Area
        * 버전 관리를 위해 파일들을 모아두는 임시 영역
    3. Repository
        * 실제 버전 관리에 대한 내용이 저장되는 영역



## Working Directory
* 실제로 작업이 이뤄지는 곳
* git status를 했을 때 붉은 색으로 표현됨
* 한 번도 버전 등록이 되지 않은 파일이나 폴더인 경우는 `untracked`로 표현된다.
* 한 번 이상 버전 등록이 된 파일이 변경이 이루어 졌다면 이 때는 `modified`라고 표현된다.



### .gitignore 파일
* 버전 관리에서 특정 파일을 제외시키기 위한 목록
    * 필요 없는 파일이란?
        * 프로젝트에서 실질적으로 사용하지 않는 것들 혹은 자동으로 생성되는 폴더나 파일
    * 절대 올려서는 안되는 중요한 파일
        * 개인정보가 들어있거나 혹은 api_key 같은 내용들이 담긴 파일
* gitignore 파일은 되도록이면 첫 commit에 같이 생성하여 등록하는 것이 좋다.
    * gitignore 파일을 자동으로 만들어 주는 곳은
    [gitignore.io](https://www.toptal.com/developers/gitignore/)이니 참고하자!



## Staging Area
* 버전 관리를 위해 파일이 임시로 모이는 영역
* `git status` 했을 때 초록색으로 표현된다.
* 처음 버전 등록이 될 파일은 `new file`로 표현된다.
* 한 번 이상 버전 등록 된 파일은 `modified`로 표현된다.
* 만약 버전 관리에 필요 없는 파일이나 폴더가 등록된 경우
    * 처음 버전에 등록될 파일이라면 `git rm --cached 파일명` 으로, 폴더라면 `-r` 옵션을 추가하여 Staging Area에서 Working Directory로 보내어 준다.(버전 관리 대상 목록에서 해당 파일명을 제외)
    * 한 번 이상 등록된 파일인 경우 `git restore --staged 파일명` 작성한다.

## Repository
* 버전 관리 정보가 들어있는 영역
* commit 된 상태인 내용들이 여기에 들어있다!
* 만약 commit을 잘못 찍었다면? --> 다음 시간에.....

