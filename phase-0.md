# Phase 0: 환경 세팅 — 완료

**완료일**: 2026-04-29

## 환경

- OS: Windows 11 Pro + WSL2 Ubuntu 22.04 (E:\Robot\wsl)
- GPU: NVIDIA RTX 4080 (Driver 591.86, CUDA 13.1)
- Python: 3.10.12 + venv (NumPy 2.2.6, Matplotlib, Jupyter, SciPy)
- C++: gcc 11.4.0, CMake 3.22.1
- Git: 2.34.1, GitHub SSH 인증
- VS Code: Remote-WSL + Python/C++/CMake/ROS 확장
- Docker: 29.4.1 + GPU 컨테이너 패스스루 검증

## 검증 통과

- [x] WSL Ubuntu에서 NumPy 동작 (`np.dot([1,2,3],[4,5,6]) == 32`)
- [x] CMake C++ 프로젝트 빌드/실행 (`sum == 15`)
- [x] GitHub 레포 생성 + SSH 푸시 정상
- [x] Docker GPU 패스스루 (`docker run --gpus all` 안에서 RTX 4080 인식)

## 다음

Phase 1 — 수학 + 운동학 토대 시작.
