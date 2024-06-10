# env_and_install

<가상환경 생성 및 실행> </br>
conda create -n [가상환경명] python=3.8 cudatoolkit==11.4 </br>
conda activate [가상환경명]

<가상환경 목록 확인> </br>
conda info --envs

<가상환경 종료> </br>
conda deactivate

<가상환경 삭제> </br>
conda remove --name [가상환경명] --all

<주피터 노트북 설치> </br>
pip3 install jupyter notebook ipykernel </br>
python -m ipykernel install --user --name [가상환경명] --display-name [커널명]

<커널 목록 확인> </br>
jupyter kernelspec list

<커널 삭제> </br>
jupyter kernelspec uninstall [커널명]

<기타 프로그램 설치> </br>
pip3 install torch==1.9.0+cu111 torchvision==0.10.0+cu111 -f https://download.pytorch.org/whl/torch_stable.html </br>
#pip3 install pytorch-cuda=11.7 -c pytorch -c nvidia </br>
pip3 install torch torchvision numpy pandas matplotlip tqdm timm opencv-python

<버전 확인> </br>
torch.__version__

<gpu 상태 확인> </br>
nvidia-smi

<cuda 버전 확인> </br>
nvcc -V  or --version
