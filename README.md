2020 한국텍학회 제13차 정기총회 및 학술대회에서 TeXnical Vim이라는 주제로
발표한 자료입니다.

## 조판하기
폰트는 Fira Sans, Noto Sans CJK KR, Noto Sans Mono와 Python 및 Pygments가
필요합니다.
폰트의 경우 없으시다면 Homebrew로
```sh
$ brew tap homebrew/cask-fonts
$ brew cask install font-fira-sans font-fira-sans-mono font-noto-sans-cjk font-noto-sans-mono
```
설치하면 되고, Pygments의 경우 (설치하고자 하는 Python에서)
```sh
$ pip install Pygments
```
로 설치하시면 됩니다.
다른 폰트를 원하시는 경우LaTeX 파일의 `% Font Settings %` 부분을 수정하면
됩니다.

XeLaTeX으로 다음과 같이 (두어 번) 조판합니다:
```sh
$ xelatex --shell-escape texnical-vim
```
