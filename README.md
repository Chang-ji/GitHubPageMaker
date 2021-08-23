## Chang-ji.github.io 에 올리는 법
1. GitHubPageMaker 빌드 
~~~bash
bundle exec jekyll serve
~~~
2. output 파일 github 연결(초기)
~~~bash
cd output
git init
git add .
git commit -m "first commit"
git branch -M main
git remote set-url origin https://github.com/Chang-ji/Chang-jigithub.io.git
git remote add origin https://github.com/Chang-ji/Chang-jigithub.io.git
git pull origin main
cd ..
bundle exec jekyll serve
cd output
git push -u origin main
~~~
> github Desktop 받은 후에 clone을 두번하자  
이때 두번재 clone은 output으로 폴더를 만들자

3. output 파일 github 연결(한번 연결 이후)
~~~bash
cd output
git add .
git commit -m "second commit"
git pull origin main
cd ..
bundle exec jekyll serve
cd output
git push -u origin main
~~~

4. 자동 배포 파일 추가
~~~bash
start AutoDeploy.bat
~~~