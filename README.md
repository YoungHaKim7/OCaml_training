<p align="center">
  <img width=25px src=https://github.com/user-attachments/assets/ddad614c-4b16-431f-951e-5f9bdf4d917e" />
  <img width=55px src=https://github-production-user-asset-6210df.s3.amazonaws.com/67513038/527075167-ddad614c-4b16-431f-951e-5f9bdf4d917e.svg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20251216%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20251216T132650Z&X-Amz-Expires=300&X-Amz-Signature=625ae4d298485d4dda393c2aa33683c6814ba53c8b0adcbaebe87ffddc09a278&X-Amz-SignedHeaders=host" />
![Image](https://github.com/user-attachments/assets/ddad614c-4b16-431f-951e-5f9bdf4d917e)
![Image](https://github.com/user-attachments/assets/0dffef3b-b00c-4564-a0f6-5ce5f72983af)
</p>

# OCaml_training
- OCaml is a general-purpose, industrial-strength programming language with an emphasis on expressiveness and safety.
- 공식 홈페이지
  - https://ocaml.org/
  - Github | The core OCaml system: compilers, runtime system, base libraries
    - https://github.com/ocaml/ocaml
- compile
  - https://github.com/ocaml-opam/opam-compiler

# Playground
- https://ocaml.org/play

# OCaml언어
- Rust는 개발 초기에 OCaml로 컴파일러가 제작되었다. 이후 언어가 발전함에 따라 컴파일러는 Rust 자체로 재작성되었다.
- 4. 학문적 위상
Haskell 등과 함께 힌들리-밀너 타입 시스템(Hindley-Milner Type System)을 사용하는 몇 없는 순수 함수형 언어이므로 프로그래밍 언어론을 공부하다 보면 꽤 자주 언급되는 것을 볼 수 있을 만큼 현업에서의 점유율과는 별개로 학술적 분야에서의 위상을 가진다. 자동정리증명 언어 중 하나인 Coq도 OCaml을 기반으로 한다.
- https://namu.wiki/w/OCaml

- Wiki정의
  - https://en.wikipedia.org/wiki/OCaml

# examples
- All the examples in Real World OCaml 
- https://github.com/realworldocaml/examples
  - (위 자료 막히기전 Deprecated 버젼) https://github.com/realworldocaml/scripts

# Install

```bash
$ bash -c "sh <(curl -fsSL https://opam.ocaml.org/install.sh)"
## Downloading opam 2.5.0 for linux on x86_64...
## Downloaded.
## Where should it be installed ? [/usr/local/bin]
Write access to '/usr/local/bin' required, using 'sudo'.
Command: install -m 755 /tmp/opam-2.5.0-x86_64-linux /usr/local/bin/opam
[sudo] password for g:
## opam 2.5.0 installed to /usr/local/bin
Write access to '/etc/apparmor.d' required, using 'sudo'.
Command: install -m 644 /tmp/opam-local.aa.tmp /etc/apparmor.d/opam-local
Write access to '/etc/apparmor.d' required, using 'sudo'.
Command: apparmor_parser -a /etc/apparmor.d/opam-local
AppArmor profile successfully added.
## Run this script again with '--restore ' to revert.
```
- https://ocaml.org/docs/installing-ocaml
```bash
<><> ocp-indent.1.9.0 installed successfully ><><><><><><><><><><><><><><><><><>
=> This package requires additional configuration for use in editors. Install package 'user-setup', or manually:

   * for Emacs, add these lines to ~/.emacs:
     (add-to-list 'load-path "/home/g/.opam/default/share/emacs/site-lisp")
     (require 'ocp-indent)

   * for Vim, add this line to ~/.vimrc:
     set rtp^="/home/g/.opam/default/share/ocp-indent/vim"
```

# 필수 설치

```bash
opam install ocaml-lsp-server odoc ocamlformat utop
```

- opam종료
  - `Ctrl + d`

# 프로젝트 만들기
- https://ocaml.org/docs/your-first-program

```bash
# 프로젝트 만들기 init
$ opam exec -- dune init proj hello
Success: initialized project component named hello


# build
opam exec -- dune build

# build하고 바로 실행
$ opam exec -- dune exec hello
Hello, World!
```

# watch모드

- Watch Mode
  - Before we dive in, note that you will typically want to use Dune's watch mode to continually compile and optionally restart your program. This ensures that the language server has the freshest possible data about your project, so your editor support will be top-notch. To use watch mode, just add the `-w` flag:

```bash
opam exec -- dune build -w
opam exec -- dune exec hello -w

```
