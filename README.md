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
