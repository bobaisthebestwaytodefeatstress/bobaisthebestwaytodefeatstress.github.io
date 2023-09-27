---
title:  "두번째 블로그"
excerpt: "여러분 Vim 쓰세요"

categories:
  - Blog
tags:
  - Blog
last_modified_at: 2023-08-18T08:06:00-05:00
---

# 맥에서 Vim 세팅하기

이 글을 읽는 사람들 중에서 Vim이 안깔려있는 사람은 없을거라 믿음ㅋㅋ
## 1. Vim 설치 확인

맥에는 기본적으로 Vim이 설치되어 있고 아래 명령어를 입력하여 확인할 수 있다.

```bash
vim --version
```

## 2. .vimrc 파일 생성 및 설정

`.vimrc` 파일은 Vim의 설정 파일입니다. 사용자 홈 디렉토리에 위치해야 합니다.

```bash
cd ~
touch .vimrc
```

이제 `.vimrc` 파일을 열고 원하는 설정을 추가하면 됩니다.

```bash
vi ~/.vimrc
```

다음은 일반적인 예시 설정입니다:

```vimscript
syntax on               " 문법 하이라이트 활성화 
set number              " 라인 번호 표시 
set tabstop=4           " 탭 너비를 4로 설정 
set softtabstop=4       " 탭키를 눌렀을 때 스페이스바 4번 누른 것과 같게 설정 
set shiftwidth=4        " >>, << 커맨드로 들여쓰기 할 때의 너비를 4로 설정  
set expandtab           " 탭 대신 스페이스 사용 
set autoindent          " 자동 들여쓰기 활성화  
```

## 3. 변경사항 적용하기 

변경사항을 적용하려면 다음 명령어를 입력합니다:

```bash
source ~/.vimrc
```

그러면 이제부터 vim 에디터를 열 때마다 위에서 정의한 세팅들이 반영됩니다.

---
위의 과정들은 간단하게 vim 을 세팅하는 방법 중 하나입니다.
더 다양한 옵션들과 플러그인들로 개인화된 작업환경을 만들 수 있습니다.
