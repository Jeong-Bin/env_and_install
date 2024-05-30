# env_and_install

<가상환경 생성 및 실행> \d
conda create -n [가상환경명] python=3.8 cudatoolkit==11.4
conda activate [가상환경명]

<가상환경 목록 확인>
conda info --envs

<가상환경 종료>
conda deactivate

<가상환경 삭제>
conda remove --name [가상환경명] --all

<주피터 노트북 설치>
pip3 install jupyter notebook ipykernel
python -m ipykernel install --user --name [가상환경명] --display-name [커널명]

<커널 목록 확인>
jupyter kernelspec list

<커널 삭제>
jupyter kernelspec uninstall [커널명]

<기타 프로그램 설치>
pip3 install pytorch-cuda=11.7 -c pytorch -c nvidia

pip3 install torch torchvision numpy pandas matplotlip tqdm timm opencv-python

<버전 확인>
torch.__version__

<gpu 상태 확인>
nvidia-smi

<cuda 버전 확인>
nvcc -V  or --version
