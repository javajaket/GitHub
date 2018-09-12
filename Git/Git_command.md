Git command
====
-----
1.Git 작업환경 시작하기 
  - `clone` 새로운 디렉터리에 Repository를 복제한다.
  - `init` 새로운 빈 Repositiory를 생성하고, 기존 존재하던 것들을 초기화한다.

2.현재 변경작업
  - `add` Add file contents to the index
  - `mv` Move or rename a file, a directory, or a symlink
  - `reset` Reset currnet HEAD to the specified state
  -  `rm` Remove files from the working tree and from the index

3.작업이력과 현재 상태를 검사
  - `bisect` Find by binary search the change that introuduced a bug
  - `grep` Print lines matching a pattern
  - `log` Show commit logs
  - `show` Show various types of objects
  - `status` Show the working tree status

4.성장, 표시, 당신의 최근 변경 이력
  - `branch` List,create, or delete branches
  - `checkout` Switch barnches or restore working tree files
  - `commit` Record changes to the repository
  - `diff` Show changes between commits, commit and working tree,etc
  - `merge` Join two or more development histories together
  - `rebase` Forward-port local comits to the updated upstream head
  - `tag` Create, list, delete or verify a tag object signed with GPG

5.협업 관련
  - `fetch` 다른 저장소에서 개체를 다운로드하고 바로 병합하지는 않는 상태
  - `pull` 원격저장소(Repository)에서 로컬저장소로 가져와 로컬지점과 통합한다.
  - `push` 관련 객체를 가지고 원격저장소에 업데이트 위해 보낸다. 바로 업데이트 되지 않는다.

6.원격 저장소 URL 변경
  - 기존 원격 저장소 URL을 변경하기 위해 `git remote set-url`명령어를 사용
  ```
  $ git remote -v 
    <!-- view existing remotes -->
  origin https://github.com/user/repo.git(fetch)
  origin https://github.com/user/repo.git(push)

  $ git remote set-url origin https://github.com/user/repos2.git
  ```

  ```
  $ git remote -v 
  <!-- Verify new remote URL -->
  origin https://github.com/user/repo2.git(fetch)
  origin https://github.com/user/rep02.git(push)
  ```
  - 두 개의 인자를 가진다.
    - 기존 원격 저장소 이름: origin
    - 새로운 원격 저장소 URL: https://github.com/user/repo2.git