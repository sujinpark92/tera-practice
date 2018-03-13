브랜치 생성
> git checkout -b sujin

브랜치 생성한것 원격저장소에 push
> git push origin sujin

작업 후,

커밋
> git add .

> git commit -m "commit message"

원격 저장소 내 브랜치에만 저장(no master)
> git push origin sujin


master에 반영하기

> git checkout master

> git merge sujin

master에 변경 사항 생기면

> git pull master

> git checkout sujin

> git merge master



-------------------------------------------


브랜치 생성
> git checkout -b sujin

브랜치 생성한것 원격저장소에 push
> git push origin dev

작업 후,

커밋
> git add .

> git commit -m "commit message"

원격 저장소 내 브랜치에만 저장(no master)
> git push origin sujin


master에 반영하기

> git checkout dev

> git merge sujin

master에 변경 사항 생기면

( dev 브랜치에서 )
> git pull dev

> git checkout sujin

> git merge dev