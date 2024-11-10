---
layout: single
title: "주피터노트북 커널 죽었을 시 해결법"
---

1. jupyter_notebook_config.py 파일을 찾아 max_buffer_size를 1000000000000000정도로 크게 늘려준다.

2. 아나콘다 프롬포트에서 환경을 재설치 후 실행때마다 new_env환경을 activate시켜준다.
```markdown
conda create -n new_env python=3.8
conda activate new_env
conda install jupyter numpy matplotlib torchvision -c pytorch
